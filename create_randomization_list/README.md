Frequently clinical trials intend to compare the differences between two treatment types. Different treatments need to 
assigned to study patients randomly. The following R code snipped shows how a simple randomization list of 100 unique 
"Verum" and 100 unique "Placebo" entries can be generated.

``` r
# set seed to ensure reproducibility
set.seed(1337)
# sample 100 unique four digit ids
id <- sample(x=c(1000:2000), size=200, replace=F)

# set seed o ensure reproducibility
set.seed(1337)
# generate shuffled list of
# "Placebo" (n=100) and
# "Verum" (n=100)
drug <- sample(x=c(rep(x="Verum", times=100), rep(x="Placebo", times=100)), size=200, replace=F)
 
# merge the ids and the drugs
randomization_list <- data.frame(cbind(id, drug))
```

The list created from this snippet is saved here as reference.
