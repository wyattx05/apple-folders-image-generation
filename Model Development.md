# Model Progression & Development
Here is where I will show all the developments for FolderGenie and changes in new models and datasets. Currently the latest model trained is model 6 with STable Diffusion. This is also the first model actually posted to GitHub.

## Model 1 & 2

| ![bluecolorfolderonawhiteb_43957192 Background Removed](https://github.com/user-attachments/assets/ef1a6c74-645b-4e02-9ad7-c911094ed48d) | ![blackfoldercolorcompassic_54796498](https://github.com/user-attachments/assets/2909e151-9de2-43d8-8c1f-d293f90617ff) | ![icecolorfolder_28304545](https://github.com/user-attachments/assets/7aa4f266-cde1-47bf-aa6d-92a472dcd139) | ![folder_22663677](https://github.com/user-attachments/assets/ee5b94e6-1eb0-4f1e-ba54-ae82e6ca35c5) | ![tealcolorfolderonawhiteb_51554145](https://github.com/user-attachments/assets/384290bc-dda9-46f9-a0ac-cbb8b92d218d) | 
| ---------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |

### Model 1 generation:

I started this project by creating the dataset by using a base folder on my Mac and changing the color with the systems color picker then saving them all as PNGs. I also used the Icons8 website to gather different icons and a website that could generate more folder colors and icons on them.
Then after gathering all the images, I put the folder into VScode to easily make a text file for each image. This first dataset only had the images with no white background so when the model was being trained for this first tes, there was some errors and the results were not good. For the results for model 1 the black icons from the dataset won’t show on the training preview leading me to worry and the model wasnt working well. This was only a test training, so I wasn’t expecting the results to be good since it is only being trained for 100 iterations. 
I realized for the next model test each image of a folder and icon was going to need a white background behind it and I would have to edit the prompts to add it in.

### Model 2 generation:

I put each image file through Adobe Illustrator to put a white background around it as well as adjusted the prompts of the folder images to clarify the white background behind it for the second model attempt.
For the results for model 2 all the icons and folders are visible behind a white background. Thie results from this model were not good also becuase I only trained it with only 100 training iterations again because it was only a test to ensure the dataset was looking good. But with the 3rd version of this model I am going to train it with 1500 training iterations where I will really start testing the results from these models.

## Model 3

| ![bluecolorfolderwithanicon_28207089](https://github.com/user-attachments/assets/b7a567c9-a67e-45f7-909f-bda49e8ee3c4) | ![pinkcolorfolderwithanicon_89192924](https://github.com/user-attachments/assets/9de4b586-efd2-4037-af89-4ec4d300d4ed) | ![greencolorfolderwithanico_12357541](https://github.com/user-attachments/assets/09549c7c-2026-42f2-9596-f492c9142e83) | ![tealcolorfolderonawhiteb_51291364](https://github.com/user-attachments/assets/0471383f-567e-40a0-9a0f-5c666545ac31) | ![greencolorfolderonawhite_98275435](https://github.com/user-attachments/assets/bc61c46d-8df6-4e8e-a0a9-f259a63b8b5a) |
| ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |

This model was the first where I took the results generated seriously. I trained the model with 1500 iterations whih is the defult for stable diffusion. These results were not as bad as I expected it generated many different kinds of folders but still had some clear problems with putting icons on folders. For the next model since there are 26 images in the dataset I am going to train it 2600 times and then after that model depending on the results I will train that model again instead of retraining with the basic stable diffusion model. My hope is that this will make the model the best it can be.

## Model 4-4.1 & 5

| ![Blackcolorfolderonawhite_88810004](https://github.com/user-attachments/assets/c07b5fcc-aced-4949-9198-06624188846f) | ![Browncolorfolderwithanexa_62713662 Background Removed](https://github.com/user-attachments/assets/fe590d15-8473-44a1-a872-f7ac7ad75346) | ![pinkcolorfolderwithasmile_25127792](https://github.com/user-attachments/assets/372652a8-f938-4f44-9449-d51aecbd91a0) | ![greencolorfolderonawhite_13032951](https://github.com/user-attachments/assets/faa7c9bb-2489-43da-91f7-6825c5b33a16) | ![orangecolorfolderwithaloc_91029156 Background Removed](https://github.com/user-attachments/assets/92f54231-29d4-4fdc-b023-8e9508bdc492) | ![greencolorfolderwithacomp_59761842](https://github.com/user-attachments/assets/2d95a5d8-c352-4b79-a7c0-27aefbba9131) | ![purplecolorfolderwithaico_51220246](https://github.com/user-attachments/assets/85ce060b-a6e7-481a-9a45-974b2f33bc9e) |
| --------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
 
### Model 4 generation:

| Resolution for data set: 512x512 | Training Iterations: 2600 | Model Size: 8 | Time: Around 3 Hours |

This model has the best results so far. Almost every time it generated a folder that could easily be used and it’s only problem was with adding icons on the folder. It did better than before but could only add an icon that was used for the two example images of a a triangle image on a folder in the dataset. My thought process here is that if I were to upload examples of all different icons on folders then it would better understand how to add those icons into any color folder. This is what I am going to do but I don’t know if I should go retrain model 4 or start over and make a model 5. I am going to try both. Right now, I am using prompts combining the training prompts from the dataset but in the future hope to get more complex with it.

### Model 4.1 Generation:

Resolution for data set: 512x512 | Training Iterations: 1300 | Model Size: 8 | Time: 1 Hour |

Before I completely retrain to make model 5 I wanted to train model 4 further with a new dataset I made of icons on a basic blue folder to see if it could improve it’s overall generation.
Results were not as good as I expected. It was actually worse than model 4 not so I edited the prompts of the folders with icons dataset and combinded them with model4 dataset to train the new model 5 dataset
When I would ask for the model to generate a purple color folder with a database icon it would produce 1 of three things, a blue folder with a purple icon, a blue folder, or a purple folder. I have more hope with model 5

Model 5 Generation:

| Resolution for data set: 512x512 | Training Iterations: 4200 | Model Size: 8 | Time: 3-5 Hours |

The results were not as good as I expected. The model still had the same trouble putting icons on folders and aftering testing a various different prompts I decided I needed to refine the pronpts in the training data to be more consistant. My plan is to scrap model five go into the latest dataset and make everyprompt unified. I only have three types of prompts, folers with icons prompts, folder colors prompts, and icon prompts. Once I go over the prompts in the dataset I will retrain to make model six at 4200 iterations again.

## Model 6

| ![redcolorfolderonawhiteba_41700723 Background Removed](https://github.com/user-attachments/assets/30b1ebeb-fd85-4df9-8f7f-38b2e5d02f23) | ![orangecolorfolderonawhite_54862724 Background Removed](https://github.com/user-attachments/assets/866187f8-93b9-4247-90a6-ea9915f0f8b1) | ![pinkcolorfolderonawhiteb_4803479 Background Removed](https://github.com/user-attachments/assets/50902625-89d0-4555-a8f7-975352d54827) | ![purplecolorfolderonawhite_8427870 Background Removed](https://github.com/user-attachments/assets/5faa5ba9-ec54-41a6-a487-be9ce47699c9) | ![Yellowcolorfolderonawhite_90432293 Background Removed](https://github.com/user-attachments/assets/4131193b-7759-4aa1-a4e3-236709c0cbb3) | ![greencolorfolderonawhite_71597878 Background Removed](https://github.com/user-attachments/assets/30c4a6c2-28ef-4827-8343-aa40ddcab2f4) | ![bluesmile](https://github.com/user-attachments/assets/046446f0-ae78-4d06-9a6e-8e8548620df7) |
| ---------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------- |

| Resolution for data set: 512x512 | Training Iterations: 4200 | Model Size: 8 | Time: 3 - 5 Hours |

The results of model 6 were a lot better and after fixing all the prompts in the data set I made prompt templates to use while genorating the folders. After using this model for a couple hours I realized it was good enough to publish on GitHub making it the first publicly avaible version. It still has some major bugs but has created some good folders so far. I plan to update with more iterations and give more detailed reports. I especially want to try other platforms that DiffusionBee. Looking at the results above you can see the star isn't the same color as the folder and looks diffrent than the other folders. This has happened with a lot of generations and I kind of like this design too along with the translucent design. I could eventually build eough images to build a dataset to devide those designs instead of it being randmom. For now model 6 is good and it is time I give my computer a break on training. 

I started this project Sunday January 5th and made Model 6 on January 8th. 

## Model 6.1

| ![](https://github.com/user-attachments/assets/092a29d1-bbce-4f5c-a612-48390b88a9d6) | ![](https://github.com/user-attachments/assets/fe4e727a-87ed-4876-8b91-12f4bc59f759) | ![](https://github.com/user-attachments/assets/1ea2e337-2f39-426b-bf78-22e779d8d304) |  ![](https://github.com/user-attachments/assets/3a6a8d0b-0fa0-4c34-9f5e-bc79972d2896) | ![](https://github.com/user-attachments/assets/88ff2a11-7c4f-4807-abd7-65e4132f9751) | ![](https://github.com/user-attachments/assets/c42ae5a7-c451-46a5-9a2d-97932fd8ddfc) |
| ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------|

| Resolution for data set: 512x512 | Training Iterations: 4200 | Model Size: 8 |

Prompts used:

- purple color folder on a white background with an icon of a flower on it.
- ice color folder on a white background with an icon of a teardrop on it.
- orange color folder on a white background with an icon of a sun on it.
- pink color folder on a white background with an icon of a compass on it.
- red color folder on a white background with an icon of a apple on it.
- grey color folder on a white background with an icon of a mountain on it.



Model 6.1 results were very simillar to model 6. Over the use for a few days I saw small improvments in generation but then model 6 would out perform sometimes when I would compare them with the same prompts.
I hoped for better results but I just retraining on the same data wont imrpove much and adding more data would help more. There are also some inconsitecies in the dataset which make the model struggle to generate icons like books on folders.



