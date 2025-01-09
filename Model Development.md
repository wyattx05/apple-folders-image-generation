# Model Progression & Development
Here is where I will show all the developments for FolderGenie and changes in new models and datasets. Currently the latest model trained is model 6 with STable Diffusion. This is also the first model actually posted to GitHub.

## Model 1 & 2

Model 1 generation:

I started this project by creating the dataset by using a base folder on my Mac and changing the color with the systems color picker then saving them all as PNGs. I also used the Icons8 website to gather different icons and a website that could generate more folder colors and icons on them.
Then after gathering all the images, I put the folder into VScode to easily make a text file for each image. This first dataset only had the images with no white background so when the model was being trained for this first tes, there was some errors and the results were not good. For the results for model 1 the black icons from the dataset won’t show on the training preview leading me to worry and the model wasnt working well. This was only a test training, so I wasn’t expecting the results to be good since it is only being trained for 100 iterations. 
I realized for the next model test each image of a folder and icon was going to need a white background behind it and I would have to edit the prompts to add it in.

Model 2 generation:

I put each image file through Adobe Illustrator to put a white background around it as well as adjusted the prompts of the folder images to clarify the white background behind it for the second model attempt.
For the results for model 2 all the icons and folders are visible behind a white background. Thie results from this model were not good also becuase I only trained it with only 100 training iterations again because it was only a test to ensure the dataset was looking good. But with the 3rd version of this model I am going to train it with 1500 training iterations where I will really start testing the results from these models.

## Model 3
This model was the first where I took the results generated seriously. I trained the model with 1500 iterations whih is the defult for stable diffusion. These results were not as bad as I expected it generated many different kinds of folders but still had some clear problems with putting icons on folders. For the next model since there are 26 images in the dataset I am going to train it 2600 times and then after that model depending on the results I will train that model again instead of retraining with the basic stable diffusion model. My hope is that this will make the model the best it can be.

## Model 4-4.1 & 5

Model 4 generation:

Resolution for data set: 512x512
Training Iterations: 2600
Model Size: 8
Time: Around 3 Hours

This model has the best results so far. Almost every time it generated a folder that could easily be used and it’s only problem was with adding icons on the folder. It did better than before but could only add an icon that was used for the two example images of a a triangle image on a folder in the dataset. My thought process here is that if I were to upload examples of all different icons on folders then it would better understand how to add those icons into any color folder. This is what I am going to do but I don’t know if I should go retrain model 4 or start over and make a model 5. I am going to try both. Right now, I am using prompts combining the training prompts from the dataset but in the future hope to get more complex with it.

Model 4.1 Generation:

Resolution for data set: 512x512
Training Iterations: 1300
Model Size: 8
Time: 1 hour

Before I completely retrain to make model 5 I wanted to train model 4 further with a new dataset I made of icons on a basic blue folder to see if it could improve it’s overall generation.
Results were not as good as I expected. It was actually worse than model 4 not so I edited the prompts of the folders with icons dataset and combinded them with model4 dataset to train the new model 5 dataset
When I would ask for the model to generate a purple color folder with a database icon it would produce 1 of three things, a blue folder with a purple icon, a blue folder, or a purple folder. I have more hope with model 5

Model 5 Generation:

Resolution for data set: 512x512
Training Iterations: 4200
Model Size: 8
Time: 

The results were not as good as I expected. The model still had the same trouble putting icons on folders and aftering testing a various different prompts I decided I needed to refine the pronpts in the training data to be more consistant. My plan is to scrap model five go into the latest dataset and make everyprompt unified. I only have three types of prompts, folers with icons prompts, folder colors prompts, and icon prompts. Once I go over the prompts in the dataset I will retrain to make model six at 4200 iterations again.

## Model 6
Resolution for data set: 512x512
Training Iterations: 4200
Model Size: 8
Time: 

The results of model 6 were a lot better and after fixing all the prompts in the data set I made prompt templates to use while genorating the folders. After using this model for a couple hours I realized it was good enough to publish on GitHub making it the first publicly avaible version. It still has some major bugs but has created some good folders so far. I plan to update with more iterations and give more detailed reports. I especially want to try other platforms that DiffusionBee.
