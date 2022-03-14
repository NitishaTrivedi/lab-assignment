package Assignment_1;
//ASSIGNMENT 1 QUESTION 2
import java.util.Scanner;

public class GradesAverage {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc=new Scanner(System.in);
		System.out.println("Enter the number of students:");
		int num=sc.nextInt();
		double sum=0;
		int marks[]=new int[num];
		for(int i=0;i<num;i++) {
			System.out.println("Enter the marks for Student"+(i+1));
			marks[i]=sc.nextInt();
			boolean flag=check(marks,i);
			if (flag==true) {
				sum+=marks[i];
			}
		}
			System.out.println("Average is: "+(sum/num));


	}
	public static boolean check( int marks[], int i) {
		Scanner sc=new Scanner(System.in);
		if(marks[i]>100 || marks[i]<0) {	
			System.out.println("Try Again and Re-Enter the marks");
			marks[i]=sc.nextInt();
			boolean flag=check(marks,i);
		}
		return true;
	}


}
