
### Description
For my capstone project, I wanted to train a convolutional neural network that could classify an image of a monkey by its species. There exist pre-trained neural networks that one can use to make an image classification task easier (VGG16, MobileNet, etc.), but I wanted to attempt to make one from scratch.

### Process
I gathered the data by downloading images of each monkey species; most species had between 50 and 100 images. I ended up with 40 species in all.

I began to train the neural network on every image, but quickly realized the task was taking much more time and computing power than I had available. I created a new, smaller dataset (only 3 species with 400 and 600 images per class) to fine-tune my model more quickly. After training the model on the smaller dataset, I decided to use this small dataset for my final model. I realized that the model may not work as well on the larger dataset because of the smaller class sizes.

### Model Architecture


![image](./images/model-1.png)
![image](./images/model-2.png)
![image](./images/model-3.png)

### Results

With my final model, I was only able to achieve an accuracy of 51%. While this is an 11-point improvement over the baseline (40%), I am not satisfied with the model in its current form. I would like to gather more images, add more layers, and train for a longer amount of time.

### Limitations and Next Steps:

In order to train a neural network like this, it’s said that a good rule of thumb is to have around 1000 images per class. My dataset’s largest class has 658 images. To create a better model, I would need many more images of each species.

The quality and content of the images is important. The images in my dataset were color, high-quality (1000x1000) images, with monkeys in different positions, backgrounds of trees and grass, and some images having watermarks or other text features. Much of the difficulty in training this model comes from the high variety in the types of patterns seen in the images. In the future, I would train the model for much longer with more computing power, most likely on the cloud.


