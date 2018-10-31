Activity7-Lab7
================
Taehoon Ha
10/31/2018

-   [Question 1.](#question-1.)
-   [Question 2.](#question-2.)

### Question 1.

Re-format the code according to the style guide.

``` r
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

``` r
prime = function(n) { 
    if(n%%1!=0 | n<0) { 
        return (FALSE)
    } else if (n==1) {
        return (FALSE)
    } else if (n==2) {
        return (TRUE)
    } else {
        for(i in 2:(sqrt(n))) {
            if(n %% i == 0) {
                return (FALSE)
            }
        } 
    return (TRUE)
    }
}
```

### Question 2.

Re-format and debug the function `find_runs` that finds consecutive ones in a given vector.

``` r
find_runs <- function(x, k) {
   n <- length(x)
   runs <- NULL
   for (i in 1:(n-k+1)) {
       if (all(x[i:(i+k-1)] == 1)) runs <- c(runs, i)
    }
   return(runs)
}

find_runs(c(1,0,0,1,1,0,1,1,1), 2)
```

    ## [1] 4 7 8
