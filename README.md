# Driving_Pal
A drowsiness and distraction detector using openCV, dlib and keras which would monitor the eyes of the vehicle driver and activate a sound alarm if he dozes during driving. If he is not dozing, but yawning, then remind him to stop nearby for a coffee.
Next I generated 'eye' dataset by capturing my random eye movement in a live feed and converting the ROI of every frame to image for 15 minutes.This generated around 3k images consisting of distracted eyes and focused eyes. Used keras and fed this dataset to a convolutional neural network model to perform clustering. Model returned a probabilty, If this probability is less than 0.5 then we conclude the driver is distracted and warn him, otherwise let him enjoy the ride.
