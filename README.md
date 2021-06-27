# FinalProject
Important information and remarks about the project:

- We developed the lab in Google Collab (without using the cluster) due to lack of some libraries in it, like tqdm. And so, it is uploaded as a .ipynb file proper structured
  properly structured to run in Collab (obvioulsy it can also be run in other similar IDEs, like Jupyter Notebook).
- Related to the stated above, even though the code is delivered in a condition where it shouldn't happen at first (with appropiate hyperparameters to avoid it), depending on how     big is the chunk of training and testing data you use, it can be the case that Google Collab runs out of Cuda GPUs. That's why
  If you run out of Cuda memory for GPU execution when doing training or testing, you can try to increase the parameter N. Also, you better try to mantain a low batch_size value     (like 16) and not increase too much the number of epochs. And, most importantly, remember to RESTART EXECUTION ENVIRONMENT at each execution (to empty cuda memory).
  These are just "extreme" solutions in case you find in that situation, but the code is not meant to act like this.
- Code is designed to store (grid structured) the output images as .png (low resolution, high resolution and super resolution) in output_images folder.
  Currently, this folder contains a few examples to show how the stored output would be like after execution.
- 
