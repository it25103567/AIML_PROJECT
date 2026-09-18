# AI-Based Crop Disease Detection

**Dataset:** https://www.kaggle.com/datasets/jawadal1045/20k-multi-class-crop-disease-images

This project focuses on developing a machine learning system for crop
disease classification using crop leaf images. The dataset contains
images representing different crop diseases across multiple crops.

The project focuses on Exploratory Data Analysis (EDA) and data
preprocessing to prepare the dataset for the subsequent machine learning
stages.

## Group Members

| Student ID | Student Name | Task |
|---|---|---|
| IT25103052 | Vidhyadhakshini G.I. | Class Imbalance Handling |
| IT25103229 | Haadiya M.H. | Pixel Normalization |
| IT25103233 | Ammara M.S | Image Resizing |
| IT25103274 | Wardini K. R. V. | Image Color/Channel Preprocessing |
| IT25103371 | Nafas M.K | Data Augmentation |
| IT25103567 | Ranasinghe U. I. | Categorical Label Encoding |
| IT25103599 | Samararathna D. K. | Image Quality Enhancement |

## Project Structure

- `notebooks/` : Contains Jupyter/Colab notebooks for different stages of the
  machine learning pipeline.
- `data/` : Contains the datasets used throughout the project.
- `EDA/` : Contains generated EDA visualizations for the preprocessing
  techniques.
- `outputs/` : Contains the generated preprocessing outputs and results.
- `Group_Preprocessing_Pipeline/` : Contains the integrated group
  preprocessing pipeline.

## Data Preprocessing

The preprocessing stage prepares the crop disease images for machine
learning.

The following preprocessing techniques are performed in the required
order:

1. **Image Resizing:** Images are resized to a consistent dimension of
   **224 × 224** pixels to provide a standardized input size.

2. **Pixel Normalization:** Pixel values are converted from the original
   range of **0–255** to the range **0–1**.

3. **Data Augmentation:** Training images are transformed using techniques
   such as rotation, flipping, zooming, and shifting to increase data
   diversity.

4. **Categorical Label Encoding:** The 20 disease class names are converted
   into numerical labels for machine learning.

5. **Class Imbalance Handling:** The distribution of the 20 disease classes
   is examined to identify classes with substantially fewer images.
   Appropriate methods such as targeted augmentation or class weights
   are used where required.

6. **Image Color/Channel Preprocessing:** Image channels are checked to
   ensure consistency. Images with formats such as grayscale or RGBA can
   be converted to RGB when necessary.

7. **Image Quality Enhancement:** Images are investigated for issues such
   as poor contrast or excessive noise. Where justified, techniques such
   as contrast enhancement or denoising can be applied.

## Exploratory Data Analysis (EDA)

Exploratory Data Analysis is performed to understand the characteristics
and distribution of the crop disease dataset before and during the
preprocessing stage.

The EDA includes:

- Analysis of disease class distribution
- Analysis of class imbalance
- Analysis of image dimensions
- Analysis of pixel-value distributions
- Analysis of image color and channel information
- Visualization of original and transformed images
- Comparison of image characteristics before and after preprocessing

The generated visualizations help identify important patterns and
characteristics within the dataset and support the selection of
appropriate preprocessing techniques.

## Integrated Preprocessing Pipeline

The overall preprocessing workflow is:

**Raw Dataset**
→ **Image Resizing**
→ **Pixel Normalization**
→ **Data Augmentation**
→ **Categorical Label Encoding**
→ **Class Imbalance Handling**
→ **Image Color/Channel Preprocessing**
→ **Image Quality Enhancement**
→ **Final Preprocessed Dataset**

## Preprocessing Results

The integrated preprocessing pipeline produced the following results:

- Images standardized to **224 × 224 pixels**
- Pixel values normalized to **0–1**
- **3,160** additional augmented training images generated for 12 selected
  classes
- **20** disease classes encoded using numerical labels **0–19**
- Class distribution analyzed and class weights generated for the
  20 classes
- Images checked and represented using **RGB with 3 channels**
- Image quality enhancement demonstrated through contrast enhancement

## Conclusion

The data preprocessing stage of the Crop Disease AI project was
successfully completed by integrating the contributions of all seven
group members.

The dataset was processed through image resizing, pixel normalization,
data augmentation, categorical label encoding, class imbalance handling,
image color/channel preprocessing, and image quality enhancement.

The preprocessing results and EDA visualizations demonstrate the
transformations applied to the dataset and provide a structured
foundation for the subsequent machine learning stages.
