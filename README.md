# Image_Captioning-using-Pytorch-and-Flickr8k

## Requirements

This project requires the following libraries and environment to successfully run the Image Captioning model (ViT + Transformer Decoder):

### 1. Framework & Core Libraries
* `torch`, `torchvision`: For building, training, and optimizing the deep learning model.
* `transformers` (Hugging Face): Provides the architecture and pre-trained weights for the Vision Transformer (`google/vit-base-patch16-224-in21k`).

### 2. Data Processing & Visualization
* `pandas`, `numpy`: For tabular data manipulation and numerical operations.
* `matplotlib`, `opencv-python` (`cv2`), `Pillow` (`PIL`): For image processing and result visualization (including Attention Maps).
* `tqdm`: For displaying training progress bars.

### 3. NLP & Evaluation Metrics
* `spacy`: For English text tokenization.
* `nltk`: Required for computing the METEOR score.
* `rouge-score`: For ROUGE-L metric evaluation.
* `pycocoevalcap`: For comprehensive evaluation using standard Image Captioning metrics (BLEU 1-4, METEOR, ROUGE-L, CIDEr).

**Installation Command:**
```bash
pip install torch torchvision transformers pandas numpy matplotlib opencv-python Pillow tqdm spacy nltk rouge-score pycocoevalcap
python -m spacy download en_core_web_sm
```

###Data Source
* **Flickr30k:** [eeshawn/flickr30k](https://www.kaggle.com/datasets/eeshawn/flickr30k)
* **Flickr8k (Source 1):** [tuanphanthai/flickr8k](https://www.kaggle.com/datasets/tuanphanthai/flickr8k)
* **Flickr8k (Source 2):** [adityajn105/flickr8k](https://www.kaggle.com/datasets/adityajn105/flickr8k)

###Path Configuration (Kaggle / Google Colab / Local)
* `root_folder`: The path to the directory containing the input images (e.g., `.../flickr30k_images` or `.../Images`).
* `annotation_file`: The path to the text file containing the caption data (e.g., `captions.txt` or `captions.csv`).
