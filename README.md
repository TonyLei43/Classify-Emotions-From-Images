# Classify-Emotions-From-Images

**Description**: This was a resaerch project for a professsor who wanted to classify the emotions in an image using machine learning to better undertstand the emotional landscape of social conflicts. 

## Pipeline
1. Given a csv of images and data, I downloaded the images for every row using the `url` column
2. Using the Py-Feat API library, process and extract the FexData for each image for storage in subfolders
3. Once the FexData has been extracted, I can use PyFeat's methods to generate predictions for the faces in the image
4. Create a data frame using Pandas that includes the image ID and the emotions of each face in the image
5. Join the pre-existing csv in step 1 to the dataframe in step 4 to create a joint dataframe with information about the image and the emotion of each face
6. Save combined dataframe to google drive storage

## Learning Outcomes
- Learned how to effectively use the PyFeat Library for emotion detection
- Used the OS library to create folders/subfolders and checking for existing files
- Learned how to batch data for preprocessing and merging data afterwards

## Challenges
- Since the csv being processed varied in size (100MB-10GB+), I had to figure out an effective way of processing the data
- A lot of trial and error since the code would stop and break halfway through, which meant I needed to write code for redundant images/processed images
- Working with a new library that I never used before meant that I had to research and play around with the code and read the documentation before applying it to the project

## Technologies Used
- Python
- Google Colab
- PyFeat
- OS
- Pandas
