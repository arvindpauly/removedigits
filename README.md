# removedigits
import java.util.Arrays;
import java.util.Scanner;
public class Removedigits {
	public static void main(String[] args) {
		Scanner a = new Scanner(System.in);
		System.out.println("enter the number");
		String num = a.next();
		System.out.println("enter no of digits to delete");
		int del = a.nextInt();
		char[] ac = num.toCharArray();
		Arrays.sort(ac);
          String out = "";
		for (int countDigit = 0; countDigit < ac.length - del; countDigit++) {
			out = out.concat(ac[countDigit] + "");
		}
		System.out.println(out);

	}

}
