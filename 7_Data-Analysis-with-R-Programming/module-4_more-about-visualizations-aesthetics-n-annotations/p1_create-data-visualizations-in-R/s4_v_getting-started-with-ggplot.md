# Video: Getting started with ggplot()

## Question & Notes

- Geom (R): the geometric object used to represent the data
  - point: use point to create scatter plot
  - bar
  - line
  - more,....
- Aesthetic: a visual property of an object in your plot
- Mapping (R): matching up a specific variable in your dataset with a specific aesthetic

- Get help about geom_function: `? geom_[function-name]`

### Steps to create plot

1. Start with the ggplot function and choose a dataset to work with
2. Add a geom_ function to display your data:
   - geom_point()
   - geom_line()
3. Map the variable you want to plot in the arguments of the aes() function

Basic Syntax:

```r
library(ggplot2)

ggplot(data = <data>) + # choose data frame to work with
 GEOM_FUNCTION(
    mapping = # tell R what aesthetic to use for the plot
    aes(<AESTHETIC MAPPINGS>))

? geom_point
```

## Practice

```r
library(ggplot2)
library(palmerpenguins)

ggplot(data = penguins) + # choose data frame to work with
 geom_point(
    mapping = # tell R what aesthetic to use for the plot
    aes( # [name of aesthetic] = name of variable
        x = flipper_length_mm, y = body_mass_g))


ggplot(data = penguins) + # choose data frame to work with
  geom_point(
    mapping = # tell R what aesthetic to use for the plot
      aes( # [name of aesthetic] = name of variable
        x = bill_length_mm, y = bill_depth_mm))

? geom_point
```
