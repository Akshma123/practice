class Person
{
 String name;
 int yearOfBirth;
 Person(String name,int yearOfBirth)
 {
   this.name=name;
   this.yearOfBirth=yearOfBirth;
 }
}
class Student extends Person
{
 String major;
 Student(String major)
 {
  super("akshma",1996);
  this.major=major;
 }
 public void display()
 {
  System.out.println(name+" "+yearOfBirth+" "+major);
 }
}
class Instructor extends Person
{
 double salary;
 Instructor(double salary)
 {
  super("akki",1995);
  this.salary=salary;
 }
 public void display()
 {
  System.out.println(name+" "+yearOfBirth+" "+salary);
 }
} 
 class TestPerson
{
 public static void main(String[] args)
 {
  Student s=new Student("cse");
  Instructor i=new Instructor(50000);
  s.display();
  i.display();
 }
}
