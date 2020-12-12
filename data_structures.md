[Home](README.md) - [Code Review](CodeReview.md) - [Data Structures and Algorithms](data_structures.md) - [Software Engineering and Design](softeng_design.md) - [Databases](databases.md)

<h1>Data Structures</h1>

 ## Narrative
 
 This artifact is a simple C++ grading program. It is a easy to use grading system teachers can use to enter a student's grades and get the average and letter grade. This code was chosen was because I felt it was structured to be simple but yet very powerful program. Using the mathmatic coding to reach the desired results shows how structure is important to excuting the code. I customized the program to have five grades entered. Once they are entered, the program runs and a grade is given. 
 
 ## C++ Code Grading Program
 
```
#include<iostream>
using namespace std;
int main()
                   {
        
        /*Stating there will be five assignments*/
        int marks[5], i;
        float sum=0,avg;
 
 
        /*Instructs user to enter grades for the student*/
        cout<<"\n Enter Grade of Student \n";
        cout<<"------------------------------------";

        /*List name of assignments*/
        cout<<"\n Milestone:One : ";
        cin>>marks[0];
        cout<<"\n Milestone:Two : ";
        cin>>marks[1];
        cout<<"\n Milestone:Three : ";
        cin>>marks[2];
        cout<<"\n Milestone:Four : ";
        cin>>marks[3];
        cout<<"\n Final Project : ";
        cin>>marks[4];

        for(i=0;i<5;i++)
        {
                sum=sum+marks[i];
        }
        cout<<"------------------------------------";

        /*Calculates and prints results*/
        cout<<"\n Total Marks of Student = "<<sum;
        avg=sum/5;
        cout<<"\n Average = "<<avg;
        cout<<"\n Grade   = ";

        if(avg>80)
        {
                cout<<"A";
        }
        else if(avg>60 && avg<=80)
        {
                cout<<"B";
        }
        else if(avg>40 && avg<=60)
        {
                cout<<"C";
        }
        else
        {
                cout<<"D";
        }
        return 0;
}
```



## Enhancements

This a simple reconstruction of the C++ grading program I used before but this time it is built using java. Having the ability to be flexible is important when trying to achieve a goal. I decided to convert the grading program from C++ to Java because it made more sense to me to present my knowledge of achieving the same goal through different means. This program again shows the algorithm of producing the mean of a sum of numbers. Though it is a simple program, it does show how effective the algorithm is and how productive the program can be for a teacher's grading technique. I believe I have met the objectives given. I wanted to enhance the project by showcasing my ability to achieve a goal in different ways. This ability is a crucial skill that will provide me support going forward in the real world working environment. This was something I find that I am very comfortable working in. Early in the program, I had the opportunity to work with both C++ and Java. They are my favorite languages to use and I tried to use them periodically to stay fluent in them. I found that my original set up names each assignment. I realized that it wouldn’t be needed because as long as each assignment's grade was entered correctly, the result would be right. So I simplified the java version and just names each assignment “subject”. 

##Enhancement Java Grading Program
```
import java.util.Scanner;

public class Main
{
    public static void main(String args[])
    {
    	/* This program assumes that the student has 5 subjects,*/
        int marks[] = new int[5];
        int i;
        float total=0, avg;
        Scanner scanner = new Scanner(System.in);
		
        
        for(i=0; i<5; i++) { 
           System.out.print("Enter Marks of Subject"+(i+1)+":");
           marks[i] = scanner.nextInt();
           total = total + marks[i];
        }
        scanner.close();
        //Calculating average here
        avg = total/6;
        System.out.print("The student Grade is: ");
        if(avg>=80)
        {
            System.out.print("A");
        }
        else if(avg>=60 && avg<80)
        {
           System.out.print("B");
        } 
        else if(avg>=40 && avg<60)
        {
            System.out.print("C");
        }
        else
        {
            System.out.print("D");
        }
    }
}
```



[Home](README.md) - [Code Review](CodeReview.md) - [Data Structures and Algorithms](data_structures.md) - [Software Engineering and Design](softeng_design.md) - [Databases](databases.md)
