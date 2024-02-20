# Electronic Products Rating and Recommendations
  
  Please see the [Tableau Dashboard](https://public.tableau.com/app/profile/sotiria.ntinou/viz/ElectronicProductsRating/Dashboard1)

## Table of Contents

* [Problem Statement](#problem-statement)
* [Data Sourcing](#data-sourcing)
* [Data Presentation](#data-presentation)
* [Data Analysis](#data-analysis)
* [Insights](#insights)
* [Recommendations](#recommendations)

- - - -

### Problem Statement

The purpose of this analysis is to provide information that come from Electronics Products Rating and Recommendation Data 
about online buyers' preferences and satisfaction.

About:
* Rating levels and Recommendation Status
* Review Frequency and Rating over Time
* Helpful Reviews
* Product's Rating
* Color preferences
* Brand and Categories of Products Rating


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

    
   ![alt text](https://github.com/RoulaNtinou/ElectronicProductsRecommendations-Tableau/blob/e2e8856ec1615a005fb8cc8a8d3a8f3e81784ecd/QuarterlyReviewRating.png)

  > There are a few key observations regarding customer engagement and satisfaction with products, particularly in 2018:
  >
  > - **Decrease in Reviews** : There is a significant decrease in the number of reviews in 2018 compared to previous years, representing a decrease in customer engagement with the 
  > products.
  > - **High Satisfaction Levels** : Despite the decrease in engagement, the majority of customers who left reviews in 2018 (approximately 90%) rated the products highly, with ratings 
  > of 4 or 5.
  > - **Low Dissatisfaction Levels** : Conversely, a very small percentage of customers (below 10%) who left reviews in 2018 gave low ratings of 1 or 2, indicating low levels of 
  > dissatisfaction with the products.
 
    





3.  **Helpful reviews and Rating**
   
   ![alt text](https://github.com/RoulaNtinou/ElectronicProductsRecommendations-Tableau/blob/a35f88d78db92ec673af3b6eb0eda146f90b9498/HelpfulReviewPorRating.png)

> It appears that there is a correlation between the rating given by customers and the likelihood of their reviews being voted as helpful.
> 
>  Here's a breakdown of the percentages of helpful votes for reviews of different ratings:
> 
> **Rating 5**: Approximately 68% of helpful votes were cast for reviews with a rating of 5. This indicates that a significant portion of customers find reviews with the highest rating to be helpful when making purchasing decisions.
> 
> **Rating 4**: Around 17% of helpful votes were cast for reviews with a rating of 4. While slightly lower than for rating 5 reviews, this still suggests that positive reviews with a slightly lower rating are also considered helpful by customers.
> 
> **Rating 3**: Only 4% of helpful votes were cast for reviews with a rating of 3. This suggests that reviews with a moderate rating may be less influential in terms of receiving helpful votes compared to higher-rated reviews.
> 
> **Ratings 2 and 1**: Approximately 6% of helpful votes were cast for reviews with ratings of 2 or 1. This indicates that reviews with lower ratings are less likely to be perceived as helpful by customers, possibly due to the negative sentiment associated with these ratings.

   



4. **Top 15 products(based on the number of reviews) and their rating**.
   
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
     Choose a brand to see detailed information. 

    ![alt text](https://github.com/RoulaNtinou/ElectronicProductsRecommendations-Tableau/blob/4bb9130e7c52cd5f2aa2679aeca325d5c0a69f59/CategoriesperBrandRecommendations.png)

   > - **Top Brands Have Categories with Negative Recommendations**:
   >   Among the top five brands sorted by the number of reviews, each brand has at least one category of products with negative 
   >   recommendations exceeding 10% of the total recommendations. This indicates that even popular brands may have certain product 
   >   categories that receive more negative feedback from customers.
   >                                                                                                                                 
   > - **Rest of the Brands Have Mostly Positive Recommendations**:
   >   Conversely, the rest of the brands (those not in the top five) have all their product categories with positive recommendations 
   >   exceeding 90% of the total recommendations. This suggests that these brands generally maintain high levels of customer > 
   >   satisfaction across all their product categories.
   
- - - -
   
### Insights

 #### <ins>Reviews Over Time</ins>
 
* One factor worth mentioning that could contribute to the significant increase in reviews since 2013 is:
  **The Rise of Online Shopping and Review Culture**: The increasing trend in online shopping and the prevalence of review platforms may 
  have encouraged more customers to leave reviews as part of their purchasing decision-making process.

* These observations suggest that while there has been **a decline in customer engagement with the products in 2018**, the overall 
  satisfaction levels among the customers who did engage remained high

#### <ins>Rating-Recommendations-Helpful Reviews</ins>

* **Satisfied customers are highly likely to endorse the product**, while dissatisfied customers are unlikely to do so. Understanding and addressing the factors driving customer satisfaction can therefore have a significant impact on improving recommendations and overall customer loyalty.
  

*  **The importance of positive reviews**, particularly those with higher ratings, in influencing customer perceptions and receiving helpful votes from other shoppers, and finally in increasing sales.

#### <ins>The more the Reviews the wider the range of opinions</ins>  
*  Products with a larger number of reviews may also attract a wider range of opinions, including more negative feedback. On the other hand, products with fewer reviews may have a more skewed distribution towards positive ratings.

  - - - -

  ###Recommendations

  * Engage with Customers and encourage them to leave reviews even by offering incentives.

  * Promote Positive Reviews: Showcase positive reviews and testimonials to build trust and credibility with potential customers. 
    Highlighting the positive experiences of satisfied customers can help influence purchasing decisions and attract new customers.

  * Use customer feedback as a valuable source of insights to continuously improve product quality and enhance the overall customer 
    experience.

