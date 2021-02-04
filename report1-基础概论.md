# Java基础概论.实验报告
## 实验目的：
通过实验，掌握Java基础环境搭建过程，熟悉Java编译运行流程。学会编写简单基础的Java程序。
## 实验准备与环境：
1.操作系统：Windows XP/2003/7
2.IDE：Eclipse + JDK1.7
## 实验要求：
1.编写一个Java程序，从键盘上输入你的个人信息：姓名，性别，年龄，爱好，然后定义相关变量来保存你自己输入的这些信息，最后将这些变量格式化后输出打印。
要求：对用户输入的信息进行验证，要求性别必须是男或女，年龄必须在18到60之间，爱好必须不能超过4个;

2.让用户输入10个任意的数字，把其中的奇数都打印出来，并且以3个一行的格式进行打印，每行打印的数字之间用空格隔开;

3.使用三种循环结构（while，do-while，for）实现将200-300之间所有能同时被3和7整除的数字之和求出来;

4.计算1！+2！+3！+4！+。。。+n！之和，其中n的值由用户来输入;

## 实验步骤：
1.第一题代码如下：
**代码**
---java
import java.util.Scanner;//先调用Scanner
public class javatry1 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		//1,
		Scanner r=new Scanner(System.in);
		System.out.println("请输入您的姓名：  \n");//用户输入
		String n=r.next();
		System.out.println("请输入您的性别：  \n");//用户输入
		String y=r.next();
		System.out.println("请输入您的年龄：  \n");//用户输入
		 int ag=r.nextInt();
		System.out.println("请输入您的爱好： \n ");//用户输入
		String hb=r.next();
		
		person p=new person();

		p.check(n,y,ag,hb);

	}

}

class person{
	 String name;//名字
	 String x;//性别
	 int ager ;//年龄
	 String hbt;//爱好
	 
	public void check(String name,String x,int ager,String hbt){//验证
		if(x.equals("男") && ager>=18 || ager<=60){
			System.out.println("姓名：\n"+name+"性别：\n"+x+"年龄：\n"+ager+"爱好：\n"+hbt);
		}
		else if(x.equals("女")&& ager>=18 || ager<=60){
			System.out.println("姓名：\n"+name+"\n性别：\n"+x+"\n年龄：\n"+ager+"\n爱好：\n"+hbt);
		}
		else{
			System.out.println("您的输入不正确！");
		}
	}
	
}
---
## 分析与总结：
- Bulleted
- List

1. Numbered
2. List

3.huhh
**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image]()
