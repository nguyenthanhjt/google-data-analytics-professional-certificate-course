# Saving images without ggsave()

![Image](./resources/img-3.png)

In most cases, `ggsave()` is the simplest way to save your plot. But there are situations when it might be best to save your plot by writing it directly to a graphics device. This reading will cover some of the different ways you can save images and plots without `ggsave()`, and includes additional resources to check out if you want to learn more. 

A graphics device allows a plot to appear on your computer. Examples include:

- A window on your computer (screen device)
- A PDF, PNG, or JPEG file (file device)
- An SVG, or scalable vector graphics file (file device)

When you make a plot in R, it has to be “sent” to a specific graphics device. To save images without using `ggsave()`, you can open an R graphics device like `png()` or `pdf()`; these will allow you to save your plot as a .png or .pdf file. You can also choose to print the plot and then close the device using `dev.off()`.

## Example of using `png()`

```R
png(file = "exampleplot.png", bg = "transparent")
plot(1:10)
rect(1, 5, 3, 7, col = "white")
dev.off()
```

## Example of using `pdf()`

```R
pdf(file = "/Users/username/Desktop/example.pdf",    
       width = 4,     
       height = 4) 
plot(x = 1:10,     
        y = 1:10)
abline(v = 0)
text(x = 0, y = 1, labels = "Random text")
dev.off()
```

## Resources

To learn more about the different processes for saving images, check out these resources:

- [**Saving images without ggsave()**](https://ggplot2.tidyverse.org/reference/ggsave.html#saving-images-without-ggsave-): This resource is pulled directly from the ggplot2 documentation at [tidyverse.org](https://www.tidyverse.org/). It explores the tools you can use to save images in R, and includes several examples to follow along with and learn how to save images in your own R workspace.

- [**How to save a ggplot**](https://www.datanovia.com/en/blog/how-to-save-a-ggplot/): This resource covers multiple different methods for saving ggplots. It also includes copyable code with explanations about how each function is being used so that you can better understand each step in the process.  

- [**Saving a plot in R**](https://www.datamentor.io/r-programming/saving-plot/):  - This guide covers multiple file formats that you can use to save your plots in R. Each section includes an example with an actual plot that you can copy and use for practice in your own R workspace.
