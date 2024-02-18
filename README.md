# Electronic Products Rating and Recommendations

## Table of Contents

* [Problem Statement](#problem-statement)
* [Data Sourcing](#data-sourcing)
* [Data Presentation](#data-presentation)
* [Data Analysis](#data-analysis)
* [Insights](#insights)

- - - -

### Problem Statement

The purpose of this analysis is to provide information that come from Electronics Products Rating and Recommendation Data 
about online buyers' preferences and satisfaction.

About:
* Rating levels and Recommendation Status
* Review Frequency and Rating over Time
* Helpful Reviews
* Product's Rating
* Brand and Categories of Products Rating
* Color preferences

- - - -


### Data Sourcing

The Dataset used for this analysis comes from [Onyx Data](https://onyxdata.co.uk/data-dna-dataset-challenge/) and are available in the file above.

- - - -

### Data Presentation
The Dataset has 21 columns, with 7,299 entries and 7238 reviews.
The reviews were collected from Sep 2007 until May 2018. But since 2013 they increased significantly.

| Columns              | Entries            | 
| ----------------     |:-----------------  |
| id                   | 7299 non-null      |
| brand                | 7299 non-null      |
| colors               | 5280 non-null      |
| categories           | 7299 non-null      |
| dateAdded            | 7299 non-null      |
| dateUpdated          | 7299 non-null      |
| dimension            | 6090 non-null      |
| manufacturer         | 4632 non-null      |
| manufacturerNumber   | 7299 non-null      |
| name                 | 7299 non-null      |
| reviews.date         | 7238 non-null      |
| reviews.dateSeen     | 7299 non-null      |
| reviews.doRecommend  | 5908 non-null      |
| reviews.numHelpful   | 5813 non-null      |
| reviews.rating       | 7135 non-null      |
| reviews.text         | 7294 non-null      |
| reviews.title        | 7295 non-null      |
| reviews.username     | 7299 non-null      |
| sourceURLs           | 7299 non-null      |
| upc                  | 7299 non-null      |
| weight               | 7299 non-null      |
 
 
Data Cleaning was done already.

- - - -

### Data Analysis


1. **Relationship between product ratings and recommendation status**.
   See the following graph.

   ![alt text](https://github.com/RoulaNtinou/ElectronicProductsRecommendations-Tableau/blob/0ed57382bea835e78425e1e254db6011e5db4d9e/RatingRecommendations.png)

  > There is a strong relationship between the rating given by customers and their likelihood to recommend the product.                                                         
  > Here's a breakdown of the relationship:
  >
  >
  > - **Satisfied Customers (Rating 4 or 5)**:
  > Almost 98% of satisfied customers, who rated the product highly with a 4 or 5, are likely to recommend it. This indicates a high level of satisfaction and endorsement for the 
  > product.
  >
  > - **Dissatisfied Customers (Rating 1 or 2)**:
  > Conversely, almost 98% of dissatisfied customers, who rated the product poorly with a 1 or 2, are unlikely to recommend it. This suggests a strong negative sentiment towards the 
  > product among dissatisfied customers.
  >
  > - **Neutral or Mixed Feelings (Rating 3)**:
  > Among customers who have neutral or mixed feelings about the product, approximately 40% of them still recommend it, while 60% do not. This indicates a less decisive recommendation 
  > behavior among customers with moderate satisfaction levels.





 2. **Review frequency and rating over time**.
   See the following graph.

   ![alt text](https://github.com/RoulaNtinou/ElectronicProductsRecommendations-Tableau/blob/e2e8856ec1615a005fb8cc8a8d3a8f3e81784ecd/QuarterlyReviewRating.png)


  > - **Decrease in Reviews** : There is a significant decrease in the number of reviews in 2018 compared to previous years, representing a decrease in customer engagement with the 
  > products.
  > - **High Satisfaction Levels** : Despite the decrease in engagement, the majority of customers who left reviews in 2018 (approximately 90%) rated the products highly, with ratings 
  > of 4 or 5.
  > - **Low Dissatisfaction Levels** : Conversely, a very small percentage of customers (below 10%) who left reviews in 2018 gave low ratings of 1 or 2, indicating low levels of 
  > dissatisfaction with the products.
 
    





3.  It appears that there is a correlation between the **rating given by customers and the likelihood of their reviews being voted as helpful**.
    Here's a breakdown of the percentages of helpful votes for reviews of different ratings:

   ![alt text](https://github.com/RoulaNtinou/ElectronicProductsRecommendations-Tableau/blob/a35f88d78db92ec673af3b6eb0eda146f90b9498/HelpfulReviewPorRating.png)
   

    
    > - **Rating 5** : Approximately 68% of helpful votes were cast for reviews with a rating of 5. This indicates that a significant portion of customers 
    >   find reviews with the highest rating to be helpful when making purchasing decisions.
    >
    > - **Rating 4** : Around 17% of helpful votes were cast for reviews with a rating of 4. While slightly lower than for rating 5 reviews, this still                           
    >   suggests that positive reviews with a slightly lower rating are also considered helpful by customers.
    > 
    > - **Rating 3** : Only 4% of helpful votes were cast for reviews with a rating of 3. This suggests that reviews with a moderate rating may be less                        
    >   influential in terms of receiving helpful votes compared to higher-rated reviews.
    >
    > - **Ratings 2 and 1**: Approximately 6% of helpful votes were cast for reviews with ratings of 2 or 1. This indicates that reviews with lower ratings                            
    >   are less likely to be perceived as helpful by customers, possibly due to the negative sentiment associated with these ratings.



4. **Products' Rating**, sorting the products with the most reviews, what we have here are **the 15 top products(based on the number of reviews)**.
   
    ![alt text](https://github.com/RoulaNtinou/ElectronicProductsRecommendations-Tableau/blob/f9b809a36769b952d153d9636f8f317ad09d6f0b/ProductsAndRating.png)


  > - **Products with Most Reviews** (e.g., Logitech Remote Control):
  >   This product has a significant number of reviews, but a relatively higher proportion of negative ratings (ratings 1 and 2), with 16% combined.
  >   Positive ratings (ratings 4 and 5) still form the majority but are comparatively lower at 73%.
  >
  > - **Products with Fewer Reviews** (e.g., Sanus Wall Mount):
  >   These products have fewer reviews but tend to have a higher proportion of positive ratings and a lower proportion of negative ratings.
  >   For example, the Sanus Wall Mount has a combined 3% for ratings 1 and 2, while ratings 4 and 5 make up 90% of the total ratings.


5. **Colors Popularity**, sorting the products colors according to reviewer's preferences.
   See the following graph.

    ![alt text](https://github.com/RoulaNtinou/ElectronicProductsRecommendations-Tableau/blob/6564be45a73de12ad3b268e74519a65c283db4f6/Colors.png)

   > It seems that black is the most preferred color among reviewers, followed by variations such as black and white, black grey red blue, multicolor, and blue.
   > Here's a summary of the proportions:
   > 
   > - **Black** : Approximately 68% of the products are black, indicating a strong preference for this color among reviewers.
   > 
   > - **Black and White** : Around 11.21% of the products are black and white, suggesting a significant but relatively smaller preference for this combination.
   > 
   > - **Black Grey Red Blue**: Similarly, approximately 11.14% of the products feature a combination of black, grey, red, and blue, indicating a preference for multicolored options 
   >   with black as a dominant color.
   >
   > - **Multicolor**: About 5% of the products are multicolored, suggesting a preference for diverse color options among a smaller portion of reviewers.
   > 
   > - **Blue**: Finally, approximately 4.5% of the products are blue, indicating a lesser but still notable preference for this color.


6. **Brands per Categories of products with Recommendations**

    ![alt text](https://github.com/RoulaNtinou/ElectronicProductsRecommendations-Tableau/blob/4bb9130e7c52cd5f2aa2679aeca325d5c0a69f59/CategoriesperBrandRecommendations.png)

   

   
   

   













   









































### Insights
