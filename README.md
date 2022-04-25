# Amazon_Vine_Analysis

I was tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

## Resources

- Google Colab (PySpark)
- Jupyter Notebook
- AWS S3 and RDS
- PostgreSQL

## Results

### Deliverable 1

In Deliverable 1 we are tasked with extrating the dataset using google Colab with PySpark. I chose dataset: https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Furniture_v1_00.tsv.gzCreated 

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
- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?
- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?
