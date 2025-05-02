# miniproject

# 🧠 Evaluating the Robustness of Image Captioning LLMs against Adversarial Attacks

This repository contains the implementation and evaluation code for assessing how well large language models (LLMs) like BLIP-2 and GIT perform on image captioning tasks, especially under adversarial attacks. We use clean and attacked images to generate and compare captions.

---

## 📁 Repository Structure


```text
your-repo/
│
├── single_image_inference/
│   └── BLIP-2.ipynb
│   └── Hybrid.ipynb
│   └── pali.ipynb
|   └── git.ipynb
│
├── batch_dataset_inference/
│   └── BLIP-2.ipynb
│   └── Hybrid.ipynb
│   └── pali.ipynb
|   └── git.ipynb
│
├── output_json/
│   └── BLIP-2.json
│   └── Hybrid.json
│   └── pali.json
|   └── git.json
|── Robustness.ipynb
|── performance.txt
|── Report.pdf
|── miniproject.pdf
```


---

## 🔍 Folders Description

### `single_image_inference/`
Contains notebooks that demonstrate how each model performs captioning on a **single image**, both clean and adversarially attacked.

### `batch_dataset_inference/`
Includes scripts to generate captions over **entire datasets** using various LLMs and apply adversarial attacks like FGSM, PGD, DeepFool, BIM, and AutoAttack.

### `output_json/`
Stores `.json` files that hold the **original and attacked captions**, along with image IDs and evaluation metrics such as BLEU, METEOR, and BERTScore.

---

## 🧪 Models Used

- **BLIP-2**
- **GIT (Generative Image-to-Text)**
- **ViT-GPT2**
- **Pali**
- **Hybrid (BLIP-2 + GIT)**

---

## ⚔️ Adversarial Attacks Applied

- **FGSM (Fast Gradient Sign Method)**
- **PGD (Projected Gradient Descent)**
- **DeepFool**
- **AutoAttack**
- **C&W, BIM, JSMA, One Pixel**
- **Trigger & Universal Patch Attacks**

---

## 📊 Evaluation Metrics

We used the following standard NLP metrics to measure caption quality:

- **BLEU**
- **METEOR**
- **BERTScore**

These scores are stored in the `output_json/` folder for both original and attacked cases.

---

## 💻 Technologies

- PyTorch, Hugging Face Transformers
- Torchvision, Pillow, Matplotlib
- NLTK, pycocoevalcap, BERTScore
- JSON, NumPy, tqdm
- Google Colab for GPU support

---

## 📚 Dataset

- **Flickr8k** – used for evaluating captioning robustness under adversarial perturbations.

---

## 🤝 Authors

- V. Madhu Sree (N200806)
- K. Swathi (N200774)
- P.N.P. Asritha (N200621)
- G. Sathish Roy (N200298)
- N. Abhiram Naidu (N200211)

---

## 📌 Objective

To analyze how well image captioning models can handle subtle, adversarial changes and still generate meaningful captions, which is crucial in safety-critical applications like healthcare, autonomous driving, and content moderation.

---

## 📎 References

- [Awesome LVLM Attack Resources](https://github.com/liudaizong/Awesome-LVLM-Attack)
- [Flickr8k Dataset](https://github.com/jbrownlee/Datasets/releases/tag/Flickr8k)
- [Understanding Adversarial Attacks on LVLMs (arXiv:2312.03777)](https://arxiv.org/pdf/2312.03777)

---

