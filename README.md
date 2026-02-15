# Plant-Species-Image-Classification


Step 10: Upload All Required Files to GitHub
Your repository must contain:
● README.md







Reflection Questions:

1. How did the number of images per class affect your model’s accuracy?

The number of images per class had a strong impact on accuracy. Classes with more images were learned better by the model, resulting in higher accuracy and fewer errors, while classes with fewer images were often misclassified because the model did not see enough variations (size, color, lighting, and angle) to learn their features well. This caused class imbalance, which made the model biased toward classes with more samples.

2. Which plant species were most commonly misclassified and why?

Plant species with similar leaf shapes, textures, or colors were most commonly misclassified. For example, plants with similar green tones, vein patterns, or leaf sizes confused the model because deep learning relies on visual features, and these species look very similar in images. Poor lighting, background noise, and overlapping leaves also made it harder for the model to distinguish between them.

3. How did changing the epochs, batch size, or learning rate affect the training results?

Epochs:
Increasing epochs improved accuracy at first because the model learned more, but too many epochs caused overfitting, where the model memorized the training images and performed worse on new data.

Batch size:
Smaller batch sizes gave more stable learning but took longer to train, while larger batch sizes trained faster but sometimes resulted in less accurate models.

Learning rate:
A high learning rate caused the model to skip the best solution, while a very low learning rate made training slow. A balanced learning rate produced the best accuracy.

4. What challenges did you encounter during dataset collection and labeling?

The main challenges were:

Limited number of images for some plant species

Inconsistent lighting and backgrounds

Incorrect or unclear labels

Similar-looking plants that made labeling difficult
These issues introduced noise into the dataset, which affected training quality.

5. If you were to improve your model, what specific changes would you make and why?

To improve the model, I would:

Collect more images per plant species to reduce class imbalance

Use data augmentation (rotation, zoom, brightness changes) to increase image variety

Improve image quality and labeling accuracy

Fine-tune the learning rate, batch size, and number of epochs

Use a pre-trained CNN model (like MobileNet or ResNet) to improve feature extraction

These changes would help the model learn better, generalize more accurately, and reduce misclassification.
