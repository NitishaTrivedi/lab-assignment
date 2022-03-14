package Assignment_1;

import java.util.Scanner;

// 	QUESTION 4
public class Pascal {
	public static void main(String args[]) {
		Scanner sc = new Scanner(System.in);
		int n, i, j, a[][];
		System.out.println("Enter the no. of steps");
		n = sc.nextInt();
		a = new int[n][n];
		for (i = 0; i < n; i++) {
			for (j = 0; j <= i; j++)
				if (j == 0 || j == i)
					a[i][j] = 1;
				else
					a[i][j] = a[i - 1][j - 1] + a[i - 1][j];
		}
		for (i = 0; i < n; i++) {
			for (j = 0; j <= i; j++)
				System.out.print(a[i][j] + " ");

			System.out.println();
		}
	}
}
