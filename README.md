# Major_project
Mounting Google Drive and Extracting Data: The notebook starts by mounting your Google Drive to access files and then extracts a zip file containing image and mask data.
Loading and Preprocessing Images: It then loads the images and corresponding masks, sorts them, and resizes them to 512x512 pixels.
Data Augmentation: The code applies data augmentation (horizontal flip and brightness/contrast adjustment) to increase the size of the training dataset.
Building the U-Net Model: A 2D U-Net model is defined using the Keras API for image segmentation. There was also a 3D U-Net model definition, but the 2D model was the one compiled and used for training.
Preparing Data for Training: The image and mask data are converted to NumPy arrays, normalized, and split into training and validation sets.
Training the Model: The U-Net model is compiled with the Adam optimizer and binary cross-entropy loss, and then trained on the prepared data.
Evaluating and Visualizing Results: Finally, the notebook includes code to predict segmentation masks on the training data and visualize the original image, the ground truth mask, and the predicted mask.
