Write a program for leader board position
input1:11
input2:21 19 20 18 17 19 16 15 9 11 1      
output: 11 15 16 19 20 21 


using System;
 
public class HelloWorld
{
    public static void Main(string[] args)
    {
        int a = Convert.ToInt32(Console.ReadLine());
 
        //string str=Console.ReadLine();
        string rts=Console.ReadLine();
        string[] str=rts.Split(" ");
        int[] arr=new int[a];
        for(int i=0;i<a;i++)
        {
            arr[i]=Convert.ToInt32(str[i]);
        }
        int k=arr[a-1];
        for(int j=a-2;j>=0;j--)
        {
            if(arr[j]>k)
            {
                Console.Write(arr[j]+" ");
                k=arr[j];
 
            }
        }
    }
}


Program to find unnion of two arrays
ip1: 5
2 3 4 7 1
4
4 1 3 5

1 2 3 4 5 7


using System;
 
public class HelloWorld
{
    public static void Main(string[] args)
    {
        int a = Convert.ToInt32(Console.ReadLine());
        string rts=Console.ReadLine();
        string[] str=rts.Split(" ");
        int[] arr=new int[a];
        for(int i=0;i<a;i++)
        {
            arr[i]=Convert.ToInt32(str[i]);
        }
        int b = Convert.ToInt32(Console.ReadLine());
        string rts2=Console.ReadLine();
        string[] str2=rts.Split(" ");
        int[] brr=new int[b];
        for(int i=0;i<b;i++)
        {
            brr[i]=Convert.ToInt32(str2[i]);
        }
        int[] crr=new int[a+b];
        for(int i=0;i<a;i++)
        {
            crr[i]=arr[i];
        }
        for(int k=0,l=a;k<b;l++,k++)
        {
            crr[l]=brr[k];
 
        }
        Array.Sort(crr);
        for(int h=0;h<a+b;h++)
        {
            bool flag=false;
            for(int y=0;y<h;y++)
            {
                if(crr[y]==crr[h])
                {
                    flag = true;
                }
            }
            if(flag==false)
            {
                Console.Write(crr[h]+" ");
            }
        }
    }
}



binary search




