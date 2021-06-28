
import java.util.ArrayList;
import java.util.Collections;
import java.util.Scanner;
import java.util.List;
import java.util.Scanner;


public class Arrays {
	public static void main(String[] args) {
		
		Scanner input=new Scanner(System.in);
   
		List<Doubles> numbers=new ArrayList<>();
		for(int i=0; i<5; ++i)
		{
			System.out.println("Enter a number");
			numbers.add(Doubles.parseDouble(input.nextline()));
			
		}
        Double sum=0;
        Double product=1.0;
        for(Double number: numbers)
        {
        	sum+number;
        	product*=number;
        }
        System.out.println("The sum is:"+sum);
        System.out.println("The product is:"+product);
        Collections.sort(numbers);
        System.out.println("The maximum is:"+numbers.get(5));
        System.out.println("The minimum is:"+numbers.get(0));
	}
	
	}

}
