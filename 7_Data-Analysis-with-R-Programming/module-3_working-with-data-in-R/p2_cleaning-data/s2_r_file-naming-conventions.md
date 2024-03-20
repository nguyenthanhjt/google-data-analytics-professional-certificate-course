# File-naming conventions

An important part of cleaning data is making sure that all of your files are accurately named. Although individual preferences will vary a bit, most analysts generally agree that file names should be accurate, consistent, and easy to read. This reading provides some general guidelines for you to follow when naming or renaming your data files. 

![A tall filing cabinet with one open drawer. Manila files are spread across the floor below.](./resources/img-1.png)

## What’s in a (file)name?

When you first start working with R (or any other programming language, analysis tool, or platform, for that matter), you or your company should establish naming conventions for your files. This helps ensure that anyone reviewing your analysis–yourself included–can quickly and easily find what they need. Next are some helpful “do’s” and “don’ts” to keep in mind when naming your files.

### Do

- Keep your filenames to a reasonable length
- Use underscores and hyphens for readability
- Start or end your filename with a letter or number
- Use a standard date format when applicable; example: YYYY-MM-DD
- Use filenames for related files that work well with default ordering; example: in chronological order, or logical order using numbers first

|**Examples of good filenames**  |
|--------------------------------|
| 2020-04-10_march-attendance.R  |
| 2021_03_20_new_customer_ids.csv|
| 01_data-sales.html             |
| 02_data-sales.html             |

### Don't

- Use unnecessary additional characters in filenames
- Use spaces or “illegal” characters; examples: &, %, #, <, or >
- Start or end your filename with a symbol
- Use incomplete or inconsistent date formats; example: M-D-YY
- Use filenames for related files that do not work well with default ordering; examples: a random system of numbers or date formats, or using letters first

| **Examples of filenames to avoid**      |
|-----------------------------------------|
|4102020marchattendance<workinprogress>.R |
|_20210320*newcustomeridsforfebonly.csv   |
|firstfile_for_datasales/1-25-2020.html   |
|secondfile_for_datasales/2-5-2020.html   |

## Additional resources

These resources include more info about some of the file naming standards discussed here, and provide additional insights into best practices.

- [How to name files](https://speakerdeck.com/jennybc/how-to-name-files): this resource from Speaker Deck is a playful take on file naming. It includes several slides with tips and examples for how to accurately name lots of different types of files. You will learn why filenames should be both machine readable and human readable.
- [File naming and structure](https://www.tikar.or.id/?q=node/205): this resource from the Princeton University Library provides an easy-to-scan list of best practices, considerations, and examples for developing file naming conventions.

## My Wrapped Keypoints

In this section, the focus is on establishing effective file-naming conventions for data files. Here's a summary of the key points covered:

1. **Importance of Naming Conventions:** Clear and consistent file names are essential for organizing and locating data files efficiently, especially when collaborating with others.

2. **Guidelines for File Naming:**
   - **Do:** Keep filenames concise, use underscores or hyphens for readability, start or end filenames with letters/numbers, employ standard date formats, and use filenames that facilitate logical ordering.
   - **Don't:** Include unnecessary characters, use spaces or special symbols, start or end filenames with symbols, employ inconsistent date formats, or use filenames that hinder logical ordering.

3. **Examples:** Clear examples of good and bad filenames are provided to illustrate the recommended practices and the pitfalls to avoid.

4. **Additional Resources:** Links to external resources are provided for further exploration of file naming standards and best practices, including tips on making filenames machine-readable and human-readable, and considerations for developing comprehensive file naming conventions.

By following these guidelines, analysts can ensure that their data files are accurately named, facilitating easy retrieval and enhancing overall data organization and management.
