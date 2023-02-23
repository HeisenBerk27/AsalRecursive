# AsalRecursive
www.patika.dev
----------------


import java.util.Scanner;

public class AsalRecursive {
	
	static boolean Asal(int sayi, int x) {
		if(x==1) {
			return true;
		}
		else {
			if(sayi %x ==0) {
				return false;
			}
			else {
				return Asal(sayi, x-1);
			}
		}
	}

	public static void main(String[] args) {
		
		Scanner scanner = new Scanner(System.in);
		System.out.println("Bir sayı giriniz: ");
        int sayi = scanner.nextInt();
        
        if (Asal(sayi, sayi / 2)) {
            System.out.println(sayi + " asal bir sayıdır.");
        }
        else {
        	System.out.println(sayi + " Asal sayi değildir. ");
        }
	}

}
