# assignment-3

1. **Data Preparation and Augmentation**:
   This section involves importing the necessary libraries and setting up data augmentation using the `ImageDataGenerator`. Images are augmented with various transformations, such as rotation, shifting, shearing, zooming, and flipping. The data is loaded into training and validation generators, ensuring effective training of the model on diverse data.

2. **MobileNetV2-based Mask Classification Model**:
   Here, a deep learning model for mask classification is created using the MobileNetV2 architecture, pretrained on ImageNet. The architecture is extended with additional layers for the specific mask classification task, including a global average pooling layer and fully connected layers. The model outputs probabilities for three classes: 'Incorrect Mask', 'With Mask', and 'Without Mask'.

3. **Real-time Mask Detection from Webcam**:
   The code switches focus to real-time mask detection using OpenCV and the trained model. The webcam captures video frames, and face detection is performed on each frame using a pre-trained deep learning model. Detected faces are preprocessed and classified using the MobileNetV2-based mask classification model. The predicted class is used to annotate the frame with a bounding box and mask label.

4. **Display and User Interaction**:
   The annotated frames are displayed in a window titled 'Mask Detection'. The loop continues until the user presses the 'q' key. Upon exiting the loop, the video capture is released, and all windows are closed.

Description:
This code showcases a dynamic real-time mask detection system utilizing advanced deep learning and computer vision techniques. The core of the implementation revolves around a sophisticated MobileNetV2-based model, meticulously trained to categorize facial states into three distinct classes: 'Incorrect Mask', 'With Mask', and 'Without Mask'. The code seamlessly captures video frames through a webcam feed, rapidly identifies faces, and employs the expertly trained model to predict the adherence to mask protocols.

**The accompanying dataset, a testament to meticulous curation and creation by ME**, serves as a cornerstone of the entire solution. It encapsulates diverse instances of mask-wearing scenarios, meticulously compiled and shaped by the creator's hands-on involvement. For a comprehensive understanding and access to this invaluable resource, kindly refer to the Kaggle page [Face Mask Classification: Mask, Unmask, Incorrect](https://www.kaggle.com/datasets/shariaarfin/mask-detection), bearing the distinctive mark of its creator.

