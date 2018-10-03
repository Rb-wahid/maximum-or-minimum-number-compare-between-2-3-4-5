
import java.util.Scanner;


/**
 *date 10/3/2018
 * time 12:15 AM
 * @author Rb wahid
 */
public class maximumOrMinimumNumberCheck {
    static Scanner myScanner = new Scanner(System.in);
    public static void main(String[] args){
        String ans ;
        prln("What do you want to check,Minimum Number or Maximum Number??");
        pr("Answer:");
        ans = myScanner.nextLine();
        
        //for minimum
        if("minimum".equals(ans.toLowerCase())){
            //User input:how many numbers compare 
            pr("How many numbers do you want to compare? <You can compare the maximum number of 5 numbers..> \nAnswer:");
            int compareBetween = myScanner.nextInt();
            switch(compareBetween){
                case 2:
                    int a, b, result;
                    pr("Input value of A:");
                    a = myScanner.nextInt();
                    pr("Input value of B:");
                    b = myScanner.nextInt();
                   
                    result = a<b?a:b;
                   
                   prln("\n\n *** Minimum number is "+ result+" ***");
                    
                    thankYou();
                    
                    break;
                    
                case 3:
                    int x, y, z, result3;
                    
                    pr("Input value of A:");
                    x = myScanner.nextInt();
                    pr("Input value of B:");
                    y = myScanner.nextInt();
                    pr("Input value of C:");
                    z = myScanner.nextInt();
                    
                   result3 = x<y?(x<z?x:z):(y<z?y:z);
                   
                  prln("\n\n *** Minimum number is "+ result3+" ***");
                    
                    thankYou();
                    
                    break;
                
                case 4:
                    int aa, bb, cc, dd, result4;
                    
                    pr("Input value of A:");
                    aa = myScanner.nextInt();
                    pr("Input value of B:");
                    bb = myScanner.nextInt();
                    pr("Input value of C:");
                    cc = myScanner.nextInt();
                    pr("Input value of D:");
                    dd = myScanner.nextInt();
                    
                    result4 = aa<bb?(aa<cc?(aa<dd?(aa):(dd) ):(cc) ) : (bb<cc?(bb<dd?(bb):(dd)):(cc));
                    
                   prln("\n\n *** Minimum number is "+ result4+" ***");
                    
                    thankYou();
                    
                    break;
                    
                case 5:
                     int aaa, bbb, ccc, ddd, eee, result5;
                    
                    pr("Input value of A:");
                    aaa = myScanner.nextInt();
                    pr("Input value of B:");
                    bbb = myScanner.nextInt();
                    pr("Input value of C:");
                    ccc = myScanner.nextInt();
                    pr("Input value of D:");
                    ddd = myScanner.nextInt();
                    pr("Input value of E:");
                    eee = myScanner.nextInt();
                    
                    //wrong  result5 = aaa<bbb?(aaa<ccc?(aaa<ddd?(aaa<eee?aaa:eee):(ddd<eee?ddd:eee) ):(ccc<ddd?(ccc<eee?(eee):(ddd)):(ddd)) ) : (bbb<ccc?(bbb<ddd?(bbb<eee?bbb:eee):(ddd<eee?ddd:eee)):(ccc<ddd?(ccc<eee?ccc:eee):(ddd)));
                    //currect
                       result5 = aaa<bbb?aaa<ccc?aaa<ddd?aaa<eee?aaa:eee:ddd<eee?ddd:eee:ccc<ddd?ccc<eee?ccc:eee:ddd<eee?ddd:eee:bbb<ccc?bbb<ddd?bbb<eee?bbb:eee:ddd<eee?ddd:eee:ccc<ddd?ccc<eee?ccc:eee:ddd<eee?ddd:eee;
                  
                   prln("\n\n *** Minimum number is "+ result5+" ***");
                    
                    thankYou();
                    
                    break;
                    
                default:
                    invalidInput();
            }
        }
        
        //for maximum
        else if(ans.toLowerCase().equals("maximum")){
             //User input:how many numbers compare 
            pr("How many numbers do you want to compare? <You can compare the maximum number of 5 numbers..> \nAnswer:");
            int compareBetween = myScanner.nextInt();
            switch(compareBetween){
                case 2:
                    int a, b, result;
                    pr("Input value of A:");
                    a = myScanner.nextInt();
                    pr("Input value of B:");
                    b = myScanner.nextInt();
                   
                    result = a>b?a:b;
                   
                   prln("\n\n *** Maximum number is "+ result+" ***");
                    
                    thankYou();
                    
                    break;
                    
                case 3:
                    int x, y, z, result3;
                    
                    pr("Input value of A:");
                    x = myScanner.nextInt();
                    pr("Input value of B:");
                    y = myScanner.nextInt();
                    pr("Input value of C:");
                    z = myScanner.nextInt();
                    
                   result3 = x>y?(x>z?x:z):(y>z?y:z);
                   
                  prln("\n\n *** Maximum number is "+ result3+" ***");
                    
                    thankYou();
                    
                    break;
                
                case 4:
                    int aa, bb, cc, dd, result4;
                    
                    pr("Input value of A:");
                    aa = myScanner.nextInt();
                    pr("Input value of B:");
                    bb = myScanner.nextInt();
                    pr("Input value of C:");
                    cc = myScanner.nextInt();
                    pr("Input value of D:");
                    dd = myScanner.nextInt();
                    
                    result4 = aa>bb?(aa>cc?(aa>dd?(aa):(dd) ):(cc) ) : (bb>cc?(bb>dd?(bb):(dd)):(cc));
                   
                    
                   prln("\n\n *** Maximum number is "+ result4+" ***");
                    
                    thankYou();
                    
                    break;
                    
                case 5:
                     int aaa, bbb, ccc, ddd, eee, result5;
                    
                    pr("Input value of A:");
                    aaa = myScanner.nextInt();
                    pr("Input value of B:");
                    bbb = myScanner.nextInt();
                    pr("Input value of C:");
                    ccc = myScanner.nextInt();
                    pr("Input value of D:");
                    ddd = myScanner.nextInt();
                    pr("Input value of E:");
                    eee = myScanner.nextInt();
                    
                    //wrong  result5 = aaa>bbb?(aaa>ccc?(aaa>ddd?(aaa>eee?aaa:eee):(ddd) ):(ccc>ddd?(ccc>eee?ccc:eee):(ddd)) ) : (bbb>ccc?(bbb>ddd?(bbb>eee?bbb:eee):(ddd)):(ccc));
                    //currect 
                     result5 = aaa>bbb?aaa>ccc?aaa>ddd?aaa>eee?aaa:eee:ddd>eee?ddd:eee:ccc>ddd?ccc>eee?ccc:eee:ddd>eee?ddd:eee:bbb>ccc?bbb>ddd?bbb>eee?bbb:eee:ddd>eee?ddd:eee:ccc>ddd?ccc>eee?ccc:eee:ddd>eee?ddd:eee;
                   prln("\n\n *** Maximum number is "+ result5+" ***");
                    
                    thankYou();
                    
                    break;
                    
                default:
                    invalidInput();
            }
        }
        
        //if user invalid input
        else{
           invalidInput();
        }
        
    }
       static void prln(Object anyobject){
    
        System.out.println(anyobject);
    }
        static void pr(Object anyobject){
            System.out.print(anyobject);
        }
        static void thankYou(){
             prln("\n\n--------------------------------------------------------");
            prln("Thank you for using my program.\n\n");
           
        }
        
        static void invalidInput(){
             prln("\n\n--------------------------------------------------------");
            prln("Invalid Input.\nIf you don`t give the right input,I can`t help you.\n\n");
        }
   
}
