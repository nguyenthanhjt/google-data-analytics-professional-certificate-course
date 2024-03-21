# R

## Syntax

- Call a column of a Data frame: [data-frame-name]$[column-name]

## R common function

### Inspect - Review data set information

- `str()`:
- `glimpse()`:
- `colnames()`:
- `head()`: view first 6 rows of data

### Data Manipulation function

- `separate()`: `separate(dataset, column-name, into=c('new-col-1','new-col-2',..), sep = 'separator-character')`: split data in a column into some others columns
- `unit()`: allow to merge/combine columns together
- `mutate()`: modify the data set by add/.. columns
- `group_by()`: group data by columns
  - `group_by(column-1-name, column-2-name,...)`
- `mean()`: calculate average of a columns
  - `mean(column-name)` 
- `sd()`: calculate the Deviation compare to average value of a column
- `cor(x, y))`: calculate the correlation between 2 columns' value
- `bias(actual, predicted)`: bias computes the average amount by which actual is greater than predicted.
  - actual: The ground truth numeric vector.
  - predicted: The predicted numeric vector, where each element in the vector is a prediction for the corresponding element in actual.
  - If a model is unbiased bias(actual, predicted) should be close to zero. Bias is calculated by taking the average of (actual - predicted).
- `sample()`: function allows you to take a random sample of elements from a data set. 
- `arrange(data-set, desc(column-name))`: sort `asc(column-name)`, `desc(column-name`) by input column-name