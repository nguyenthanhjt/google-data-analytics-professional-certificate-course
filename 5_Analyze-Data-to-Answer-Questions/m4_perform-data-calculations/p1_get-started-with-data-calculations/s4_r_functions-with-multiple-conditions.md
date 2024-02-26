# Reading: Functions with Multiple Conditions

As you’ve been learning, conditional functions and formulas perform calculations according to specific conditions. In addition, functions including `SUMIF` and `COUNTIF` only work in cases where there is one condition. However, if you have more than one condition, you would need to use the `SUMIFS` or the `COUNTIFS` function instead. These functions enable you to perform calculations if you have two or more conditions. In this reading, you will learn more about conditional functions and how to construct functions with multiple conditions by exploring their basic syntax and checking out an example. You will also be able to access resources for similar functions in Excel.

## SUMIF to SUMIFS

Previously, you learned that the `SUMIF` function adds values in a particular range based on a single condition. The basic syntax is `=SUMIF(range, criterion, sum_range)`.

The first range is where the function will search for the condition that you have set. The criterion is the condition you are applying and the sum_range is the range of cells that will be included in the calculation. For example, in an accounting spreadsheet, you could use `SUMIF` to calculate the total expenses for a specific category, like Travel expenses, within a given month.

Or, you could find the total sales for automotive fuel treatment products– in this table, the ProductA is high octane fuel and ProductB is standard octane. Table 1 includes columns for Product, Region, Quarter, and Sales.

**Example Spreadsheet:**

| Product  | Region | Quarter | Sales |
| -------  | ------ | ------- | ----- |
| ProductA | East   | Q1      | 100   |
| ProductB | West   | Q2      | 150   |
| ProductA | East   | Q3      | 120   |
| ...      | ...    | ...     | ...   |

You could use `SUMIF` to calculate the total sales for Product A using a formula like this:

```excel
=SUMIF(A2:A8, "ProductA", D2:D8)
```

But, you could also build in multiple conditions by using the `SUMIFS` function. `SUMIF` and `SUMIFS` are very similar: They add up values in a range. But `SUMIFS` can include multiple conditions. This gives you more control over your summing criteria, which, in turn, allows you to perform more complex data analysis easily.

The basic syntax is: `=SUMIFS(sum_range, criteria_range1, criterion1, [criteria_range2, criterion2, ...])`

The square brackets let you know that this is optional. The ellipsis at the end of the statement enables as many repetitions of these parameters as needed. For example, if you wanted to calculate the sum of sales for ProductA in the East district in the first quarter, you could create a `SUMIFS` statement with multiple conditions, like this:

```excel
=SUMIFS(D2:D8, A2:A8, "ProductA", B2:B8, "East", C2:C8, "Q1")
```

In this example, `B2:B8` is the second criterion_range and "East" is the second condition. The third criterion_range is `C2:C8` and the third condition is "Q1". As long as you follow the basic syntax, you can add up to 127 conditions to a `SUMIFS` statement!

## COUNTIF to COUNTIFS

Just like the `SUMIFS` function, `COUNTIFS` allows you to create a `COUNTIF` function with multiple conditions. The definition for `COUNTIF` is a function that counts the number of cells in a range that meet a single condition. For example, using `COUNTIF` to track the number of days a temporary employee was absent in an attendance record.

The basic syntax is: `=COUNTIF(range, criterion)`

Just like `SUMIF`, you set the range and then the condition that needs to be met. For example, in Table 1, if you wanted to count the number of transactions for ProductA, you could use a `COUNTIF` function like this:

```excel
=COUNTIF(A2:A8, "ProductA")
```

`COUNTIFS` has the same basic syntax as `SUMIFS`: `=COUNTIFS(criteria_range1, criterion1, [criteria_range2, criterion2, ...])`

The criteria_range and criterion are in the same order, and you can add more conditions to the end of the function. So, if you wanted to find the number of sales transactions for ProductA in the East region in the first quarter, you could use `COUNTIFS` to apply those conditions, like this:

```excel
=COUNTIFS(A2:A8, "ProductA", B2:B8, "East", C2:C8, "Q2")
```

This enables you to find every instance where both of conditions (East and Q1) are true.

## For More Information

`SUMIFS` and `COUNTIFS` are just two examples of functions with multiple conditions. They help demonstrate how multiple conditions can be built into the basic syntax of a function. There are other functions with multiple conditions that you can use in your data analysis and many resources available online to help you get started:

- [How to use the Excel IFS function](https://exceljet.net/excel-functions/excel-ifs-function): This includes an explanation and example of the `IFS` function in Excel. It’s a great reference if you’re interested in learning more about IFS. The example is a useful way to understand this function and how it can be used.

- [VLOOKUP in Excel with multiple criteria](https://exceljet.net/formula/vlookup-with-multiple-criteria): Similar to the previous resource, this resource goes into more detail about how to use `VLOOKUP` with multiple criteria. Being able to apply `VLOOKUP` with multiple criteria will be a useful skill, so check out this resource for more guidance on how you can start using it on your spreadsheet data.

- [INDEX and MATCH in Excel with multiple criteria](https://excelchamps.com/excel-formulas/index-match-multiple-criteria/): This resource explains how to use the `INDEX` and `MATCH` functions with multiple criteria. It also includes an example, which demonstrates how these functions work with multiple criteria and actual data.

- [Using IF with AND, OR, and NOT functions in Excel](https://support.microsoft.com/en-us/office/using-if-with-and-or-and-not-functions-d895f58c-b36c-419e-b1f2-5c193a236d97): This resource combines `IF` with `AND`, `OR`, and `NOT` functions to create more complex functions. By combining these functions, you can perform your tasks more efficiently and cover more criteria at once.