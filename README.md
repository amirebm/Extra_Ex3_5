/* Write a program that prompts the user to enter an integer for
today’s day of the week (Sunday is 0, Monday is 1, …, and Saturday is 6). Also
prompt the user to enter the number of days after today for a future day and display
the future day of the week. */

# Extra_Ex3_5

package com.personal.Extra5;

import java.util.Scanner;

public class Extra3_5 {

	public static void main(String[] args) {

		Scanner sc= new Scanner(System.in);
		int currentDay,futureDay,day;
		System.out.println("Enter today's day");
		currentDay= sc.nextInt();
		System.out.println("Enter the number of days elapsed since today");
		futureDay= sc.nextInt();
		if (futureDay <=7)
			day= futureDay-currentDay;
		else
		day= (futureDay% 7)+ (currentDay);
		
		switch (currentDay) {
		case 0:
			System.out.println("Sunday is today");
			break;
		case 1:
			System.out.println("Monday is today ");
			break;
		case 2:
			System.out.println("Thursday is today");
			break;
		case 3:
			System.out.println("Wednesday is today");
			break;
		case 4:
			System.out.println("Tuesday is today");
			break;
		case 5:
			System.out.println("Friday is today");
			break;
		case 6:
			System.out.println("Saturday is today");
			break;
		
		}
		
		
		switch (day) {
		case 0:
			System.out.println(" and the future day is Sunday");
			break;
		case 1:
			System.out.println("and the future day is Monday ");
			break;
		case 2:
			System.out.println("and the future day is Thursday");
			break;
		case 3:
			System.out.println("and the future day is Wednesday");
			break;
		case 4:
			System.out.println("and the future day is Tuesday");
			break;
		case 5:
			System.out.println("and the future day is Friday");
			break;
		case 6:
			System.out.println("and the future day is Saturday");
			break;
		
		}
				
	}

}
