# Linear-Sort-an-Array
to sort the value as linear Sort -if any small value to change or swapping the index location as ascending order using linear sort
import java.util.Scanner;
class sortArr
{
    Scanner sc=new Scanner(System.in);
    public void sorta1()
    {
        int i,j,n,temp;
        System.out.println("Enter the  no of Elements ");
        n=sc.nextInt();
        int a[]=new int[n];
        System.out.println("Enter the Elements");
        for(i=0;i<n;i++)
        {
            a[i]=sc.nextInt();
        }

        for (i=0;i<n-1;i++)
        {
            for (j=i+1;j<n;j++)
            {
                if(a[i]>a[j])
                {
                    temp=a[i];
                    a[i]=a[j];
                    a[j]=temp;
                }
            }
        }
        System.out.println("Sorted array list");
        for(i=0;i<n;i++)
        {
            System.out.print(a[i]+" , ");
        }
    }
}




public class sortArray1 {
    public static void main(String args[])
    {
        sortArr objArr=new sortArr();
        objArr.sorta1();
    }
}
