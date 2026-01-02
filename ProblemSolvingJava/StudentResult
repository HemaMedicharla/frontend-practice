package ProblemSolving;

import java.util.Scanner;

public class StudentResult {
	public String studentName;
	public int studentId;
	public String courseName;
	public double totalMarks;
	
	//parameterized constructor
	public StudentResult(String studentName,int studentId,String courseName,double totalMarks) {
		this.studentName=studentName;
		this.studentId=studentId;
		this.courseName=courseName;
		this.totalMarks=totalMarks;
		System.out.println("Student Record Created Successfully");
	}
	public void addMarks(double marks) {
		
		if(marks<=0) {
			System.out.println("Invalid marks entered");
			return;
		}
		totalMarks += marks;
		System.out.println("Marks Updated Successfully  :"+totalMarks);
	}
	public void viewTotalMarks() {
		System.out.println("TotalMarks :"+totalMarks);
		return;
	}
	public void calculateGrade() {
        if(totalMarks==0) {
			System.out.println("No marks available to calculate grade");
			return;
		}
        System.out.println(" Student TotalMarks :"+totalMarks);
		if(totalMarks>=90) {
			System.out.println("'A' Grade");
		}else if(totalMarks>=80 && totalMarks<=89) {
			System.out.println("'B' Grade");
		}else if(totalMarks>=70 && totalMarks<=79) {
			System.out.println("'C' Grade");
		}else if(totalMarks>=60 && totalMarks<=69) {
			System.out.println("'D' Grade");
		}else if(totalMarks<60) {
			System.out.println("FAIL");
		}else {
			System.out.println("Invalid marks entered");
		}
		
	}
	public void exit() {
	
		System.out.println("Thank You! Result Processing Completed.");
	}

	public static void main(String[] args) {
		Scanner sc=new Scanner(System.in);
		
		System.out.println("Enter your name :");
		String studentName=sc.nextLine();
		System.out.println("Enter your student Id :");
		int studentId=sc.nextInt();
		sc.nextLine();
		System.out.println("Enter your course name :");
		String courseName=sc.nextLine();
		System.out.println("Enter your total marks :");
		double totalMarks = sc.nextDouble();
		StudentResult student=new StudentResult(studentName,studentId,courseName,totalMarks);
		System.out.println("---------Menu-------");
		int choice=0;
		do {
			System.out.println("What do you want to do");
			System.out.println("Enter 1 to add marks to previous marks");
			System.out.println("Enter 2 to calculate grade");
			System.out.println("Enter 3 to view total marks");
			System.out.println("Enter 4 to exit");
			choice=sc.nextInt();
			switch(choice)
			{
			case 1:
				System.out.println("Add more subject marks");
				double marks=sc.nextDouble();
				student.addMarks(marks);
				break;
			case 2:
				System.out.println("Calculate grade");
				student.calculateGrade();
			    break;
			case 3:
				System.out.println("View total marks");
				student.viewTotalMarks();
				break;
			case 4:
				System.out.println("Exit");
				student.exit();
				break;
			default:
			    System.out.println("Invalid option");
			}
		}while(choice!=4) ;
			
		sc.close();
			
		
		}

}	
	
		
	

