# App-Rating-Prediction
Analysis & Perdicting app rating using Python.

# Description
## Objective:
Make a model to predict the app rating, with other information about the app provided.
## Problem Statement:
Google Play Store team is about to launch a new feature wherein, certain apps that are promising, are boosted in visibility. The boost will manifest in multiple ways including higher priority in recommendations sections (“Similar apps”, “You might also like”, “New and updated games”). These will also get a boost in search results visibility.  This feature will help bring more attention to newer apps that have the potential.
## Fields in the data:
<ol>
  <li>App: Application name</li>
  <li>Category: Category to which the app belongs</li>
  <li>Rating: Overall user rating of the app</li>
  <li>Reviews: Number of user reviews for the app</li>
  <li>Size: Size of the app</li>
  <li>Installs: Number of user downloads/installs for the app</li>
  <li>Type: Paid or Free</li>
  <li>Price: Price of the app</li>
  <li>Content Rating: Age group the app is targeted at – Children / Mature 21+ / Adult</li>
  <li>Genres: An app can belong to multiple genres (apart from its main category). For example, a musical family game will belong to Music, Game, Family genres.</li>
  <li>Last Updated: Date when the app was last updated on Play Store</li>
  <li>Current Ver: Current version of the app available on Play Store</li>
  <li>Android Ver: Minimum required Android version</li>

  <li>Load the data file using pandas</li>
  <li>Check for null values in the data and get the number of null values for each column</li>
  <li>Drop records with nulls in any of the columns</li>

  <li>Fix incorrect data types and inconsistent formatting:
    <ol>
      <li>Convert Size column (Kb/Mb) to numeric format</li>
      <li>Extract the numeric value from the Size column</li>
      <li>Multiply the value by 1,000 if size is mentioned in Mb</li>
      <li>Convert Reviews column to numeric (int/float)</li>
      <li>Clean Installs column by removing ‘+’ and ‘,’ and convert to integer</li>
      <li>Remove ‘$’ from Price column and convert it to numeric</li>
    </ol>
  </li>

  <li>Perform sanity checks:
    <ol>
      <li>Ensure Rating is between 1 and 5; drop rows outside this range</li>
      <li>Ensure Reviews are not more than Installs; drop invalid rows</li>
      <li>For Free apps, ensure Price is not greater than 0; drop invalid rows</li>
    </ol>
  </li>

  <li>Perform univariate analysis</li>
  <li>Perform outlier treatment</li>
  <li>Perform bivariate analysis</li>
  <li>Perform data preprocessing</li>

  <li>Split the data into train and test sets using 70-30 split and name them df_train and df_test</li>
  <li>Separate into X_train, y_train, X_test, and y_test</li>

  <li>Build a Linear Regression model</li>
  <li>Report the R² score on the training set</li>
  <li>Make predictions on the test set and report the R² score</li>
</ol>
