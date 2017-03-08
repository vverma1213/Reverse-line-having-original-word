# Reverse-line-having-original-word
# Input "This is a good book"
# Output "book good a is This"

###########################Solution##############################

public class TestingString1
{

	public static void main(String[] args)
	{
		String s = "This is a good book";
		String s1 = reverseOriginalString(s);
		System.out.println(s1);
	}

	private static String reverseOriginalString(String s)
	{
		if (s.isEmpty())
		{
			return s;
		}
		String str[] = s.split("\\s");
		for (String s1 : str)
		{
			System.out.print(s1 + " ");
		}
		System.out.println("");
		String temp = "";
		String str1 = "";
		for (int i = 1; i <= str.length; i++)
		{
			str1 = str[str.length - i];
			temp = temp + " " + str1;

		}
		return temp;
	}
}
