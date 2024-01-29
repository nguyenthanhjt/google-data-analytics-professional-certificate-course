# Step-by-Step: Filter data with SQL

This reading outlines the steps the instructor performs in the following video, [Filter data with SQL](https://www.coursera.org/learn/analyze-data/lecture/Y5Nmb/more-on-sorting-and-filtering). In the video, the instructor demonstrates filtering data with SQL using `WHERE` clauses.

Keep this step-by-step guide open as you watch the video. It can serve as a helpful reference tool if you need additional context or clarification while following the video steps. This is not a graded activity, but you can complete these steps to practice the skills demonstrated in the video.

## What you’ll need

If you’d like to follow along with the instructor, you will need to log in to your BigQuery account and upload the Movies dataset. To do this, follow the instructions in the reading [Upload the movie dataset to BigQuery](https://www.coursera.org/learn/analyze-data/supplement/sBFZn/optional-upload-the-movie-dataset-to-bigquery).

## Example 1: Filter data in SQL

Complete the following steps to use the `WHERE` clause to filter the database and narrow down the list to movies in the comedy genre.

1. In the BigQuery `Explorer` pane, select the `movie` dataset then the `movies` table.

2. Select the `Preview` tab from the `Details` pane.

3. Select **Query** then **In new tab** and enter the following code into the query editor:

    ```sql
    SELECT *
    FROM `projectID.movie_data.movies`
    ```

    **Note**: If you’re completing this code in BigQuery, replace `projectID` in the code block to your own projectID.
4. Use the `WHERE` clause to filter the data. Enter `WHERE Genre = 'Comedy';` to filter for and select rows with 'Comedy' in the Genre column.
5. Your code should now match this code block:

    ```sql
    SELECT *
    FROM `projectID.movie_data.movies`
    WHERE Genre = 'Comedy';
    ```

6. Select `RUN` to run the query. The results display a shorter list of movies, all in the comedy genre.
