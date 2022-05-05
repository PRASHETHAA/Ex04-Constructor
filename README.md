# Ex04-Constructor
## Aim:
 To write a C# program to calculate the salary of an employee by passing the name, designation, noofexperience, basic salary and insurance amount through constructor.
 
 ## Algorithm:
 ### Step1:
 
 
 
 ## Program:
 ```
 using System;  
   public class Employee  
    {  
        public String job;  
        public String name;  
        public int exp;  
        public int bs;  
        public int insurance;
        double hra,ta,salary;  
        public Employee(String name, String job,int exp,int bs,int i)  
        {  
            this.name = name;  
            this.job = job;  
            this.exp = exp;
            this.bs=bs;
            this.insurance=i;  
        }  
        public void Salary(){
            hra = this.bs*0.2;
            ta=this.bs*0.1;
            salary = this.bs+hra+ta-insurance;
        }
        public void display()  
        {  
            Console.WriteLine("Name of the employee is "+ this.name+ " having "+this.exp+ " of experience, working as " +this.job+" Receives " +salary+ " of salary");
        }   
   }  
   class TestEmployee{  
       public static void Main(string[] args)  
        {  
            String nam,jo;
            int ex;int b;int ins;
            nam=Console.ReadLine();
            jo=Console.ReadLine();
            ex=Convert.ToInt32(Console.ReadLine());
            b=Convert.ToInt32(Console.ReadLine());
            ins=Convert.ToInt32(Console.ReadLine());
            Employee e1 = new Employee(nam,jo,ex,b,ins);  
            e1.Salary();   
            e1.display();  
  
        }  
    }
    ```
 ## Output:
 ![4exp](https://user-images.githubusercontent.com/75234942/166975935-2ac9ab46-c751-4c7b-a846-e2c3f85ab321.png)

 ## Result:
