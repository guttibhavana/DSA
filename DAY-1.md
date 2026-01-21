Missing Number:
```def missingNum(self, arr):
        su=0
        n=len(arr)+1
        for i in range(len(arr)):
            su+=arr[i]
        total=n*(n+1)//2
        return total-su
```
SecondLargest:
``` def getSecondLargest(self, arr):
        # Code Here
        if len(arr)<2:
            return -1
        maxn=sec=float('-inf')
        for num in arr:
            if num>maxn:
                sec=maxn
                maxn=num
            elif num>sec and num!=maxn:
                sec=num
        if sec==float('-inf'):
            return -1
        else:
            return sec
```
            
