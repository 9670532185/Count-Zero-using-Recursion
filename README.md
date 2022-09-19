# Count-Zero-using-Recursion
public class Countzero {
    public static int Zero(int n)
    {
        //base case
        if(n==0)
        {
            return 0;
        }
        if(n%10==0)
        {
            return 1+Zero(n/10);
        }
        else{
            return Zero(n/10);
        }

    }
    public static void main(String[] args)
    {
        int n=102000;
        System.out.println(Zero(n));
    }
    
}
