#Food Classification and Nutrition Fact extact

**Introduction**

Basically, we want to train an food image classifier to recongnize different food and extract the nutrition fact of the food, based on the result we will provide the recommendation and score. 

**Backgroud **

Food plays an important part in our life. With the improvement of life quality and people's healthy awareness increasing, more and more people start pursuing healthy food and healthy eating behavior. How to help people easily transfer to a healthy eating behavior? How to make the tracking process more convenient? Food classification is the crucial point to solve this problem. So we want to build the deep learning model to recognize the food image and provide nutrition fact based on the result. 

**Technical Detail**

***Data Set***:

We will use the Food-101 Data Set for trainning food image classifier. This data set contain 101 food categories, with 101000 images. For each food categories, there are 250 test images and 750 training images. The training data are not cleaned, there is still some noise data. The noise data are some with intense colors and some with incorrect labels. All images were rescaled to have a maximum side length of 512 pixels. 

*Data Citation: Bossard, Lukas and Guillaumin, Matthieu and Van Gool, Luc, Food-101 – Mining Discriminative Components with Random Forests, European Conference on Computer Vision, 2014*

For the food nutrition fact, we will crawl the data from nutritionvalue.org. The data contain nutritional value for common food and products. All the nutrition fact are based on serving size of 100g. 

***Enviornment Requirement***: 

We will use the fastai to train the model and deploy the model a mobile app built by React Native. 

fastai: version 1.0.42

PyTorch: version 1.0.0

React Native: version 0.58.6

***Design***:

*<u>Food Image Classification</u>*:

1. Retrieve and store the data
2. Read the image:
   - Specifies the path where the images are located
   - Assigan training/ validation rate to 80/20
   - Set image size
   - Normalizes the images
3. We will build a deep learning mode to train the data
4. Evaluate the training result and do more training.
5. Deploy to the mobile app. We will try to deploy the deep learning model with mobile app using Expo

<u>*Nutrition Fact extract*</u>:

1. Crawl the data from nutritionalvalue.org website
2. Profile and clean the data 
3. Set score for different food nutrition fact composition
4. Match the nutrition fact with the result of food classification
5. Provide score accordingly

***Hypothesis***:

Based on Food 101 dataset we expect to reach accuracy around 95% and retrieve the nutrition fact with accuracy around 98%. Deploy to mobile is a big challenge since we will use PyTorch rather than TensorFlow. We will figure out how to use Expo to get the model run on mobile app. 

