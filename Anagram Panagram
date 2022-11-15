import java.util.*;

public class AnagAndPanag {
    void anagaram(String s1, String s2) {
        char[] ch1 = s1.toCharArray();
        char[] ch2 = s2.toCharArray();

        Arrays.sort(ch1);
        Arrays.sort(ch2);

        boolean output = Arrays.equals(ch1, ch2);

        if (output) {
            System.out.println("\ngiven string is an anagram");
        } else {
            System.out.println("\ngiven string is not an anagram");
        }
    }

    void panagram(String s){
        int flag=0;
        for(int i=97;i<=122;i++){
            for(int j=0;j<s.length();j++){
                if((char)i==s.charAt(j)){
                    flag +=1;
                    break;
                }
            }
        }
        if(flag ==26){
            System.out.println("\nthe given string is a panagram");
        }
        else{
            System.out.println("\nthe given string is not a panagram");
        }
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        AnagAndPanag obj = new AnagAndPanag();
        char chr;
        do{
            System.out.println("enter your choice \n1.anagram \n2.panagram");
            int choice=sc.nextInt();
            switch(choice){
                case 1:
                System.out.println("enter two strings: ");
                String s1=sc.next();
                String s2=sc.next();
                obj.anagaram(s1, s2);
                break;

                case 2:
                System.out.println("enter a sentence: ");
                String s3=sc.next();
                obj.panagram(s3);
                break;
            }
            System.out.println("do you want to continue: \n 1.if yes enter 'y'");
            chr = sc.next().charAt(0);
        }
        while(chr == 'y' || chr =='Y');
        sc.close();   
}
}


