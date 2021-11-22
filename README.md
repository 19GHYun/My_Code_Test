# My_Code_Test
```java

import java.util.*;
import java.util.Scanner;


public class Main {
	public static void main(String[] args)
	{
		
		Scanner s = new Scanner(System.in);
		
		int[][] array;
		
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
		int a = 0;
		int b = 0;
		
		doing = s.nextInt();
			
			for(int i = 0; i < doing ; i++) {

				a = s.nextInt();
				b = s.nextInt();
				
				a--;
				b--;
				
				if(array[a][b] == 0) {
					array[a][b] = 1;
				}
				else
					array[a][b] = 0;
				
				if(a-1 < 0) {
					continue;
				}
				else if(a - 1 >= 0) {
				if(array[a-1][b] == 0) {
					array[a-1][b] = 1;
				}
				else if(array[a-1][b] == 1) {
					array[a-1][b] = 0;
				}
				}
					
				if( a + 1 == 3) {
					continue;
				}
				else {
					if(array[a+1][b] == 0) {
						array[a+1][b] = 1;
					}
					else if(array[a+1][b] == 1) {
						array[a+1][b] = 0;
					}
				}
				
				if(b-1 < 0) {
					continue;
				}
				else if( b-1 >= 0) {
					if(array[a][b-1] == 0) {
						array[a][b-1] = 1;
					}
					else if(array[a][b-1] == 1) {
						array[a][b-1] = 0;
					}
				}
				
				
				if(b+1 ==3 ) {
					continue;
				}
				else {
					if(array[a][b+1] == 0) {
						array[a][b+1] = 1 ;
						
					}
					else if(array[a][b+1] == 1) {
						array[a][b+1] = 0;
					}
				}
				
				now_doing++;
				
				int checking = 0;
				
				for(int z = 0; z < 3; z++) {
					for(int k = 0; k < 3; k++) {
						if(array[z][k] == 1) {
							checking = 1;
						}
					
					}
				}
				
				if(checking == 1) {
					System.out.println(now_doing);
					break;
				}
				if(checking == 0 && i == 2) {
					System.out.println("-1");
					break;
				}
			
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
