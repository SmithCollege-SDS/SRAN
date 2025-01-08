# SRAN: The *S*mith *R* *A*rchive *N*etwork

SRAN is an R package repository, similar to the well-known [CRAN](https://cran.r-project.org/web/packages/index.html) package repository. Its purpose is to provide a location for Smith College SDS faculty to distribute R packages. SRAN was created using [`{drat}`](https://github.com/eddelbuettel/drat/).

## Installing packages from SRAN

If you want to install a package from SRAN, first add SRAN to your list of R package repositories.

```r
options("repos" = c(options("repos"), "https://SmithCollege-SDS.github.io/SRAN/"))
```

Then, use the `install.packages()` function to install the packages you want. For example, you could install the [sds100](https://github.com/SmithCollege-SDS/sds100/) package by running the command:

```r
install.packages("sds100")
```

## Advantages of using SRAN to distribute your package

Because SRAN is a "proper" package repository, using SRAN to distribute your package has several advantages other methods of distributing packages.

1. Users can install SRAN packages using only "base" R functions
2. Packages installed from SRAN have an upgrade path
3. Authors of other packages (including yourself!) can easily depend on a package distributed from SRAN

Of course, you can achieve all of these features by submitting your package to CRAN as well, but this comes with stricter requirements and maintenance responsibilities that may not be worth it to take on.
