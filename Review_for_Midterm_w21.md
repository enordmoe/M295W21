Midterm Exam Review
================
Introduction to Data Science
E. Nordmoe

  - [3 Data Visualization](#data-visualization)
  - [5 Data Transformation](#data-transformation)
  - [Types of Questions](#types-of-questions)

# 3 Data Visualization

Every **ggplot2** plot has three key components:

1.  data,
2.  A set of aesthetic mappings between variables in the data and visual
    properties, and
3.  At least one layer which describes how to render each observation.
    Layers are usually created with a geom function.

Here’s a simple example:

``` r
ggplot(mpg, aes(x = displ, y = hwy)) + 
  geom_point()
```

1.  Be familiar with the following geoms and their typical aesthetic
    specifications:

<!-- end list -->

  - `geom_bar()`  
  - `geom_boxplot()`  
  - `geom_col()`  
  - `geom_density()`  
  - `geom_freqpoly()`  
  - `geom_histogram()`  
  - `geom_jitter()`  
  - `geom_line()`
  - `geom_point()`  
  - `geom_smooth()`

<!-- end list -->

2.  Common aesthetics and their relationship to type of variable
    (categorical vs quantitative/continuous) :

<!-- end list -->

  - `x` and `y`  
  - `color` and `fill`  
  - `size`, `shape`, and `linetype`

<!-- end list -->

3.  Scales and how they can be used and specified manually

4.  Stats and their connections to geoms, especially for categorical
    variable plots like `geom_bar()`.

5.  Position adjustments and their relationship to geoms

6.  Faceting methods and their purposes

7.  Use of `coord_flip()` and `coord_cartesian()` to control the
    appearance of plots.

8.  Practice on the end of section questions in R4DS. I have a link to
    R4DS solutions near the top of the Moodle page but [it’s also
    here](https://moodle.kzoo.edu/mod/url/view.php?id=199818). These
    solutions also have some very valuable insights and extensions to
    the text material.

# 5 Data Transformation

1.  Be familiar with the different types of variables in R.

2.  Know the purpose and syntax of the five key **dplyr** functions:  

<!-- end list -->

  - `filter()`  
  - `arrange()`  
  - `select()`  
  - `mutate()`  
  - `summarise()`

<!-- end list -->

3.  Be able to describe the role of `group_by()` to change the scope of
    each function from operating on the entire dataset to operating on
    it group-by-group.

4.  Know how missing values work and how to use the `is.na()` function
    to include or remove cases with NA values.

5.  Be familiar with “helper” functions for `select()` and
    `summarise()`. These need not be memorized since you have them on
    the cheat sheets.

6.  Other commands from this section you should know about and be able
    to use when necessary:

<!-- end list -->

  - `distinct()`  
  - `count()`  
  - `slice()`  
  - `pull()`  
  - `top_n()`

# Types of Questions

1.  Multiple choice: Which code chunk yields this output?  
2.  What does this code do?
3.  Find the error and fix it.  
4.  What goes in the missing spot in the code chunk?  
5.  Write a small code chunk to create the given output.
