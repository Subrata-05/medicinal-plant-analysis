# Botanica.ai

## AI-Powered Indian Medicinal Plant Recognition System

Botanica.ai is a deep learning-based computer vision project designed to identify Indian medicinal plants from images and provide relevant botanical and medicinal information about the recognized species.

The system combines transfer learning with EfficientNetB3 for image classification and a structured knowledge base to provide information such as scientific name, plant family, common names, parts used, key compounds, traditional uses, and safety precautions.

## Key Features

- Medicinal plant classification using an EfficientNetB3-based deep learning model.
- Support for 28 Indian medicinal plant species.
- Transfer learning using an EfficientNetB3 model pretrained on ImageNet.
- Image preprocessing and data augmentation for model training.
- Retrieval of botanical and medicinal information associated with the predicted plant.
- Safety and precaution information for plants that may require careful handling.
- Model evaluation and performance metric generation.
- GPU-compatible training workflow using Google Colab.

## Machine Learning Pipeline

```text
Input Image
     |
     v
Image Preprocessing
     |
     v
Data Augmentation
     |
     v
EfficientNetB3
     |
     v
Transfer Learning and Fine-Tuning
     |
     v
Plant Classification
     |
     v
Class Mapping
     |
     v
Medicinal Information Retrieval
     |
     v
Plant Information and Safety Precautions
```

## Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Deep Learning | TensorFlow, Keras |
| Model Architecture | EfficientNetB3 |
| Transfer Learning | ImageNet |
| Data Processing | Pandas, NumPy |
| Data Augmentation | Keras ImageDataGenerator |
| Visualization | Matplotlib |
| Model Evaluation | Scikit-learn |
| Training Environment | Google Colab, GPU |

## Supported Plant Classes

The current model supports 28 medicinal plant classes:

1. Adathoda
2. Banana
3. Bush Clock Vine
4. Champaka
5. Chitrak
6. Common Lantana
7. Crown Flower
8. Datura
9. Four O' Clock Flower
10. Hibiscus
11. Honey Suckle
12. Indian Mallow
13. Jatropha
14. Malabar Melastome
15. Marigold
16. Nagapoovu
17. Nityakalyani
18. Pinwheel
19. Rose
20. Shankupushpam
21. Spider Lily
22. Sunflower
23. Thechi
24. Thumba
25. Touch Me Not
26. Tridax procumbens
27. Wild Potato Vine
28. Yellow Daisy

## Dataset

The project uses the IMFI (Indian Medicinal Flower Image) Dataset, containing images representing Indian medicinal flower species.

The dataset and trained model files are not included in this repository because of their size and distribution considerations.

### Dataset Setup

To train the model:

1. Obtain the IMFI dataset.
2. Organize the images according to their respective class directories.
3. Upload the dataset to Google Drive.
4. Open `colab_train.ipynb` using Google Colab.
5. Select a GPU runtime.
6. Update the dataset path if required.
7. Execute the notebook to train the model.

## Getting Started

### Prerequisites

Make sure Python is installed on your system.

Clone the repository:

```bash
git clone https://github.com/Subrata-05/medicinal-plant-analysis.git
```

Navigate to the project directory:

```bash
cd medicinal-plant-analysis
```

Install the required dependencies:

```bash
pip install tensorflow numpy pandas matplotlib scikit-learn
```

## Model Training

For model training, open `colab_train.ipynb` in Google Colab.

The notebook performs the following steps:

- Dataset loading
- Image preprocessing
- Data augmentation
- Transfer learning
- Model training
- Validation
- Model evaluation
- Model saving

After training, the model can be saved as:

```text
medicinal_model.keras
```

along with the corresponding class-index mapping.

## Model Inference

Once the trained model and class-index file are available, run:

```bash
python test_model.py
```

The inference pipeline accepts an image and generates the predicted plant class along with its prediction confidence.

The associated medicinal information can then be retrieved from the project's JSON knowledge base.

## Project Structure

```text
medicinal-plant-analysis/
|
├── .gitignore
├── LICENSE
├── README.md
|
├── colab_train.ipynb
├── Medicinal_Plant_Training.ipynb
├── project.ipynb
├── project1.ipynb
|
├── train_medicinal.py
├── train_script.py
├── inference.py
├── generate_metrics.py
├── test_model.py
|
├── class_indices.json
├── medicinal_class_indices.json
├── medicinal_properties.json
└── test_model.md
```

## Model Evaluation

The repository includes utilities for evaluating the trained classification model and generating performance metrics.

The evaluation workflow can be used to analyze:

- Classification accuracy
- Precision
- Recall
- F1-score
- Class-wise performance
- Prediction results

Actual performance metrics should be reported here after evaluating the final trained model on a test dataset.

## Disclaimer

The medicinal information presented by Botanica.ai is intended for educational and informational purposes only.

The system is not intended to provide medical diagnosis, treatment recommendations, or professional medical advice.

Plant identification predictions should be independently verified, and medicinal plants should not be consumed or used for treatment based solely on the output of this system.

## Future Improvements

Potential future enhancements include:

- Increasing the number of supported medicinal plant species.
- Improving classification performance using larger and more diverse datasets.
- Deploying the trained model through a REST API.
- Developing a web-based user interface.
- Adding multilingual plant information.
- Implementing model explainability using techniques such as Grad-CAM.
- Deploying the application as a cloud-based service.

## Project

Botanica.ai was developed as a collaborative machine learning and computer vision project focused on applying deep learning to medicinal plant recognition.

### Core Areas

- Computer Vision
- Deep Learning
- Transfer Learning
- Image Classification
- Data Processing
- Model Evaluation
- Medicinal Plant Knowledge Retrieval

## License

This project is licensed under the terms specified in the `LICENSE` file.
# Botanica.ai

## AI-Powered Indian Medicinal Plant Recognition System

Botanica.ai is a deep learning-based computer vision project designed to identify Indian medicinal plants from images and provide relevant botanical and medicinal information about the recognized species.

The system combines transfer learning with EfficientNetB3 for image classification and a structured knowledge base to provide information such as scientific name, plant family, common names, parts used, key compounds, traditional uses, and safety precautions.

## Key Features

- Medicinal plant classification using an EfficientNetB3-based deep learning model.
- Support for 28 Indian medicinal plant species.
- Transfer learning using an EfficientNetB3 model pretrained on ImageNet.
- Image preprocessing and data augmentation for model training.
- Retrieval of botanical and medicinal information associated with the predicted plant.
- Safety and precaution information for plants that may require careful handling.
- Model evaluation and performance metric generation.
- GPU-compatible training workflow using Google Colab.

## Machine Learning Pipeline

```text
Input Image
     |
     v
Image Preprocessing
     |
     v
Data Augmentation
     |
     v
EfficientNetB3
     |
     v
Transfer Learning and Fine-Tuning
     |
     v
Plant Classification
     |
     v
Class Mapping
     |
     v
Medicinal Information Retrieval
     |
     v
Plant Information and Safety Precautions
```

## Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Deep Learning | TensorFlow, Keras |
| Model Architecture | EfficientNetB3 |
| Transfer Learning | ImageNet |
| Data Processing | Pandas, NumPy |
| Data Augmentation | Keras ImageDataGenerator |
| Visualization | Matplotlib |
| Model Evaluation | Scikit-learn |
| Training Environment | Google Colab, GPU |

## Supported Plant Classes

The current model supports 28 medicinal plant classes:

1. Adathoda
2. Banana
3. Bush Clock Vine
4. Champaka
5. Chitrak
6. Common Lantana
7. Crown Flower
8. Datura
9. Four O' Clock Flower
10. Hibiscus
11. Honey Suckle
12. Indian Mallow
13. Jatropha
14. Malabar Melastome
15. Marigold
16. Nagapoovu
17. Nityakalyani
18. Pinwheel
19. Rose
20. Shankupushpam
21. Spider Lily
22. Sunflower
23. Thechi
24. Thumba
25. Touch Me Not
26. Tridax procumbens
27. Wild Potato Vine
28. Yellow Daisy

## Dataset

The project uses the IMFI (Indian Medicinal Flower Image) Dataset, containing images representing Indian medicinal flower species.

The dataset and trained model files are not included in this repository because of their size and distribution considerations.

### Dataset Setup

To train the model:

1. Obtain the IMFI dataset.
2. Organize the images according to their respective class directories.
3. Upload the dataset to Google Drive.
4. Open `colab_train.ipynb` using Google Colab.
5. Select a GPU runtime.
6. Update the dataset path if required.
7. Execute the notebook to train the model.

## Getting Started

### Prerequisites

Make sure Python is installed on your system.

Clone the repository:

```bash
git clone https://github.com/Subrata-05/medicinal-plant-analysis.git
```

Navigate to the project directory:

```bash
cd medicinal-plant-analysis
```

Install the required dependencies:

```bash
pip install tensorflow numpy pandas matplotlib scikit-learn
```

## Model Training

For model training, open `colab_train.ipynb` in Google Colab.

The notebook performs the following steps:

- Dataset loading
- Image preprocessing
- Data augmentation
- Transfer learning
- Model training
- Validation
- Model evaluation
- Model saving

After training, the model can be saved as:

```text
medicinal_model.keras
```

along with the corresponding class-index mapping.

## Model Inference

Once the trained model and class-index file are available, run:

```bash
python test_model.py
```

The inference pipeline accepts an image and generates the predicted plant class along with its prediction confidence.

The associated medicinal information can then be retrieved from the project's JSON knowledge base.

## Project Structure

```text
medicinal-plant-analysis/
|
├── .gitignore
├── LICENSE
├── README.md
|
├── colab_train.ipynb
├── Medicinal_Plant_Training.ipynb
├── project.ipynb
├── project1.ipynb
|
├── train_medicinal.py
├── train_script.py
├── inference.py
├── generate_metrics.py
├── test_model.py
|
├── class_indices.json
├── medicinal_class_indices.json
├── medicinal_properties.json
└── test_model.md
```

## Model Evaluation

The repository includes utilities for evaluating the trained classification model and generating performance metrics.

The evaluation workflow can be used to analyze:

- Classification accuracy
- Precision
- Recall
- F1-score
- Class-wise performance
- Prediction results

Actual performance metrics should be reported here after evaluating the final trained model on a test dataset.

## Disclaimer

The medicinal information presented by Botanica.ai is intended for educational and informational purposes only.

The system is not intended to provide medical diagnosis, treatment recommendations, or professional medical advice.

Plant identification predictions should be independently verified, and medicinal plants should not be consumed or used for treatment based solely on the output of this system.

## Future Improvements

Potential future enhancements include:

- Increasing the number of supported medicinal plant species.
- Improving classification performance using larger and more diverse datasets.
- Deploying the trained model through a REST API.
- Developing a web-based user interface.
- Adding multilingual plant information.
- Implementing model explainability using techniques such as Grad-CAM.
- Deploying the application as a cloud-based service.

## Project

Botanica.ai was developed as a collaborative machine learning and computer vision project focused on applying deep learning to medicinal plant recognition.

### Core Areas

- Computer Vision
- Deep Learning
- Transfer Learning
- Image Classification
- Data Processing
- Model Evaluation
- Medicinal Plant Knowledge Retrieval

## License

This project is licensed under the terms specified in the `LICENSE` file.
sidered professional medical advice. Always consult a qualified healthcare provider or Ayurvedic practitioner before using any plant for medicinal purposes. Some plants included in the dataset (e.g., Datura, Crown Flower) are highly toxic.
