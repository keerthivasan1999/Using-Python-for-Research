Uploading Jupyter notebook file and csv files of course final project (Physical Activity Detector)
# INTRODUCTION
**Prediction of the type of physical activity (e.g., walking, climbing stairs) from tri-axial smartphone accelerometer data**

Smartphone accelerometers are precise, and different physical activities give rise to varying acceleration patterns. The input data used for training in this project consists of two files. The first file, train_time_series.csv, contains the raw accelerometer data, it has the following format:

timestamp, UTC time, accuracy, x, y, z

We can use the timestamp column as our time variable; we'll also need the last three columns, here labeled x, y, and z, which correspond to measurements of linear acceleration along each of the three orthogonal axes.

The second file, train_labels.csv, contains the activity labels, and we'll be using these labels to train our model. Different activities have been numbered with integers. We use the following encoding: **1 = standing, 2 = walking, 3 = stairs down, 4 = stairs up**. Because the accelerometers are sampled at high frequency, the labels in train_labels.csv are only provided for every 10th observation in train_time_series.csv.

Our goal is to classify different physical activities as accurately as possible. To test our code, we're also provided with a file called test_time_series.csv, we need to give the activity labels predicted by our code for this test data set.
