# Find your recipe
----------------
## Recommendation system project for cooking recipes 
![](/images/You-May-Also-Like.png.png)

Cooking is a hobby for some and a major problem for others. However, you can always use a helping hand for cooking. 
Being a mom of two, it is always a difficult decision to decide what to prepare for lunch or dinner. 
Sometimes faced with limited items in the kitchen, it is always a challenge to decide what to cook for meal. 
This inspired us to create a system that can recommend recipes based on ingredient suggestions. 

### Research Goal

Build recommendation system for people depend of their preference in the food.
Recommends new ingredients given user entered ingredients. 
This project is created in hopes to support homecooks in cooking quick and delicious meals. 
User will enter ingredients they have on hand, and the code will recommend the best meal based on that. 

### Dataset:

- Data for this project extracted from web-site food.com and Kaggle
- There are more than 150,000 recipes from more than 10  worlds cuisines
- All recipes contain information about ingredients, steps, time for preparation and etc.

### Methodology:

1. Download the dataset 
2. Check data set for missing/Nan/Null values
3. Create content-based recommendation:
    - Extract all recipe ingredients from recipe data
    - Obtain unique ingredient terms with corresponding quantities. Multiple ingredients as a single unit should be split into unit set ingredients. 
    For example, ingredients separated with ’and’/’or’/’instead’ are split into independent or separate ingredients. 
    Quantity associated with ingredients for the recipes are considered as the frequency of ingredient occurrence in the recipe. 
    - Construct inverted index with ingredients as terms and quantities as frequencies from all recipes. Common ingredients such as salt (to taste) are considered as a quantity of 1.
    
4. Test the data on the best model (highest recall score)


### Results:
 
![](images/result.png 'KNN results')


### Conclusion

In ideal situation users tells the recommender program what ingredients they have on hand and it given the best meal recipes. My recommendation system can give them only 75% of accuracy.


### Future Work
- Create an web-app or mobile app for my project
- Scribe more information from web about cooking and nutrition
- Try NLP - network for recipe ingredients
 
<pre>
Items in Repository:
- [/data] - folder
- *.ipynb - Jupyter Notebooks with all models
- [/images]() - all images
- [/py]() - additional user function
- [/presentation]() - pdf files of the final presentation
- README.md - a summary of the repository content
</pre>
