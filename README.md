# Assignment_3-Find_Index-

import java.util.Scanner;

public class Main{

    static int returnIndex(int[] arr, int target){

        int n = arr.length;
        int ans = 0;
        for(int i=0; i<n; i++){
                if(arr[i]  >= target){
                    ans++;



                }
            }



        return ans;

    }
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the array size");
        int n = sc.nextInt();
        int[] arr = new int[n];

        System.out.println("Enter " + n + " elements");
        for(int i = 0; i < n; i++){
            arr[i] = sc.nextInt();
        }

        System.out.println("Enter target sum ");
        int target = sc.nextInt();
        System.out.println(returnIndex(arr, target));
    }

}
