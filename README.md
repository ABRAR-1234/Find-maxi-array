# Find-maxi-array
package com.abr;

import java.util.Scanner;

public class Main {
    private static Scanner scanner = new Scanner(System.in);

    public static void main(String[] args) {
        int[] arr = getArray(5);
        int[] max = maximarray(arr);
        printarray(max);

    }
    private static int[] getArray(int number)
    {
        int[] array = new int[number];
        for(int i=0; i<array.length; i++)
        {
            array[i] = scanner.nextInt();
        }
        return array;
    }
    private static int[] maximarray(int[] array)
    {
        int[] max = new int[array.length];
        for(int i=0;i<maximarray.length;i++) {
            maximarray[i] = array[i];
        }
        boolean flag = true;
        int temp;
        while(true)
        {
            flag = false;
            if(maximarray[i]>maximarray[i+1]) {
                temp = maximarray[i];
                maximarray[i] = maximarray[i + 1];
                maximarray[i + 1] = temp;
                flag = true;
            }
        }
        return maximarray;
    }
    private static void printarray(int[] array)
    {
        for(int i=0; i<array.length; i++)
        {
            System.out.println("Element"+ i + array[i]);
        }
    }
}



