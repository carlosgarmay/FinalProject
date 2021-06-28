# FinalProject --------- BY: Carlos Gargallo, Alex Urbano and Joel Tibau
Important information and remarks about the project:

- We developed the lab in Google Collab (without using the cluster) due to lack of some libraries in it. And so, it is uploaded as a .ipynb file proper structured
  properly structured to run in Collab (obvioulsy it can also be run in other similar IDEs, like Jupyter Notebook).
- Related to the stated above, even though the code is delivered in a condition where it shouldn't happen at first (with appropiate hyperparameters to avoid it), depending on how   big is the chunk of training and testing data you use or the number of epochs you set, it can be the case that Google Collab runs out of Cuda GPUs.
  If you run out of Cuda memory for GPU execution when doing training or testing, you can try to increase the parameter N. Also, you better try to mantain a low batch_size value     (like 16) and not increase too much the number of epochs. And, most importantly, remember to RESTART EXECUTION ENVIRONMENT at each execution (to empty cuda memory).
  These are just "radical" solutions in case you find in that situation, but the code is not behave to act like this (at least for us doesn't).
- Saved_models folder contains two .pth files which are pretrained models for both the discriminator and the generator, which enable the model to start out the training process     with some more information, enabling it to perform better and obtain higher quality results. If it wasn't because of these files, we would need a bigger dataset or a higher       resolution in our low resolution images in order to obtain "decent" and visually attractive super resolution images.
- Datasets train.mat and test.data (sent by email to Abdussalam) are not included here due to their big size (not accepted by github (25 MB maximum)). Next, it is attached the       link to a Google Drive folder Data which contains the training and testing datasets. You just have to dowload them and place them in the empty Data folder you can find in the     repository. The link is: https://drive.google.com/drive/folders/1oAs51rijqgnCfnYIyxu6iN-Wlz8dWU7L?usp=sharing
- Code is designed to store (grid structured) the output images as .png (low resolution, high resolution and super resolution) in output_images folder.
  Currently, this folder contains a few examples to show how the stored output would be like after execution.

