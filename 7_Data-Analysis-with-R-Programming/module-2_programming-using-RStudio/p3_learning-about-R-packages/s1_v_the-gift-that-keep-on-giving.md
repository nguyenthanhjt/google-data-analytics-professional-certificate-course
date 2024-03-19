# Video: The gift that keeps on giving

Video transcript

- Hello, there.
- I have to say getting a package delivered to you is one of life's simple pleasures.
- It doesn't matter if it's a surprise package or something you ordered yourself.
- It's exciting to open your package to discover what's inside.
- No wonder those unboxing videos on Youtube are so popular.
- Well, R has a different kind of package that our R users can open.
- These packages are units of reproducible R code and they make it easier to keep track of code.
- They're created by members of the R community to keep track of the R functions that they write and reuse.
- These community members might then make the packages available to other users.
- It's one of the great things about being part of this community.
- Packages in R include reusable R functions and documentation about the functions including how to use them.
- They also contain sample datasets and tests for checking your code to make sure it does what you want it to do.
- By default, R includes a set of packages called base R that are available to use in RStudio when you start your first programming session.
- There's also recommended packages that are loaded but not installed.
- Before using functions from one of these packages, you'd have to load it with a library command like library boot, for example.
- Let's find out which packages we already have in RStudio.
- We'll work in our console instead of a script for now because we're practicing and don't need to save this code for later.
- To check out our packages, we'll just run the command installed.
-packages and there's our list.
- Let's focus on the package and priority columns.
- The package column gives the name of the package, like cluster or graphics.
- The priority column tells us what's needed to use functions from the package.
- If you come across the word base in the priority column, then the package is already installed and loaded.
- You can use all of the functions of that package as soon as you open RStudio.
- If you find the word recommended, then the package is installed but not loaded.
- You'll also notice a list of packages in the bottom right part of our workspace.
- This list includes a brief description of each package.
- To load class and other uninstalled packages, we'll need to use the library function followed by the name of the package.
- Now, the class package has a check next to it, so it's been successfully loaded for use.
- If you want to learn even more about your loaded packages, you can click on their names in the Packages tab.
- This opens the Help tab and shows topics related to the package you selected.
- You can also use the Help function in your programming to call up the Help tab.
- While the pre-installed packages give you tons of useful functions, there's even more packages that will further expand your programming abilities.
- You can find thousands of R packages just by doing an online search.
- One of the most commonly used sources of packages is CRAN.
- CRAN stands for comprehensive R archive network.
- It's an online archive with R packages, source code, manuals, and documentation.
- When you start working with R, you'll be able to do your own searches to find packages in CRAN or elsewhere.
- It's almost always easier to just search with your favorite search engine though.
- So packages are a pretty big part of using R.
- They give you most of what you need to complete your programming throughout the data analysis process.
- Who knows? You might even turn your own code into packages for others to use.
- Up next, we'll keep unpacking R packages.
- See you soon.

## Question & Notes

- **Packages (R)**: Units of reproducible code (R)
- **Packages in clude**:
  - Reusable R fuctions
  - Documentation about the functions
  - Sample datasets
  - Tests for checking your code
- **CRAN**: Comprehensive R Archive Network - An online archive with R  packages, source code, manuals, and documentation

### Question 1: Fill in the blank: Packages in R include _____. Select all that apply

- [ ] visualizations
- [x] sample datasets
- [x] reusable R functions
- [x] tests for checking your code

> Packages in R include reusable R functions, documentation about how to use the functions, sample datasets, and tests for checking your code.

## Keypoint from **Section 1: The gift that keeps on giving**

- **Content Summary**: This section introduces the concept of R packages, comparing them to the excitement of receiving a package delivery. R packages are described as units of reproducible R code containing functions, documentation, datasets, and tests. The video explains the presence of default packages (base R) and recommended packages in RStudio, and demonstrates how to check and load packages using the `installed.packages()` and `library()` functions, respectively. It also mentions CRAN as a major source for R packages.

- **Key Points**:
  1. R packages are units of reproducible R code created by the community.
  2. They contain functions, documentation, datasets, and tests.
  3. Base R packages are pre-installed and automatically available.
  4. Recommended packages are installed but not loaded by default.
  5. The `library()` function is used to load packages.
  6. CRAN is a major repository for R packages.
