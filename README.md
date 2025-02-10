# Flickr8K-Image-Captioning-using-CNNs-LSTMs

## Overview
This project implements an **image captioning system** using **Convolutional Neural Networks (CNNs)** and **Long Short-Term Memory (LSTMs)**. The model is trained on the **Flickr8k dataset**, which consists of images paired with human-annotated captions.

## Dataset Information
The **Flickr8k dataset** contains images with corresponding textual descriptions. The dataset is used for training, validation, and testing image captioning models.

### **Dataset Files**
- **Flickr8k.token.txt** - Raw captions for each image, formatted as `image_filename # caption_number` followed by the caption text.
- **Flickr8k.lemma.txt** - Lemmatized version of captions where words are reduced to their base forms.
- **Flickr_8k.trainImages.txt** - List of training images.
- **Flickr_8k.devImages.txt** - List of validation images.
- **Flickr_8k.testImages.txt** - List of test images.
- **ExpertAnnotations.txt** - Expert judgments on captions, scored from **1 to 4** based on accuracy.
- **CrowdFlowerAnnotations.txt** - Crowdsourced judgments indicating whether captions correctly describe images.

## Model Architecture
The image captioning model consists of:
1. **Feature Extraction using CNNs** - A pre-trained **Xception** model extracts visual features from images.
2. **Sequence Modeling using LSTMs** - An LSTM network generates captions based on extracted image features.

### Training Steps
- **Extract Image Features**: Use **Xception** to extract features from images.
- **Process Captions**: Tokenize and clean text descriptions.
- **Train LSTM Model**: Train an LSTM model to generate captions.
- **Evaluate Model**: Compare generated captions with ground truth.

## Setup & Running the Notebook
### 1. **Clone the Repository**
```sh
git clone https://github.com/your-repo/flickr8k-image-captioning.git
cd flickr8k-image-captioning
```

### 2. **Open Jupyter Notebook**
```sh
jupyter notebook
```

### 3. **Run the Notebook**
- Open `flickr8k-image-captioning-using-cnns-lstms.ipynb`.
- Run all cells sequentially to:
  1. Load the dataset.
  2. Extract image features.
  3. Train the captioning model.
  4. Generate captions for new images.

### 4. **Dataset Download**
Download the **Flickr8k dataset** from Kaggle:
🔗 [Flickr8k Dataset](https://www.kaggle.com/datasets/adityajn105/flickr8k)


## Citations
```
M. Hodosh, P. Young and J. Hockenmaier (2013)
"Framing Image Description as a Ranking Task: Data, Models and Evaluation Metrics",
Journal of Artificial Intelligence Research, Volume 47, pages 853-899.
URL: http://www.jair.org/papers/paper3994.html
```

## License
This project is for educational purposes only. Ensure compliance with the dataset’s terms of use before deployment.

---

