# varXvar  (goodness of fit)

Calculate and Visualize Variable by Variable (varXvar) Goodness of Fit in R

```r
m = matrix()

# decompose matrix
pca <- prcomp(t(m), scale = T, center = T)

# recomose the matrix  
M = (t(pca$x[] %*% t(pca$rotation[])) * pca$scale  + pca$center)

# recompose matrix using only < n > compoents
n = 2 
M_approx = (t(pca$x[,1:n] %*% t(pca$rotation[,1:n])) * pca$scale  + pca$center)

```
