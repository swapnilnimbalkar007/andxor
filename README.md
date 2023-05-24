import java.util.*; 
class operation{ 
 
    // AND operation 
    void AND(String str1) 
    { 
        char ch[]=new char[str1.length()]; 
 
        //copying char 
        for(int i=0;i<str1.length();i++) 
        { 
            ch[i]=str1.charAt(i); 
        } 
 
        System.out.println("\nResult of bitwise AND operation is : "); 
 
        for(int i=0;i<str1.length();i++) 
        { 
            int ans=(int)ch[i] & 127; 
            char result=(char)ans; 
 
            System.out.print(result); 
        } 
    } 
 
    //OR operation 
    void XOR(String str1) 
    { 
        char ch[]=new char[str1.length()]; 
 
        //copying char 
        for(int i=0;i<str1.length();i++) 
        { 
            ch[i]=str1.charAt(i); 
        } 
        System.out.println("\n\nResult of bitwise XOR operation is : "); 
 
        for(int i=0;i<str1.length();i++) 
        { 
            int ans=(int)ch[i] ^ 127; 
            char result=(char)ans; 
 
            System.out.println(result); 
        } 
    } 
} 
public class Assign_1 { 
    public static void main(String args[]) throws Exception 
    { 
        Scanner sc=new Scanner(System.in); 
        System.out.print("Enter the String : "); 
        String str= sc.nextLine(); 
        System.out.println("\nEntered string is : "+str); 
 
        operation op=new operation(); 
        op.AND(str); 
        op.XOR(str); 
    } 
} 
