# Maize Disease Classification

A convolutional neural network (CNN) classifies maize leaf images in the Maize Disease Classification mobile application.

## Classification categories

The CNN identifies four categories:

- Healthy
- Cercospora
- Common Rust
- Northern Leaf Blight

## Workflow

Capture a maize leaf image with the device camera or select one from the gallery. The application preprocesses the image, classifies it with the CNN, and displays the predicted category and probability. TensorFlow Lite runs the model in the mobile application.

![Maize disease classification data flow](assets/data-flow.png)

## Model performance

The CNN achieved 88% classification accuracy. The graph shows training and validation accuracy across epochs.

![Training and validation accuracy by epoch](assets/training-validation-accuracy.png)

## Leaf image examples

The images below show examples from each classification category.

| Healthy | Cercospora | Common Rust | Northern Leaf Blight |
| --- | --- | --- | --- |
| ![Healthy maize leaf](assets/healthy.jpg) | ![Cercospora on a maize leaf](assets/cercospora.jpg) | ![Common Rust on a maize leaf](assets/common-rust.jpg) | ![Northern Leaf Blight on a maize leaf](assets/northern-leaf-blight.jpg) |

## Project files

- `CNN/cnn.py` — CNN model and training script.
- `CNN/mdd.keras` — saved Keras model.
