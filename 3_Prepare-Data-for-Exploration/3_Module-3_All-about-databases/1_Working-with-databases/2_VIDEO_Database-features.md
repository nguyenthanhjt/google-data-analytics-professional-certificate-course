# Database features

[VIDEO](./resources/2_VIDEO_Database-features.mp4) and [transcript](./resources/2_VIDEO_Database-features.txt)

Databases are essential tools for data analysts. I use them constantly. Just about all of the data I access is stored within databases. Databases store and organize data, making it much easier for data analysts to manage and access information. They help us get insights faster, make data-driven decisions, and solve problems. You've already heard a bit about what databases are and how they're used by data analysts. Now let's learn more about database features and components. Here's a simple database structure. It contains tables with information from a car manufacturer. The top level includes car dealerships, product details, and repair parts. Then if you drill down to the next level by selecting one of those tables, you'll find more specific details about each item. This is called a relational database. A relational database is a database that contains a series of related tables that can be connected via their relationships. For two tables to have a relationship, one or more of the same fields must exist inside both tables. For example, here, branch ID exists in this table and this one. If a field exists within both tables, we can use it to connect the tables together. The branch ID field is the key to connecting these tables. There are two types of keys. A primary key is an identifier that references a column in which each value is unique. You can think of it as a unique identifier for each row in a table. For our dealership table with information about the different dealership branches, branch ID is the primary key. Similarly, for the product details table about each car, VIN is our primary key. As an analyst you may need to create tables. If you do decide to include a primary key, it should be unique, meaning no two rows can have the same primary key. Also, it cannot be null or blank. There are also foreign keys. A foreign key is a field within a table that's a primary key in another table. In other words, a foreign key is how one table can be connected to another. Because our repair parts table contains information about each car part, the primary key is part ID. Each row in our repair parts table represents one unique part. All the other keys in this table, such as the VIN, are the foreign keys that allow the repair parts table to be connected to the other tables. As you can see, a table can only have one primary key but it can have multiple foreign keys. Understanding primary and foreign keys can be tricky, so you'll have more opportunities to practice coming up. But as a general summary, a primary key is used to ensure data in a specific column is unique. It uniquely identifies a record in a relational database table. Only one primary key is allowed in a table and they cannot contain null or blank values. And a foreign key is a column or group of columns in a relational database table that provides a link between the data and two tables. It refers to the field in a table that's the primary key of another table. Lastly, it's important to note that more than one foreign key is allowed to exist in a table. Feel free to rewatch this video to be sure you understand primary and foreign keys clearly. And coming up, you'll begin practicing how to access and analyze data from actual databases. That will be a great opportunity to improve your understanding of primary and foreign keys, database organization and how you might use databases in your future analytics career.

## Question

- If you create a database table and include a primary key in the table, what must you ensure? Select all that apply.
  - The primary key has a numeric value
  - `The primary key is unique`
  - The primary key isn't a foreign key in another table
  - `The primary key's value isn't null or blank`

> If you create a database table with a primary key, it must be unique and its value must not be null or blank.

- A table in a relational database can have only one foreign key.

- True
- `False`

> A table in a relational database is allowed to have multiple foreign keys.

## Keypoints

- Importance of Databases for Data Analysts:
  - Databases are essential tools for data analysts, facilitating the storage, organization, and access of data.
  - They play a crucial role in enabling faster insights, data-driven decisions, and problem-solving.
- Overview of Database Structure:
  - Introduces a simple database structure with tables containing information from a car manufacturer.
  - The structure includes top-level categories like car dealerships, product details, and repair parts.
- Relational Database Concept:
  - Defines a relational database as a database containing related tables connected via relationships.
  - Relationships are established by having one or more fields in common between tables.
- Primary and Foreign Keys:
  - Explains primary keys as unique identifiers for each row in a table, ensuring uniqueness and non-null values.
  - Introduces foreign keys as fields within a table, acting as primary keys in another table to establish connections.
- Creating Tables and Primary Keys:
  - Advises data analysts on creating tables, emphasizing the uniqueness and non-null nature of primary keys.
  - Uses examples like branch ID for dealership tables and VIN for product details.
- Understanding Foreign Keys:
  - Describes foreign keys as links between tables, with examples like part ID in a repair parts table connecting to other tables.
  - Emphasizes that a table can have multiple foreign keys but only one primary key.
- Practice Opportunities:
  - Highlights upcoming practice opportunities to reinforce understanding of primary and foreign keys, database organization, and usage.
  - Encourages reviewing the video for clarity on primary and foreign keys.
