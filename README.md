# Face-Recognition-Clustering
Practice working with images, from the process of preparing the images to extracting the features from the images using a trained embedding model. Using the features of the images in order to divide them into clusters, that is, to associate different images of the same person to the same cluster.

In this Notebook, I will perform:

1. Preprocess: loading the images from a folder called 'images' in my Google Drive. Saving the coordinates of each face in each image, and creating a 'faces' folder that will contain all the faces found after the face recognition and cropping phase.
2. Finding the best K: performing K-means and finding the optimal K based on Inertia values and Silhouette score.
3. K-means and then T-SNE: creating a K-Means model with the chosen K, and dividing the data into clusters of images of the same famous person. Each cluster will have a folder with images of that celebrity. Then, dimensionality reduction using the T-SNE method to 2D.
4. T-SNE and then K-means: reverse order of operations. Reducing the dimensionality using the T-SNE method to 2D, and only then creating a K-Means model with the selected K.
5. T-SNE and then DBSCAN (density-based clustering): Reducing the dimensionality using the T-SNE method to 2D, and then creating a DBSCAN model with the optimal 'eps' and 'samples_min'.
6. Evaluation: comparing the performance of the models. K-means and then T-SNE Vs. T-SNE and then K-means Vs. T-SNE and then DBSCAN.

This notebook is based on images of famous people, and was developed using Python with the 'open_cv' and 'face_recognition' libraries.
