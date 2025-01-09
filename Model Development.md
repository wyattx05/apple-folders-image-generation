# Model Progression & Development
Here is where I will show all the developments for FolderGenie and changes in new models and datasets. Currently the latest model trained is model 6 with STable Diffusion. This is also the first model actually posted to GitHub.

## Model 1 & 2

Model 1 generation:
I created the dataset by using a base folder on my Mac and changing the color with the systems color picker then saving them all as PNGs. I also used the Icons8 website to gather different icons and a website that could generate more folder colors and icons on them. 
Then after gathering all the images, I put the folder into VScode to easily make a text file for each image. This first dataset only had the images with no white background so when the model was being trained there was some errors and I realized for the next model test each image of a folde and icon was going to need a white background.

Original Dataset made (with icon generated from dataset)
<img width="687" alt="Screenshot 2025-01-08 at 8 21 52 PM" src="https://github.com/user-attachments/assets/7e9caf49-4391-4c1c-9948-f7f63beb4721" />

For the results for model 1 the black icons from the dataset won’t show on the training preview leading me to worry and the model wasnt working well. This was only a test training, so I wasn’t expecting the results to be good since it is only being trained for 100 iterations. 
After trying the model out for a second I quickly moved on to working on the second version. 

Model 2 generation
I put each image file through Adobe Illustrator to put a white background around it as well as adjusted the prompts of the folder images to clarify the white background behind it for the second model attempt. I also did some work on the data set simplifying and unifying prompts.
For the results for model 2 all the icons and folders are visible behind a white background. Thie results from this model were not good also becuase I only trained it with only 100 training iterations again because it was only a test to ensure the dataset was looking good. But with the 3rd version of this model I am going to train it with 1500 training iterations where I will really start testing the results from these models.

## Model 3
This model was the first where I took the results generated seriously. These results were not as bad as I expected it generated many different kinds of folders but still had some clear problems with putting icons on folders. For the next model since there are 26 images I am going to train it 2600 times and then after that model depending on the results I will train that model again instead of retraining with the basic stable diffusion model. My hope is that this will make the model the best it can be.

## Model 4-4.1 & 5



## Model 6
