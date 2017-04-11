# Core Java（10th, 中文版)
>所有笔记都只记脉络性的东西，细节忽略。笔记的作用只是**提醒**你自己构建体系而已。

---
#Part I 
---
## chapter 5 继承
- 抽象类的使用==abstract==
	- 多个类的抽象，引用与存储更方便（均用抽象类的类型）
- Java中==protected==部分对所有子类和同一个包中的其他类都可见，注意与==public==或==private==的区别；而不加任何修饰符则默认表明对本包可见
- object类是java中所有对象类型的超类
	- equals判断两个对象是否具有相同的引用
	- ==Hash Code== determines the position where the variable is. It may happen that two different variables may have the same place. Pay attention to the following example. The reason is that the hash Code of the String is determined by its content!
	```java
	import java.util.Objects;

	public class hashTest {
	public static void main(String [] args)
	{
 	String s = "OK";
 	StringBuilder sb = new StringBuilder(s);
 	System.out.println(s.hashCode() + " " + sb.hashCode());
 	String t = new String("OK");
 	StringBuilder tb = new StringBuilder(t);
 	System.out.println(t.hashCode() + " " + tb.hashCode());
 	if(Objects.equals(s,t))
 		System.out.println("These are equal!");
 	else
 		System.out.println("Not equal!");		
	}
	}
	```
	- ==toString==method the class name plus the field. to print the int array number, use ==Arrays.toString(number)==. define a toString method is easy for testing
	- 使用泛型数组列表==ArrayList==。类似C++中的向量
		- java中变量给变量赋值，是指针赋值，而不是值赋值
		- ==包装器==将基本数据类型包装成对象。ArrayList的存储类型必须是对象而非基本数据类型
	- 参数数量可变的方法
		```java
		public class paraTest {
		public static double max(double... values){
		double largest= Double.NEGATIVE_INFINITY;
		for(double v:values)
			if(v>largest)
				largest=v;
			return largest;
		}
	
		public static void main(String[] args){
			System.out.println(max(2.1,4.4 ,45.1,-6));
		}
		}
		```
	- ==reflect==特性，主要应用于工具构造者。此处；略过
	
## chapter 6 接口、lambda表达式与内部类
- 接口
	- 接口是为了解决java不支持==多继承性==的问题，每个类都可以有多个接口与一个超类
	- 接口用==implements==关键字标识，并重写接口中的方法，这些方法自动属于public，但在实现时，需要加上public关键字
	- ==instanceof==可用于检验某个对象是否实现了某个接口或者属于某个特定的类
	- 可以为接口实现一个默认实现==default==
	- Arrays.sort有两个版本的调用
	- 对象克隆接口==clonable==与==浅拷贝==
- lambda表达式
	- lambda类似一个函数，实现java传递代码块
	- 方法引用==method reference==是lambda表达式的一种等价表达，共三种类型
	- lambda表达式的作用域，与超类的最终变量==effective final==的引用，与==this==的使用
	- 书上有表格，对应==常用的函数式接口==与==基本类型的函数式接口==
- 内部类
	- 内部类的变量引用与lambda表达式类似。实际上，匿名内部类的作用与lambda表达式的作用类似，两者可以相互替代
	
## chapter 7 异常、断言和日志
- 本章暂时略过
- 可以看一下==Junit==的使用

## chapter 8 泛型程序设计
- 简单的泛型设计的方法
	- 泛型类 
	- 泛型方法
	- 类型变量的限定==extend==
	- 类型擦除（略去）
	- 通配符使用（略去）
	
## chapter 9 集合
- 一些现成的集合类型，实现了相关的代码
- 用到时再来查找！

## chapter 10~12 用户界面的设计
- 使用Windows builder来实现相关的设计
- 具体的组建使用可以查找书上的相关例子
- 善用Google、百度

## chapter 13 部署Java应用程序
- java工程可以打包成jar文件，最后通过其他软件转变为.exe文件
- 网络applet有说明，没有看

## chapter 14 并发
- 线程的基本用法 ==书上section14.1.1==
- 线程的5种状态
- 线程的属性
	- 优先级
	- 守护线程 -- 为其他线程提供服务，例如计时器等
	- 线程组
	- ···
- 线程的同步
	- 锁对象
	- 条件对象
	- ==synchronized==关键字 -- 类似封装了上述的两个对象，提供了一般的需求服务
- 阻塞队列 -- 由相关专家组开发的较高层次的队列形式的多线程服务 
- 线程安全的集合
- ==书上代码14.9~14.11==是相关的例子，可以供参考

---
#Part 2
---

	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	
	

