# Amazon_Vine_Analysis

I was tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

## Resources

- Google Colab (PySpark)
- Jupyter Notebook
- AWS S3 and RDS
- PostgreSQL

## Results

### Deliverable 1

In Deliverable 1 we are tasked with extracting the dataset using google Colab with PySpark. I chose dataset: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Furniture_v1_00.tsv.gzCreated 

Multiple dataframes were created for the dataset.

A customer dataframe:

![image](https://user-images.githubusercontent.com/96445453/165021587-4c29bdd1-7522-4942-a1ff-88834b53fc51.png)

A product dataframe:

![image](https://user-images.githubusercontent.com/96445453/165021621-adc2a1a0-9b30-400a-a4b1-65cb78b52d13.png)

A review dataframe:

![image](https://user-images.githubusercontent.com/96445453/165021380-e23c5f99-5eb7-49bc-8f69-b41196a24ef1.png)

Lastly, a vine dataframe:

![image](https://user-images.githubusercontent.com/96445453/165021792-231af188-85c2-456e-a43d-da98acfde757.png)

Then loaded the dataframes to PostgreSQL and the AWS RDS created. I ran queries to check tables ran smooth.

![image](https://user-images.githubusercontent.com/96445453/165022007-87e73ced-aee9-4706-aa15-eeb34d674c5a.png)
![image](https://user-images.githubusercontent.com/96445453/165022047-7a004830-006d-47fd-b97a-68c3b298ae40.png)
![image](https://user-images.githubusercontent.com/96445453/165022081-12acda66-fa7c-4681-bf75-25b791374160.png)
![image](https://user-images.githubusercontent.com/96445453/165023558-4776c2bb-a926-4587-9127-993e47b46da3.png)

### Deliverable 2


- How many Vine reviews and non-Vine reviews were there?
  - Out of a total of 18138 reviews in this dataset, 136 were paid reviews (.75%) while 18002 were unpaid reviews (99.25%)  
![image](https://user-images.githubusercontent.com/96445453/165027145-01119288-6042-410c-a035-ee2ddc777a69.png)
![image](https://user-images.githubusercontent.com/96445453/165027178-67baf8da-51d7-410f-b4d9-d4df36a38f37.png)

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
  - There are 8546 total five star reviews.  A total of 74 are paid Vine reviews(.87%). 8472 were unpaid 5 star reviews (99.13%)

![image](https://user-images.githubusercontent.com/96445453/165028187-258eef18-12ad-4c6b-a462-21bec8579e62.png)
![image](https://user-images.githubusercontent.com/96445453/165028357-979ea255-3454-4220-b574-e3f0f9c7f315.png)

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
  - The paid Vine reviewers percentage of 5 star ratings was 54.41%. non-Vine reviews that were 5 stars had a total percentage of 52.94%.

![image](https://user-images.githubusercontent.com/96445453/165029341-28ec39f9-e528-4cf7-9421-e204c6e3f225.png)
![image](https://user-images.githubusercontent.com/96445453/165029288-e84561dc-77f6-43df-9ef4-5dced4318419.png)

## Summary

After extracting the data it looks like there is a near 50% chance a review will be 5stars. This might indicate that people either really love the products or simply dismiss a product review with a five star rating. There are a large amount of unpaid users compared to paid users or Vine vs non-Vine. The Vine vs non-Vine data shows a similar percentage of people that vote 5 star on reviews.

See Amazon_Reviews_ETL
See Vine_Review_Analysis

