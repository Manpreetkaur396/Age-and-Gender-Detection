# Age-and-Gender-Detection

# About Dataset

 This dataset serves as a benchmark for face photos and is inclusive of various real-world imaging conditions like noise, lighting, pose, and appearance. The images have been collected from Flickr albums and distributed under the Creative Commons (CC) license. It has a total of 26,580 photos of 2,284 subjects in eight age ranges (as mentioned above) and is about 1GB in size. The models we will use have been trained on this dataset.
The dataset is composed of 5 folds to allow 5-fold 'leave one out' cross validation. To prevent overfitting, each fold contains different subjects. 

Each fold is described by a csv file with 12 columns:

user_id - the folder in the dataset containing the image. 
original_image - image name in the dataset.
face_id - the Face ID in the original Flickr image, can be ignored. 
age - age label of the face.
gender - gender label of the face.
x, y, dx, dy - bounding box of the face in the original Flickr image, can be ignored.
tilt_ang, fiducial_yaw_angle - pose of the face in the original Flickr image, can be ignored. 
fiducial_score - score of the landmark detector, can be ignored. 

If you use the dataset, please cite: Eran Eidinger, Roee Enbar, Tal Hassner. Age and Gender Estimation of Unfiltered Faces. Transactions on Information Forensics and Security (IEEE-TIFS), special issue on Facial Biometrics in the Wild, Volume 9, Issue 12, pages 2170 - 2179, 2014.
