This is a project on my Masters in Data Science for the course "Advanced Machine Learning". It was a kaggle competition lying in the category of Image Classification on which me and my colleague managed to finish in the second place.

The goal for the competition was to detect pneumonia from X-Rays. The "Advanced Machine Learning-Pneumonia Detection" pdf file will guide you through the thought process - and execution.

TLDR; It involves various techniques, such as a custom 9-layer CNN, the dealing of overfitting with Dropout layers & L2 Regularization techniques, Visual Transformers, data augmentation, fine-tuning and K-Fold cross validation.

After various attempts, we ended up using 2 pretrained models, the "EfficientNet B0" and the "DenseNet 121". The best result came after using ensambling techniques.

We trained 2 EfficientNet B0 and 2 DenseNet 121 models with the "Adam" optimizer and froze different amounts of layers (depending on the pre-trained model), then we finally used the ensamble technique for these 4 models, achieving an accuracy of 85%.
