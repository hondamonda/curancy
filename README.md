// Конвертор за мерни единици
//Да се напише програма, която преобразува разстояние между следните 8 мерни единици: m, mm, cm, mi, in, km, ft, yd. Използвайте съответствията от таблицата по-долу:
//
входна единица
изходна единица
1 meter (m)
1000 millimeters (mm)
1 meter (m)
100 centimeters (cm)
1 meter (m)
0.000621371192 miles (mi)
1 meter (m)
39.3700787 inches (in)
1 meter (m)
0.001 kilometers (km)
1 meter (m)
3.2808399 feet (ft)
1 meter (m)
1.0936133 yards (yd)
package hello;

import java.util.Scanner;

public class Hello {
	
	public static void main(String[] args){

		Scanner scan = new Scanner(System.in);
		double n = Double.parseDouble(scan.nextLine());
		String input = scan.nextLine();
		String output = scan.nextLine();
		scan.close();
		double convert = 0;
		
		switch(input) {
		case  "m" : convert = n; break;
		case "mm" : convert = n / 1000; break;
		case "cm" : convert = n / 100; break;
		case "mi" : convert = n / 0.000621371192; break;
		case "in" : convert = n / 39.3700787; break;
		case "km" : convert = n / 0.001; break;
		case "ft" : convert = n / 3.2808399; break;
		case "yd" : convert = n / 1.0936133; break;
		}

		switch (output) {
		case  "m" : convert = convert * 1; break;
		case "mm" : convert = convert * 1000; break;
		case "cm" : convert = convert * 100; break;
		case "mi" : convert = convert * 0.000621371192; break;
		case "in" : convert = convert * 39.3700787; break;
		case "km" : convert = convert * 0.001; break;
		case "ft" : convert = convert * 3.2808399; break;
		case "yd" : convert = convert * 1.0936133; break;
		}
		
		System.out.println(convert + " " + output);
	}
}
