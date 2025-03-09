# Pokémon Image Classification

## Introduction
This project involves building a neural network model to classify Pokémon images based on their types. The goal is to preprocess the images, remove their backgrounds, and train a deep learning model to predict the Pokémon type. The types considered include: **Water, Normal, Grass, Bug, Fire, Psychic, Electric**, and others classified as **Other**.

## Workflow Summary
1. **Data Loading:** Load the Pokémon dataset and classify types.
2. **Image Preprocessing:** Remove background, resize images, and convert to arrays.
3. **Data Preparation:** Encode labels, normalize images, and split data.
4. **Model Building:** Define and train a neural network model.
5. **Results Visualization:** Plot training accuracy.

## Libraries Used
- **numpy**: Numerical operations
- **pandas**: Data manipulation
- **matplotlib, seaborn**: Data visualization
- **sklearn**: Label encoding and data splitting
- **tensorflow.keras**: Neural network model building
- **PIL, cv2**: Image processing
- **glob**: File handling

## Background Removal
The `remove_background(image)` function:
- Converts images to grayscale.
- Applies binary thresholding to create a mask.
- Uses the mask to remove the background.

## Dataset Processing
- Load Pokémon images and their types.
- Resize images to **120x120 pixels**.
- Normalize pixel values to [0, 1].
- Label encode Pokémon types.

## Model Architecture
- **Input Layer:** Flattens the image input.
- **Hidden Layers:** Dense layers with ReLU activation and Dropout.
- **Output Layer:** Dense layer with Softmax activation.
- **Loss Function:** Sparse categorical crossentropy.
- **Optimizer:** Adam.

## Training
- Use data augmentation to generate varied images.
- Train the model for **50 epochs**.
- Track training and validation accuracy.

## Results Visualization
- Plot accuracy over epochs.
- Compare training vs validation accuracy.

## How to Run the Project
1. Clone the repository.
2. Place the Pokémon images and CSV file in the working directory.
3. Run the Jupyter Notebook.
4. The model will train and output accuracy plots.

## Future Improvements
- Use Convolutional Neural Networks (CNN) for better accuracy.
- Add more Pokémon types to the dataset.
- Implement a web app for real-time classification.

## File Name
**README.md**
