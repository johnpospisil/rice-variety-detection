# Rice Variety Detection with Computer Vision

![Rice Field](rice-field.jpg)

This repository contains code and documentation for classifying five different rice varieties—Arborio, Basmati, Ipsala, Jasmine, and Karacadag—using deep learning techniques. I explore both a custom Convolutional Neural Network (CNN) and a transfer learning approach (e.g., MobileNetV2) to achieve high classification accuracy on a large dataset of rice grain images.

## Project Overview

- **Objective:** Automatically identify the variety of rice from an image of a single grain.  
- **Datasets:** Organized into folders named for each variety, each containing multiple images of individual rice grains.  
- **Methods:**  
  1. **Transfer Learning** – Leveraging a pre-trained model to classify rice varieties.  
  2. **Custom CNN** – Designing a domain-specific architecture from scratch.

---

## Repository Structure

```
.
├── Rice_Image_Dataset/
│   ├── Arborio/
│   ├── Basmati/
│   ├── Ipsala/
│   ├── Jasmine/
│   └── Karacadag/
├── rice-variety-detection-with-computer-vision.ipynb
└── README.md
```

- **Rice_Image_Dataset/**  
  Contains the images split by rice variety.  
- **notebook/**  
  Jupyter notebook demonstrating the model training, evaluation, and visualizations.  
- **README.md**  
  This file.  

---

## Requirements

- Python 3.11
- TensorFlow/Keras 2.19.0  
- NumPy  
- Matplotlib  
- scikit-learn  
- (Optional) Jupyter Notebook for running `.ipynb` files

---

## Usage

1. **Clone this repository:**

   ```bash
   git clone https://github.com/johnpospisil/rice-variety-detection.git
   cd rice-variety-detection
   ```

2. **Run the notebooks:**
   - Open `rice-variety-detection-with-computer-vision.ipynb` in Jupyter (or any compatible environment).
   - Adjust the paths to your dataset if necessary.
   - Run the cells to train and evaluate the models.

3. **Evaluate Results:**
   - Inspect the accuracy and loss plots for training and validation.
   - Review the confusion matrices to see which varieties are most commonly misclassified.
   - Check the final test accuracy in the notebook output.

---

## Results

- **Custom CNN:** Achieved around **99.5%** test accuracy, demonstrating strong ability to learn subtle differences between rice varieties.  
- **Transfer Learning (MobileNetV2):** Reached approximately **98.3%** test accuracy, still highly effective but slightly lower than the custom CNN.

Both methods show minimal misclassifications, with confusion matrices highlighting only a few mix-ups among visually similar grains.

---

## Future Work

- **Fine-Tuning Transfer Learning:** Unfreezing more layers and lowering the learning rate may narrow the performance gap.  
- **Data Augmentation:** Applying more targeted augmentations could further improve generalization.  
- **Real-World Validation:** Testing on images from different lighting conditions or camera types is essential for robust deployment.

---

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use, modify, and distribute this code for your own projects.

---

## Contact

For any questions or suggestions, please [reach out to me vial email](mailto:john@johnpospisil.com).

Enjoy exploring rice variety detection with computer vision!
