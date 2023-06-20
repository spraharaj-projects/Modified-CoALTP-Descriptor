# Modified CoLTP Face Retrival System


# ABSTRACT

Searching for similar face images in large databases is a time-consuming work and an efficient face image retrieval system is valuable in this situation. Content-based face image retrieval is searching for similar face images to a given query face image in a large database. The feature extraction method adopted for extracting visual features from the given face image, plays an important role in CBFIR. Texture is a prominent feature of image which can extract contents of image, hence a good texture feature extractor is necessary for content-based image retrieval process. In this project, a new texture descriptor is developed which is a combination of Local Ternary Pattern (LTP) and gray level co-occurrence matrix (GLCM). This feature descriptor which is named as CoALTP, inherits the attributes of both LTP and GLCM. First LTPs of pixels are obtained and then using GLCM in four directions, co-relations between pixel pairs are calculated as features. The PCA is used in order to reduce the dimension of the extracted features.

# INTRODUCTION

Content based face image retrieval (CBFIR) is the application of Computer vision techniques to the face image retrieval problem and face recognition problem, that is, the problem of searching for digital face images in large databases. The Content Based Face Image Retrieval tries to solve this problem as it provides the means to index, search and retrieve specific face images. Content Based Face Image Retrieval is a task of searching face images of a person from a database and retrieval of face images, which are seems to be visually similar to a given example or query face image. Content-based Face image retrieval uses the visual contents of an image such as color, shape, texture, and spatial layout to represent and index the image. In typical content-based face image retrieval systems, the visual contents of the images in the database are extracted and described by multi-dimensional feature vectors. These feature vectors can be computed by different methods available to the users. The CBIR system consists of following components:

- **Query Face image:** It is the image to be search in the image database whether the same image is present or not or how many are similar kind images are existing or not.
- **Face Image Database:** It consists of n number of images depends on the user choice.
- **Feature extraction:** It extracts visual information from the image and saves them as features vectors in a features database. The feature extraction finds the image description in the form of feature value (or a set of value called a feature vector) for each pixel. These feature vectors are used to compare the query with the other images and retrieval.
- **Dimension reduction:** The extracted feature vector contains a huge number of variables. The feature vector is dimensionally reduced in order to comparisons faster.
- **Face Image matching:** The information about each image is stored its feature vectors for computation process and these feature vectors are matched with the feature vectors of query image which helps in measuring the similarity.
- **Resultant Retrieved face images:** It searches the previously maintained information to find the matched images from database. The output will be the similar images having same or very closest features as that of the query image.
