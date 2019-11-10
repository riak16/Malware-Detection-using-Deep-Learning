# Malware-Detection-using-Deep-Learning

## Installations:
CUDA - 9.0
CuDNN - 7.0.5
Python - 3.5+
Anaconda - 3

## Python Libraries :
	-Tensorflow GPU enabled .
	-Windows version x86 exe(local).
	-Pillow.
	-Numpy.

## Steps:
  - If you don't have benign files, use the benignGenerator.py to crawl your local machines and collect .exe files, which you can use as nenign files in your dataset.
  - Update the paths in ias.py file according to the location of the files. Use absolute paths.
	- Make sure the folders in path2 and path3 (destination of the output images 256x256 and 32x32 respectively) are created beforehand.
	- Run the ias_full.py file.
  - Update the paths in cnn1.py and build_image_data.py files according to the location of the files. Use absolute paths.
	- Run build_image_data.py. Make sure that label.txt is in the same folder as build_image_data as well as the folders(named after the 
		classes in label.txt) are in the same folder.
	- Run the build_image_data.py file. After running the file you should see "train-00000-of-00002.tfrecord" and 
		"train-00000-of-00002.tfrecord" files created.
	- Run cnn1.py. This will take a long time to run.
	- Update the paths in cnn1.py and build_image_data.py files according to the location of the files. Use absolute paths.
	- Run build_image_data.py. Make sure that label.txt is in the same folder as build_image_data as well as the folders(named after the 
		classes in label.txt) are in the same folder.
	- Run the build_image_data.py file. After running the file you should see "train-00000-of-00002.tfrecord" and 
		"train-00000-of-00002.tfrecord" files created.
	- Run cnn1.py. This will take a long time to run.

IEEE Paper link(base paper): http://ieeexplore.ieee.org/document/8190895/references?ctx=references

The code in jupyter notebook uses fast.ai libraries to solve the same problem statement. The code has been written after following the first lecture of the fast.ai lecture. to understand the code go through the pet classification problem in the lecture.

### Note: The model implemented using fast.ai libraries gives much better results than the one implemented using tensorflow.
