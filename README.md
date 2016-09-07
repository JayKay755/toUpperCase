# toUpperCase
//Convert the first character of the string to uppercase

//Преобразование первого символа строки в верхний регистр

public class Solution
{
    

	public static void main(String[] args) throws IOException
    {
        BufferedReader reader = new BufferedReader(new InputStreamReader(System.in));
        String s = reader.readLine();
        char[] ch = s.toCharArray();
        ch[0] = Character.toUpperCase(ch[0]);
        
        for (int i = 1; i < ch.length; i++)
        {
        	if (ch[i-1] == ' ') ch[i] = Character.toUpperCase(ch[i]);
        }
        
        for (int i = 0; i < ch.length; i++)
        {
        	System.out.print(ch[i]);
        }
    }
}
