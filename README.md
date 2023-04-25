##min_max_sum
Given five positive integers, find the minimum and maximum values that can be calculated by summing exactly four of the five integers. Then print the respective minimum and maximum values as a single line of two space-separated long integers.

Example
arr=[1,3,5,7,9]
The minimum sum is 1+3+5+7=16  and the maximum sum is 3+5+7+9=24. The function prints

16 24
**
Solution is:  





int min=arr.get(0);
int max=arr.get(0);
long sum=0;
for(int i=0;i<arr.size();i++){
    if(arr.get(i)<min){
        min=arr.get(i);
    }
    else if(arr.get(i)>max){
        max=arr.get(i);
    }
}
for(int i=0;i<arr.size();i++){
   sum+=arr.get(i);
}
System.out.println((sum-max) + " " + (sum-min));
    
**
