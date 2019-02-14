# Strings
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.util.Scanner;
import java.util.StringJoiner;

public class HelloWorld {

	public static void main(String[] args) throws IOException {

		StringJoiner sj = new StringJoiner(": ", "[ ", "]");
		sj.add("Mill").add("Weino").add("Aruka");

		String desiredString = sj.toString();

		System.out.println(desiredString);

		Scanner input = new Scanner(System.in);

		System.out.println("Enter your fname");
		String fname = input.nextLine();

		System.out.println("Enter your lname");
		String lname = input.nextLine();

		System.out.println("Enter your age");
		int age = input.nextInt();

		System.out.println("You are " + fname + " " + lname + " and " + age + " years old");

		String input1 = null;
		BufferedReader in = new BufferedReader(new InputStreamReader(System.in));
		System.out.println("Enter your name");
		input1 = in.readLine();
		in.close();
	}

}
