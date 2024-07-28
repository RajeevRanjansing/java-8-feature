Method Reference are special type of lambda expression.
They are often used to create simple lambda expression by referencing existiong method.
Each time when you are using lambda expression to just referring a method.You can replace your lambda expression with method reference.
It is alternative to lambda expression.
It is powerful tool that can be used to make code more concise and readable.
Type of method reference
1)Static method
2)Instance method of particular object
3)constructor 

program 1

import java.util.*;
class methodref{
    public static void main(String args[]){
        dog d=new dog();
        Runnable r=d::bark;     //Runnable is used when there is no argument 
        r.run();
    }
}
class dog{
    public void bark(){
        System.out.println("Bhow Bhow!!!");
    }
}

program 2

import java.util.*;
class methodref{
    public static void main(String args[]){
        calculator c=new calculator();
        Comparator<Integer>d=c::cal;        //This is not right way to use comparator
        int result=d.compare(15,10);        //here argument is present.so, we can't use runnable
        System.out.println(result);
    }
}
class calculator{
    public int cal(int x, int y){
        return (x+y);
    }
}

//program 3

import java.util.*;
class methodref{
    public static void main(String args[]){
        System.out.println("Method Class \n *****************");
        WorkInter workInter=Stuff::doSuff;
        workInter.doTask();
    }
}
class Stuff{
    public static void doSuff(){
        System.out.println("I am doing task");
    }
}

interface WorkInter{
    public void doTask();
}

//program 4

import java.util.*;
import java.time.LocalDate;
class methodref{
    public static void main(String args[]){
        System.out.println("I am currently doing BE \n From Laxmi institute of Technology");
        a b=stuff::Stuff;
        b.doTask();
    }
}



class stuff{
    public static void Stuff(){
        System.out.println("I am learning some new task");
        System.out.println("So, I am busy right now");
        LocalDate now=LocalDate.now();
        System.out.println(now.toString());
    } 
}

interface a{
    public void doTask();
}
