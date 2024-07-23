Indian Food Image Classifier
Description
This repository contains a deep learning model designed to classify Indian food images into 20 different classes using the Inception V3 architecture.

Features
20 Classes: The model can classify images into 20 distinct categories of Indian food. Inception V3: Utilizes the powerful Inception V3 architecture for accurate image classification.

Installation
To install, clone the repository using git clone https://github.com/Raghav-Selvakumar/Indian-Food-Image-Classifier.git, navigate to the repository directory with cd Indian-Food-Image-Classifier, and install the required dependencies using pip install -r requirements.txt.

Usage
To use the model, load the model and weights with from tensorflow.keras.models import load_model and model = load_model('path_to_model.h5'). For making predictions, use the following code: import numpy as np; from tensorflow.keras.preprocessing import image; img = image.load_img('path_to_image.jpg', target_size=(299, 299)); x = image.img_to_array(img); x = np.expand_dims(x, axis=0); x = x / 255.0; preds = model.predict(x); print('Predicted:', np.argmax(preds)).

Contact
For support or questions, please contact: raghavselva03@gmail.com
