# 8_Class_Barnyard_Animal_Image_Classifier

Project Purpose:
In this scenario the ABC Feed Company has requested a feature that can suggest feed products to a customer when they upload a photo of their animal to ABC’s website.  
ABC produces and supplies feed products for eight types of animals: cats, dogs, chickens, cows, goats/sheep, horses, pigs, and rabbits.  
In response to this request, I have developed a deep learning CNN fine-tuned from the popular MobileNet model that can predict which of the 8 classes of animal a photo depicts with an accuracy of %94.25 across a test set of 400 images. 
I have added the functionality to predict on a single image and this continues to function at a high rate of accuracy on images never before seen by the model. 
ABC’s website management team will integrate this feature functionality into their website design.

The IDE and libraries used to develop the final solution were:
•	Development Environment: 
o	JupyterLab 3.4.4
	
•		Language and library versions:
o	Anaconda 3
o	Python 3.9.13
o	Numpy 1.21.5
o	TensorFlow 2.11.0
o	Keras 2.11.0
o	Scikit-learn 1.0.2
o	IPython 7.31.1
o	Matplotlib 3.5.2

Descriptions of files in this repo...

•	Models
o	This folder contains the save file for my fully trained model, which achieved %99.54 training accuracy, %93.75 validation accuracy, and %94.25 prediction accuracy on a set of 400 test images.

•	BarnyardAnimalClassifierForTraining.ipynb
o	This file contains all the building, training, validation, and testing code for the model and multiple graphics including plots of loss and accuracy during training as well as sample images and a confusion matrix of the test set predictions. 
Each block of code is commented for clarity as to its functionality.   

•	BarnyardAnimalClassifierForDemo.ipynb
o	This file is a stripped-down version of the BarnyardAnimalClassifierForTraining.ipynb file with the model building and training sections removed.  
It is ideal for a demonstration of functionality as it loads the saved model without showing all the build data.  
The functionality allows for demos of the test phase with accompanying confusion matrix and the ability to upload an image for single prediction. 
Each block of code is commented for clarity as to its functionality.     

•	BarnyardAnimalClassifierForABCWebTeam.ipynb
o	This file is what would be submitted to ABC Feed Supply as a deliverable.  
It only contains the necessary functionality of loading the trained model, displaying an image, and making a prediction on that image. 
Each block of code is commented for clarity as to its functionality.   

•	FileManipulation.ipynb
o	This file contains the functions used for cleaning our dataset, renaming all files to our naming convention, and splitting out and populating the valid, test, and train folders.  
Each block of code is commented for clarity as to its functionality.   

Things to note...

I was not able to upload the original training, validation, and test image datasets to github as they are too large and numerous.  
I have uploaded two sample photos from each class in the 'verification' folder for use in verifying functionality of the single prediction functionality.  

There are a few places in the notebook where a filepath is used.  These are references to the location on my machine.  When running on a different machine these locations will need to be edited.

The accompanying Word document is a 30-page, 6000-word assignment including a businesss proposal aspect and goes into greater detail as to the extent of the project.  
