# nosql-Challenge

The UK Food Standards Agency evaluates various establishments across the United Kingdom, and gives them a food hygiene rating. I will evaluate some of the ratings data in order to help journalists and food critics decide where to focus future articles. This challenge will be divided into three parts.

---

## Part 1: Database and Jupyter Notebook Set Up

1. Use "NoSQL_setup_starter.ipynb" for this section of the challenge.

2. Import the data provided in the "establishments.json" file from the Terminal. Name the database "uk_food" and the collection establishments. Copy the text used to import the data from the Terminal to a markdown cell in the notebook.

3. Within the notebook, import the libraries PyMongo and Pretty Print (pprint).

4. Create an instance of the Mongo Client.

5. Confirm that I created the database and loaded the data properly:

-List the databases I have in MongoDB. Confirm that "uk_food" is listed.
-List the collection(s) in the database to ensure that establishments is there.
-Find and display one document in the establishments collection using "find_one" and display with pprint.

6. Assign the establishments collection to a variable to prepare the collection for use.

---

## Part 2: Update the Database

1. Use "NoSQL_setup_starter.ipynb" for this section of the challenge.

2. Find the BusinessTypeID for "Restaurant/Cafe/Canteen" and return only the "BusinessTypeID" and "BusinessType fields".

3 Update the new restaurant with the "BusinessTypeID" I found.

4. Remove any establishments within the "Dover Local Authority" from the database, and check the number of documents to ensure they were deleted.

5. Use "update_many" to convert latitude and longitude to decimal numbers.
   
6. Use "update_many" to convert "RatingValue" to integer numbers.

---

## Part 3: Exploratory Analysis

I will use the following questions to explore the database, and find answers, that can help journalists and food critics make a chocie:

- Which establishments have a hygiene score equal to 20?

- Which establishments in London have a RatingValue greater than or equal to 4?

- What are the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?

- How many establishments in each Local Authority area have a hygiene score of 0? Sorting the results from highest to lowest, and print out the top ten local authority areas.

 

> [!NOTE]
> Could should be working without errors. The Starter Code was provide by edX Boot Camps LLC. The code was written by David Arjuna with the assist of Xpert Learning.
> References: [UK Food Standards Agency](https://www.food.gov.uk/) (2022). [UK food hygiene rating data API](https://ratings.food.gov.uk/open-data/en-GB). Contains public sector information licensed under the [Open Government Licence v3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/). Accessed Sept 9, 2022 and Sept 12, 2022 with the establishment settings as follows: longitude=51.5072, latitude=-0.1276, maxdistancelimit=4567, pagesize=10000, sortoptionkey=distance, pagenumber=(1,2,3,4,5,6,7,8).
