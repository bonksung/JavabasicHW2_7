# JavabasicHW2_7
Help me yundo 
makeZero 메소드는 두 개의 배열 x와 y를 입력받는다. 그리고 배열 x에서 배열 y가 통째로 나오면 그 부분을 0 으로 바꾼다. 
main은 수정하지 말고 makeZero 메소드를 완성하여 결과가 나오도록 하시오.  


package homework2;
import java.util.Arrays;
public class HW2_20161178_7 {

static void makeZero(int[] x, int[] y) {
  for(int a = 0; a < x.length; a ++) {   
      if (x[a] == y[0]) {    
        int b = 1;
        while(b < y.length) {
          if(x[a+b] == y[b]) {     
            continue;     
            }     
          else      {break;}    
        if (b == y.length -1) {     
          while(a < a+y.length) {      
            x[a] = 0;     
          }    
        }       
          b+=1;     
        }   
      }  
    } 
  }  
  public static void main(String[] args) {   
    // TODO Auto-generated method stub   
    int[] a = {1, 2, 3, 4, 1, 2, 3, 4, 5};   
    int[] b = {2, 3, 4};   
    int[] c = {3, 3, 1, 3, 5, 3, 3, 3, 6, 7, 3, 3};   
    int[] d = {3, 3};   
    int[] e = {1, 2, 3, 1, 2, 3, 1, 1, 2, 3};   
    int[] f = {1};   
    int[] g = {1, 2, 3, 4, 5, 1, 2, 3, 4, 1, 2, 3, 4, 5, 1, 2, 3};   
    int[] h = {1, 2, 3, 4, 5};
    System.out.println("Original Array");   
    System.out.println("----------------------------------------");   
    System.out.println("a : " + Arrays.toString(a));   
    System.out.println("b : " + Arrays.toString(b));   
    System.out.println("c : " + Arrays.toString(c));   
    System.out.println("d : " + Arrays.toString(d));   
    System.out.println("e : " + Arrays.toString(e));   
    System.out.println("f : " + Arrays.toString(f));   
    System.out.println("g : " + Arrays.toString(g));   
    System.out.println("h : " + Arrays.toString(h));
    makeZero(a, b);   
    makeZero(c, d);   
    makeZero(e, f);   
    makeZero(g, h);
    System.out.println("\n\nAfter make zero");   
    System.out.println("----------------------------------------");   
    System.out.println("a : " + Arrays.toString(a));   
    System.out.println("b : " + Arrays.toString(b));   
    System.out.println("c : " + Arrays.toString(c));   
    System.out.println("d : " + Arrays.toString(d));   
    System.out.println("e : " + Arrays.toString(e));   
    System.out.println("f : " + Arrays.toString(f));   
    System.out.println("g : " + Arrays.toString(g));   
    System.out.println("h : " + Arrays.toString(h));  
    } 
   }
