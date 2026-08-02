# most straight-forward approach to solve a problem

# tries every possible valid solution util finds the one

## "I don't know the shortcut, so I'll check everything."

** **Real Life example** ** 
 *I have lost my key so I will inspect every possible place under bed, on table , under sofa, beside tv....*

   ### Example 1: Find Maximum Element [2,7,3,9]
    Brute force thinking:
    2= max compare with 7,
    7=max compare with 3,
    7=max compare with 9,
    9= maximum element.

## Interview Tip ⭐ Whenever the interviewer asks a problem:
>Don't immediately jump to the optimal solution.
Say something like:
"The simplest approach is to check every possibility. That would take O(n²). Then we can optimize it."
This demonstrates structured problem-solving. 
# Linear Search in an Integer Array (TC =O(n))
```

for(int i =0;i<arr.length-1;i++){
if(arr[i]==target){
System.out.println(arr[i]);
}

```
# Find the largest Element in an Array(TC=O(n))
```
int largest =arr[0];
for(int i =0;i<arr.length;i++){
if(arr[i]>largest){
largest =arr[i];
}
}
System.out.println(largest);
```
# Find Second Largest Element in an Array(TC =O(n))
```
int l1 = arr[0];
int l2 = Integer.MIN_VALUE;
for(int i =0;i<arr.length;i++){
if(arr[i]>l1){
l2 = l1;
l1=arr[i];

}
else if(arr[i]>l2 && arr[i]!=l1){
l2=arr[i];

}
}
System.out.println(l2);
```
# Check Array is sorted(TC=O(n))
```
boolean sorted = true;
for(int i =0;i<arr.length-1;i++){
  if(arr[i]>arr[i+1]){
    sorted = false;
}}
  if(sorted){
   System.out.println("sorted");
}
  else{
   System.out.println("Not sorted");}
```
# Two Sum(TC=)
```
for(int i =0;i<arr.length;i++){
  for(int j =i+1;j<arr.length;j++){
      if(arr[i]+ arr[j]==target){
      System.out.println(i +"" +j);
      }
}}
```