using System;
class MainClass {
	public static void PyramidPattern(int n) {
		for (int i = 0; i < n; i++)
		{
			//space
			for (int j = 0; j < n -i -1; j++)
			{
				Console.Write(" ");
			}
		
			//star
			for (int j = 0; j < 2 * i + 1; j++)
			{
				Console.Write("*");
			}
		
			//space
			for (int j = 0; j < n - i - 1; j++)
			{
				Console.WriteLine(" ");
			}
			Console.WriteLine(); // ending line after each row 
		}
	}
	public static void Main(string[] args){
		Console.Write(" Enter theheight of the pyramid: ");
		int n = Convert.ToInt32(Console.ReadLine());
	
	PyramidPattern(n);
}
}
