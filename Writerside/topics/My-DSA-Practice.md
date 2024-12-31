# My DSA Practice

<tabs>

<tab title="Java">

<chapter title="Table of Questions">
<table>
<tr>
<td>1</td>
<td>

[Segregate & Sort Even Odd Nums in-place](#ques1)

</td>
</tr>
</table>
</chapter>

<chapter id="ques1"  title="Question 1" level="2">

<tabs>

<tab title="Question">
<chapter title="Given an array arr, write a program segregating even and odd numbers. The program should put all even numbers first in sorted order, and then odd numbers in sorted order. Note:- You don't have to return the array, you have to modify it in-place." level="4">

<tldr>
<p>
Input: arr[] = [12, 34, 45, 9, 8, 90, 3] <br/>
 Output: [8, 12, 34, 90, 3, 9, 45] <br/>
 Explanation: Even numbers are 12, 34, 8 and 90. Rest are odd numbers.
<br/>
<br/>
Input: arr[] = [0, 1, 2, 3, 4] <br/>
Output: [0, 2, 4, 1, 3] <br/>
Explanation: 0 2 4 are even and 1 3 are odd numbers.
<br/>
<br/>
 Input: arr[] = [10, 22, 4, 6] <br/>
Output: [10, 22, 4, 6] <br/>
Explanation: Here all elements are even, so no need of segregataion
</p>
</tldr>

</chapter>
</tab>

<tab title="Explanation">

<chapter title = "I solved this question like this: " level="4"/>
<list>
<li>Filter  odd numbers in their array: oddArray</li>
<li>Filter even numbers in their array: evenArray</li>
<li>Sort both arrays</li>
<li>newArray ⇽  Combine evenArray & oddArray</li>
<li>originalArray ⇽ newArray</li>
</list>

</tab>
<tab title="Code">

```Java
import java.util.Arrays;

public class EvenOddSegregation {

    public static void main(String[] argv) {
        int[] arr = {6,5,4,3,2,1};
        EvenOddSegregation evenOddSegregation = new EvenOddSegregation();
        evenOddSegregation.segregateEvenOdd(arr);
        evenOddSegregation.printArray(arr);
    }


    void printArray(int[] arr){
        for(int elem : arr){
            System.out.print(elem + " ");
        }
    }


    public void segregateEvenOdd(int[] arr){
        int[] evenNums = Arrays.stream(arr).filter(number -> number % 2 == 0).toArray();
        int[] oddNums = Arrays.stream(arr).filter(number -> number % 2 != 0).toArray();
        Arrays.sort(evenNums);
        Arrays.sort(oddNums);
        System.arraycopy(evenNums, 0, arr, 0, evenNums.length);
        System.arraycopy(oddNums, 0, arr, evenNums.length, oddNums.length);
    }
}
```

</tab>
</tabs>

</chapter>

<chapter id="ques2"  title="Question 2" level="2">

<tabs>

<tab title="Question">
<chapter title="Given an array arr, write a program segregating even and odd numbers. The program should put all even numbers first in sorted order, and then odd numbers in sorted order. Note:- You don't have to return the array, you have to modify it in-place." level="4">

<tldr>
<p>
Input: arr[] = [12, 34, 45, 9, 8, 90, 3] <br/>
 Output: [8, 12, 34, 90, 3, 9, 45] <br/>
 Explanation: Even numbers are 12, 34, 8 and 90. Rest are odd numbers.
<br/>
<br/>
Input: arr[] = [0, 1, 2, 3, 4] <br/>
Output: [0, 2, 4, 1, 3] <br/>
Explanation: 0 2 4 are even and 1 3 are odd numbers.
<br/>
<br/>
 Input: arr[] = [10, 22, 4, 6] <br/>
Output: [10, 22, 4, 6] <br/>
Explanation: Here all elements are even, so no need of segregataion
</p>
</tldr>

</chapter>
</tab>

<tab title="Explanation">

<chapter title = "I solved this question like this: " level="4"/>
<list>
<li>Filter  odd numbers in their array: oddArray</li>
<li>Filter even numbers in their array: evenArray</li>
<li>Sort both arrays</li>
<li>newArray ⇽  Combine evenArray & oddArray</li>
<li>originalArray ⇽ newArray</li>
</list>

</tab>
<tab title="Code">

```Java
import java.util.Arrays;

public class EvenOddSegregation {

    public static void main(String[] argv) {
        int[] arr = {6,5,4,3,2,1};
        EvenOddSegregation evenOddSegregation = new EvenOddSegregation();
        evenOddSegregation.segregateEvenOdd(arr);
        evenOddSegregation.printArray(arr);
    }


    void printArray(int[] arr){
        for(int elem : arr){
            System.out.print(elem + " ");
        }
    }


    public void segregateEvenOdd(int[] arr){
        int[] evenNums = Arrays.stream(arr).filter(number -> number % 2 == 0).toArray();
        int[] oddNums = Arrays.stream(arr).filter(number -> number % 2 != 0).toArray();
        Arrays.sort(evenNums);
        Arrays.sort(oddNums);
        System.arraycopy(evenNums, 0, arr, 0, evenNums.length);
        System.arraycopy(oddNums, 0, arr, evenNums.length, oddNums.length);
    }
}
```

</tab>
</tabs>

</chapter>

</tab>

<tab title="C++">
Second tab content
</tab>

<tab title="Python">
Second tab content
</tab>



</tabs>