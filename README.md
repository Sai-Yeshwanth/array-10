import java.util.Scanner;

class Add{
	static int arr[] = new int[100];
	static Scanner input = new Scanner(System.in);
	public static void addarr()
	{
		System.out.println("Enter size of array:");
		int n = input.nextInt();
		System.out.println("Enter "+ n +" elements of array");
		for(int i=0;i<n;i++)
		{
			arr[i] = input.nextInt();
		}
		System.out.println("duplicate elementts are:");
		 for(int i = 0; i < n; i++) 
		 {  
		        for(int j = i + 1; j < n; j++) 
		        {  
		            if(arr[i] == arr[j])  
		                System.out.println(arr[j]); 
		        }  
		  }  
		
	}
}

public class Jala {

	public static void main(String[] args) {
		Add a = new Add();
		a.addarr();
	}
}
