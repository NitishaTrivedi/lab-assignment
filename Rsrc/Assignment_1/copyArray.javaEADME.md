package Assignment_1;
//ASSIGNMENT 1 QUESTION 3
import java.util.*;

public class copyArray {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner sc=new Scanner(System.in);
		System.out.println("Enter the size of array:");
		int l=sc.nextInt();
		int arr[]=new int[l];
		System.out.println("Enter array elements:");
		for(int i=0;i<arr.length;i++) {
			arr[i]=sc.nextInt();
		}
		int result[]=new int[l]; 
		result=Arrays.copyOf(arr,l);
		System.out.println("Copied Array:");
		for(int i=0;i<result.length;i++) {
			System.out.print(result[i]+" ");
		}
	}
}
