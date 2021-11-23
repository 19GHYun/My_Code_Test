# My_Code_Test
```java

import java.util.*;
import java.util.Scanner;


public class Main {
	public static void main(String[] args)
	{
		
		Scanner s = new Scanner(System.in);
		
		int[][] array;
		int[] a;
		int[] b;
		int[] checking;
		
		array = new int[3][3];
		/*
		array[0][0] = 1;
		array[0][1] = 0;
		array[0][2] = 0;
		array[1][0] = 0;
		array[1][1] = 1;
		array[1][2] = 1;
		array[2][0] = 1;
		array[2][1] = 0;
		array[2][2] = 0;
		*/
		
		for(int i = 0; i < 3; i++) {
			array[i][0] = s.nextInt();
			array[i][1] = s.nextInt();
			array[i][2] = s.nextInt();
			
		}
		
		int doing;
		int now_doing = 0;
		doing = s.nextInt();
		
		a = new int[doing];
		b = new int[doing];
		
		for(int i = 0; i < doing ; i++) {
			a[i] = s.nextInt();
			b[i] = s.nextInt();
		
			a[i]--;
			b[i]--;
		}
		
		for(int i = 0; i < doing ; i++) {
		if(array[a[i]][b[i]] == 0) {
			array[a[i]][b[i]] = 1;
		}
		else
			array[a[i]][b[i]] = 0;
		
		if(a[i]-1 < 0) {
			
		}
		else if(a[i] - 1 >= 0) {
		if(array[a[i]-1][b[i]] == 0) {
			array[a[i]-1][b[i]] = 1;
		}
		else if(array[a[i]-1][b[i]] == 1) {
			array[a[i]-1][b[i]] = 0;
		}
		}
			
		if( a[i] + 1 == 3) {
			
		}
		else {
			if(array[a[i]+1][b[i]] == 0) {
				array[a[i]+1][b[i]] = 1;
			}
			else if(array[a[i]+1][b[i]] == 1) {
				array[a[i]+1][b[i]] = 0;
			}
		}
		
		if(b[i]-1 < 0) {
		
		}
		else if( b[i]-1 >= 0) {
			if(array[a[i]][b[i]-1] == 0) {
				array[a[i]][b[i]-1] = 1;
			}
			else if(array[a[i]][b[i]-1] == 1) {
				array[a[i]][b[i]-1] = 0;
			}
		}
		
		
		if(b[i]+1 ==3 ) {
			
		}
		else {
			if(array[a[i]][b[i]+1] == 0) {
				array[a[i]][b[i]+1] = 1 ;
				
			}
			else if(array[a[i]][b[i]+1] == 1) {
				array[a[i]][b[i]+1] = 0;
			}
		}
		
		now_doing++;
		
		/*for(int z = 0; z < 3; z++) {
			for(int k = 0; k < 3; k++) {
				System.out.print(array[z][k]);
				System.out.print(" ");
				}
			System.out.println("");
			}
		System.out.println(now_doing);
		*/
		
		checking = new int[9];
		
		int c = 0;
		
		for(int z = 0; z < 3; z++) {
			for(int k = 0; k < 3; k++) {
				if(array[z][k] == 1) {
					checking[c] = 1;
				}
				c++;
			
			}
		}
		if(checking[0] == 1 && checking[1] == 1 && checking[2] == 1 && checking[3] == 1 && checking[4] == 1 && checking[5] == 1 && checking[6] == 1 && checking[7] == 1 && checking[8] == 1) {
			System.out.println(now_doing);
			break;
		}
		else if(now_doing == doing) {
			if(checking[0] == 1 && checking[1] == 1 && checking[2] == 1 && checking[3] == 1 && checking[4] == 1 && checking[5] == 1 && checking[6] == 1 && checking[7] == 1 && checking[8] == 1) {
				System.out.println(now_doing);
				break;
			}
			else {
				System.out.println("-1");
				break;
			}
			
		}
		else {
			checking[0] = 0;
			checking[1] = 0;
			checking[2] = 0;
			checking[3] = 0;
			checking[4] = 0;
			checking[5] = 0;
			checking[6] = 0;
			checking[7] = 0;
			checking[8] = 0;
		}
		
		
		
		
		}
		
		/*for(int z = 0; z < 3; z++) {
			for(int k = 0; k < 3; k++) {
				System.out.print(array[z][k]);
				System.out.print(" ");
				}
			System.out.println("");
			}
		
		System.out.println(doing);
		
		for(int j = 0; j < doing ; j++) {
		System.out.print(b[j]);
		}
		*/
	}

	
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		
		/*
		int a;
		
		Scanner s = new Scanner(System.in);
		
		a = s.nextInt();
		
		int[][] array;
		array = new int[a][a];
		
		int d = 0;
		int e = 0;
		
		int c = array[d][e];
		
		String b;
		
		s.nextLine();
		
		b = s.nextLine();
		
		//System.out.println(b + b.length());
		
		String[] words = b.split(" ");
		
		//System.out.println(words.length);
		
		for(int i = 0; i < words.length; i++) {
		if(words[i].equals("R")) {
			if(e > a-1) {
			
			}
			else
				e++;
		
		}
		else if(words[i].equals("L")) {
			if(e == 0) {
	
			}
			else
				e--;

		}
		else if(words[i].equals("D")) {
			if(d > a-1) {

			}
			else
				d++;

		}
		else if(words[i].equals("U")) {
			if(d==0) {

			}
			else
			d--;

		}
		}
		d++;
		e++;
		System.out.println(d +" "+ e);*/
	}
		
}

```
