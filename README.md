# Quadraticroots
/*Lab. 1.1) Write a Java program to find the discriminant value D and find out the roots of 

the quadratic equation of the form ax2+bx+c=0.*/

import java.util.*;

import java.lang.Math;

class QuadraticRoots {

	public static void main(String[] args) {		
  
    int a,b,c,d,deno;

		double x,r1,r2;

		Scanner s=new Scanner(System.in);

		System.out.print("Enter coefficients of quadratic equation:");

		a=s.nextInt();

		b=s.nextInt();

		c=s.nextInt();

		d=b*b-4*a*c;

		deno=2*a;

		x= Math.sqrt(d);

		if(d>=0)

		{

			if(d>0)

			{

				r1=(-b+x)/deno;

				r2=(-b-x)/deno;

				System.out.println("Roots are real and distint"+ " "+"r1="+r1+"   "+"r2="+r2);

			}

			else

			{

				r1=-b/deno;

				r2=-b/deno;

				System.out.println("Roots are real and equal"+ " "+"r1="+r1+"   "+"r2="+r2);

			}

		}

		else

		{

			System.out.println(" Roots are imaginary");

		}

	}

}
© 2021 GitHub, Inc.
