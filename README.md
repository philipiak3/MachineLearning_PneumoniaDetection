This is a project on the Data Science MSc programme for the course "Advanced Machine Learning". This was an Image Classification Kaggle competition on which me and my colleague managed to finish in the second place.

The goal for the competition was to detect pneumonia from X-Rays. The "Advanced Machine Learning-Pneumonia Detection" pdf file will guide you through the thought process - and execution.

**TLDR;** It involves various techniques, including a custom 9-layer CNN, handling overfitting with Dropout layers, L2 Regularization techniques and K-Fold cross validation, Visual Transformers, data augmentation and fine-tuning.

After various attempts, we ended up using 2 pretrained models, the "EfficientNet B0" and the "DenseNet 121". The best result came after using ensembling techniques.

We trained 2 EfficientNet B0 and 2 DenseNet 121 models with the "Adam" optimizer and froze different amounts of layers on each model (depending on the pre-trained model), and we then used an ensemble of these 4 models, achieving an accuracy of 85%.
