// _8_CountOfEqualBitPairs
import java.util.Scanner;
public class _8_CountOfEqualBitPairs {
	public static void main(String[] args) {
		Scanner input=new Scanner(System.in);
		int n=input.nextInt();
		int count=0;
		String binN=Integer.toBinaryString(n);		
		char[] bits=binN.toCharArray();	
		for (int i = 0; i < binN.length()-1; i++) {
			if (bits[i+1]==bits[i]) {
				count++;
			}
		}
		
		System.out.println(count);
	}

}
