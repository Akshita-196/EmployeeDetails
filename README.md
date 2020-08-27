# EmployeeDetails
package employee;
import java.util.*; 
public class Employee {
    String Name;
    int Salary;
    int YearOfJoining;
    String Address;
        public void GetData(){
            Scanner sc= new Scanner(System.in);
            
            Name =sc.nextLine();
            Salary = sc.nextInt();
            YearOfJoining = sc.nextInt();
            Address = sc.next();
        }
        public void PrintData(){
            System.out.println(Name+"    "+Salary+"   "+YearOfJoining+"          "+Address);
        }
    public static void main(String[] args) {
        Employee[] emp=new Employee[3];
        for(int i=0;i<3;i++){
            emp[i]=new Employee();
            System.out.println("enter employee details i.e Name,Salary,YearOfJoining,Address: ");
            emp[i].GetData();
        }
        System.out.println("Name   Salary  YearOfJoining    Address");
        for (int i=0;i<3;i++){
            emp[i].PrintData();
        }
        
    }
    
}
