# Java
/* You are given a string  that is made of lowercase English alphabets. Determine the length of the smallest S substring that contains the maximum number of distinct characters. */


import java.util.ArrayList;
import java.util.Scanner;

public class MaximumNumberOfDistinctCharacter {

	public static void main(String[] args) {

		Scanner scanner = new Scanner(System.in);
		System.out.println("Enter a String : ");
		String s = scanner.nextLine();
		s = s.toLowerCase();
		char[] ch = s.toCharArray();

		ArrayList<Character> list = new ArrayList<Character>();
		for (char c : ch) {
			if (!list.contains(c)) {
				list.add(c);
			}
		}
		System.out.println(list.size());
		scanner.close();

	}

}
