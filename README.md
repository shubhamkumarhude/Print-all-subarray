# Print-all-subarray
1. You are given an array of size 'n' and n elements of the same array. 2. You are required to find and print all the subarrays of the given array.  3. Each subarray should be space seperated and on a seperate lines. Refer to sample input and output



import java.io.*;
import java.util.*;

public class Main{

public static void main(String[] args) throws Exception {
    // write your code here
    Scanner scn = new Scanner(System.in);
    int n = scn.nextInt();
    
    int []arr= new int[n];
    for( int i = 0 ; i < arr.length; i++){
        arr[i]= scn.nextInt(); 
    }
    
    for( int i = 0 ; i <arr.length ; i++){
        for ( int j = i ; j < arr.length ; j++){
            for( int k = i ; k <=  j; k++ ){
                System.out.print(arr[k] + "\t");
            }
            System.out.println();
        }
    }
 }

}
