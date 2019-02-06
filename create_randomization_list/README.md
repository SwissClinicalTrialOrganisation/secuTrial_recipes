Frequently clinical trials intend to compare the differences between two treatment types. Different treatments need to 
assigned to study patients randomly. The following R code snipped shows how a simple randomization list of 100 unique 
"Verum" and 100 unique "Placebo" entries can be generated.

``` r
# set seed to ensure reproducibility
set.seed(1337)
# sample 100 unique four digit ids
id <- sample(x=c(1000:2000), size=200, replace=FALSE)

# set seed o ensure reproducibility
set.seed(1337)
# generate shuffled list of
# "Placebo" (n=100) and
# "Verum" (n=100)
drug <- sample(x=c(rep(x="Verum", times=100), rep(x="Placebo", times=100)), size=200, replace=FALSE)
 
# merge the ids and the drugs
randomization_list <- data.frame(cbind(id, drug))

# save the table
write.csv(x=randomization_list, file="randomization_list.csv", row.names=FALSE)

```

The list created from this snippet with the seed "1337" is saved here as reference.
