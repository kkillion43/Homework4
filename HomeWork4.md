# HomeWork4
Kyle Killion  
May 30, 2016  
### Get the bootStrap from another Normal Sample but from Size 50

```r
x <- rnorm(50,22,5)
bootMean <- numeric(1000)

for ( i in 1:1000){
  
  bootSamp <- sample(x, size=1000, replace=TRUE)
  bootMean[i] <- mean(bootSamp)
}
hist(bootMean)
```

![](HomeWork4_files/figure-html/unnamed-chunk-1-1.png)<!-- -->

```r
print(quantile(bootMean, c(.025, .975)))
```

```
##     2.5%    97.5% 
## 22.05215 22.75068
```


### Get the bootStrap from another Normal Sample but from Size 80

```r
y <- rnorm(80, 22, 5)
bootMean2 <- numeric(1000)

for (i in 1:1000){
  
  bootSamp2 <- sample(y, 1000, replace = TRUE)
  bootMean2[i] <- mean(bootSamp2)
}
hist(bootMean2)
```

![](HomeWork4_files/figure-html/unnamed-chunk-2-1.png)<!-- -->

```r
print(quantile(bootMean2, c(.025, .975)))
```

```
##     2.5%    97.5% 
## 21.79104 22.37327
```

### Get the bootStrap from another Exponential Sample but from Size 50

```r
x <- rexp(50, 1)
bootMean3 <- numeric(1000)

for ( i in 1:1000){
  
  bootSamp3 <- sample(x, size=1000, replace=TRUE)
  bootMean3[i] <- mean(bootSamp3)
}
hist(bootMean3)
```

![](HomeWork4_files/figure-html/unnamed-chunk-3-1.png)<!-- -->

```r
print(quantile(bootMean3, c(.025, .975)))
```

```
##      2.5%     97.5% 
## 0.8248007 0.9210847
```

### Get the bootStrap from another Exponential Sample but from Size 80

```r
x <- rexp(80,1)
bootMean4 <- numeric(1000)

for ( i in 1:1000){
  
  bootSamp4 <- sample(x, size=1000, replace=TRUE)
  bootMean4[i] <- mean(bootSamp4)
}
hist(bootMean4)
```

![](HomeWork4_files/figure-html/unnamed-chunk-4-1.png)<!-- -->

```r
print(quantile(bootMean, c(.025, .975)))
```

```
##     2.5%    97.5% 
## 22.05215 22.75068
```


