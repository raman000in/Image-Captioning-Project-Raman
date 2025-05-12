# 🖼️ Image Captioning - Deep Learning Project

This project predicts captions for input images using a deep learning model trained on the Flickr8k dataset.

---

## 📁 Project Structure

| File/Folder                  | Description |
|-----------------------------|-------------|
| `Main.ipynb`                | Main training and inference notebook |
| `Data Preprocessing.ipynb`  | Optional notebook for initial processing |
| `Flickr8k.token.txt`        | Captions for all images |
| `Flickr_8k.trainImages.txt` | Training image list |
| `flickr_8k_train_dataset.txt` | Preprocessed train file (image + caption) |
| `captions.npy`              | Padded sequence data |
| `next_words_compressed.npz` | Compressed next word vectors (under 25MB) |
| `train_encoded_images_subset.pkl.gz` | Compressed encoded images (under 25MB) |
| `README.md`                 | This file |
| `requirements.txt`          | Python dependencies |

---

## 🧠 Model

- Feature extractor: VGG16 (last FC layer removed)
- Decoder: LSTM
- Optimizer: Adam
- Loss: Categorical crossentropy

---

## ▶️ Run Instructions

1. Clone the repo
2. Run all cells in `Main.ipynb` (or step-by-step)
3. Use `predict_caption(image_path)` to test on new images

---

## 📧 Submission Notes

- Compressed versions of data files are included for easy upload:
  - `next_words_compressed.npz`
  - `train_encoded_images_subset.pkl.gz`

