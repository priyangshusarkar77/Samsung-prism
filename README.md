# SAMSUNG PRISM PROJECT (R&D Bangalore)

1. Explore & Implement Image Augmentation Options

About the concept: Image Augmentation is a technique using which we can artificially generate or expand the dataset. This is done by introducing some random changes or transformations on the existing dataset.
The image Augmentation technique takes advantage of a property called The Transformation Invariance property. This property states that the information contained in the image is preserved even after introducing random transformations.
Image Augmentation is used in the following situations:
	1. When we have less training data to train a Neural Network.
	2. When the trained network is Overfitting.
	3. When the performance of the network is not up to the mark.
Techniques used in Image Augmentation include rotation, flipping, elastic distortion, changing brightness-contrast values, wrapping, etc.
Image Augmentation technique is used by almost all major image processing related tasks like in AlexNet, ResNet of ImageNet competition.
In one sentence we can say that Image Augmentation is a well-tested and proven technique that improves the performance of the networks on a scale.

Our Approach on Image Augmentation Techniques:
Method 1: Provide all possible transformations to the model (This is not a practical approach. The space and time complexities are not acceptable).
Method 2: Treating this problem as a search problem and find various sequence of augmentation techniques and choose the sequence which impact the model most. (This is a good approach but finding a right sequence of augmentations is difficult because there are infinite number of variations possible).
Method 3 (Our approach): 
Step 1 (Categorization of Dataset): In this step, based on the domain we will categorize which type features we want to preserve. Based on this, we will narrow down in certain set of augmentations.
Step 2 (Applying of the Techniques): Based on the size of the dataset we have; we will be applying the techniques on each image. If we have good amount data to start with, then, we will only apply augmentations to certain images and only certain techniques.

Challanges during the project
1. From the research point of view, Image Augmentation is not an active topic but a passive topic. Due to that, it is challenging to find research articles on this topic.
2. In Image Augmentation, there is an infinite number of ways to introduce random transformations. So, it is difficult to select which type of transformation is suitable for an image.
3. Image Augmentation can only be used on data that has transformation invariance property. It is a challenge to find a dataset that has this property well maintained.
4. Image Augmentation techniques should be implemented strictly based on domain knowledge. For example, we cannot distort MRI scan images. 
5.As mentioned before, there are infinite possible ways to apply transformations. Even evaluating the performance of the network is computationally expensive.
6. Image Augmentation techniques should be handled carefully. Otherwise, it will have the opposite effect on the performance of the model.
