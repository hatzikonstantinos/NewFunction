# NewFunction
/*
 * Click nbfs://nbhost/SystemFileSystem/Templates/Licenses/license-default.txt to change this license
 * Click nbfs://nbhost/SystemFileSystem/Templates/Project/Maven2/JavaApp/src/main/java/${packagePath}/${mainClassName}.java to edit this template
 */

package com.mycompany.mavenproject2;

import java.util.Scanner;

/**
 *
 * @author User
 */
public class Mavenproject2 {

   public static void main(String[] args) {
        printperson();
   }
   public static void printperson(){
        String name;
        int age;
        int children;
        char gender;
        double salary;
        
        Scanner console=new Scanner(System.in);
        System.out.println("Enter name:");
        name=console.nextLine();
        System.out.println("Enter age:");
        age=console.nextInt();
        System.out.println("Enter gender:(F/M)");
        gender=console.next().charAt(0);
        System.out.println("Enter salary:");
        salary=console.nextDouble();
        System.out.println("Enter number of children");
        children=console.nextInt();
        System.out.println("Name: "  + name +  "\nAge: "+age+ "\nGender: " +gender+ "\nSalary: "+salary+ "\nChildren: " +children);
        if (children>2){
            System.out.println("Salary is: " +(salary+(salary*0.20)));
        }else if(children==0){
            System.out.println("Your salary is still the same");
        }
    }
}
