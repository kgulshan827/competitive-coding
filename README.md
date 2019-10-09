# competitive-coding
contain solution of codechef problems
problem code is  SAKTAN
/* package codechef; // don't place package name! */

import java.util.*;
import java.lang.*;
import java.io.*;

/* Name of the class has to be "Main" only if the class is public. */
class Codechef
{

public static void main (String[] args) throws java.lang.Exception
	{
		// your code goes here
		try
		{
		   
                Scanner sc=new Scanner(System.in);
		long t;
	    t=sc.nextLong();
	    for(int k=0;k<t;k++)
	    {
	        int n=sc.nextInt();
	        int m=sc.nextInt();
	         int z=sc.nextInt();
	        int a[][]=new int[n][m];
	        
	        int p=0;
	        for(int i=0;i<n;i++)
	        {
	            for(int j=0;j<m;j++)
	            {
	                a[i][j]=0;
	            }
	        }
	        
	           
	        
	        for(int i=0;i<z;i++)
	        {
	         int x=sc.nextInt();
	         int y=sc.nextInt();
	         for(int l=0;l<m;l++)
	         {
	             a[x-1][l]= a[x-1][l]+1;
	         }
	       for(int l=0;l<n;l++)
	         {
	             a[l][y-1]= a[l][y-1]+1;
	         }
	        }
	        for(int i=0;i<n;i++)
	        {
	            for(int j=0;j<m;j++)
	            {
	                if(a[i][j]%2==0)
	                {
	                    p++;
	                }
	            }
	        }
	 System.out.println(p);
	        
	    }
	}
	catch(NumberFormatException e)
	{
	System.out.println(e);
	
	}
}}
