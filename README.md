# Lab8
Biostatistics1 - Lab8

### Question 1. 
Read Chapter 21 from "Advanced R" 2nd ed., H. Wickham.

### Question 2.
Complete Problem 1 and Problem 2 from Activity 8 and submit your code to a GitHub repository.

#### (1) Re-format the code according to the style guide.

```{r}
prime=function(n){ 
if(n%%1!=0 | n<0){ 
return (FALSE)
}else if(n==1){
    return (FALSE)
}else if(n==2){
    return (TRUE)
    }else {
        for(i in 2:(sqrt(n))){
        if(n %% i==0){
        return (FALSE)
}
}
    return (TRUE)
}
}
```

#### (2) Re-format and debug the function `find_runs` that finds consecutive ones in a given vector.

### Question 3.
Please debug the following function that should return a sorted vector in ascending order. For example, if the input for your function is the vector (3, 1, 2), then your function should return the vector (1, 2, 3). Please submit your code to the GitHub repository.
