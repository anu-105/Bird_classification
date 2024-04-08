# Bird_classification
Birds Image Classification Dataset
This dataset comprises 525 bird species with a total of 84,635 training images, 2,625 test images (5 images per species), and 2,625 validation images (5 images per species). Each image is of size 224x224 pixels in JPG format.

About the Dataset
Quality: This dataset is meticulously curated, ensuring high quality and cleanliness. Duplicate or near-duplicate images have been removed, and defective or low-information images have been filtered out. This ensures that there is no data leakage between the training, test, and validation datasets.

Image Content: Each image contains only one bird, with the bird typically occupying at least 50% of the pixels in the image. This ensures that even moderately complex models can achieve high accuracy rates, typically in the mid-90% range.

Data Structure: The dataset includes separate directories for training, test, and validation sets, with each directory containing subdirectories corresponding to each bird species. This structure is convenient for use with tools like Keras' ImageDataGenerator.flow_from_directory.

Dataset Description File (birds.csv): This CSV file contains information about the images, including file paths, class labels (bird species), scientific labels (Latin scientific names), and dataset designations (train, test, or validation). Additionally, it includes class ID values associated with each image file's class.

Image Collection: Images were gathered from internet searches by species name and subsequently checked for duplicates or near-duplicates. Afterward, they were cropped to ensure the bird occupies a significant portion of the image and resized to 224x224 pixels. All images are original and not created through augmentation.

Training Recommendations: Due to the large size of the dataset, it is recommended to use an image size of 150x150 pixels to reduce training time.

Data Balance: The training set is not perfectly balanced, with varying numbers of files per species. However, each species has at least 130 training image files.

Gender Representation: One significant shortcoming in the dataset is the ratio of male to female species images, with approximately 80% male and 20% female images. As males are typically more diverse in coloration compared to females, classifiers may not perform as well on female species images.
