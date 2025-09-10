# 🛡️ Adversarial Robustness in CIFAR-10

This project demonstrates how deep learning models can be fooled by adversarial attacks.  
We train a simple CNN on the CIFAR-10 dataset and evaluate its robustness against **FGSM** and **PGD** attacks using [Foolbox](https://github.com/bethgelab/foolbox).

---

## 📌 Project Overview
- **Dataset**: CIFAR-10 (60,000 images, 10 classes)
- **Model**: CNN (2 convolutional layers + 2 fully connected layers)
- **Attacks**:
  - FGSM (Fast Gradient Sign Method)
  - PGD (Projected Gradient Descent)
- **Defenses**:
  - Baseline model (no defense)
  - Adversarial training (FGSM-based)

---

## 📂 Files
- `adversarial_robustness_cifar10.ipynb` → Main Colab notebook with training, attacks, and defenses
- `requirements.txt` → Dependencies (PyTorch, Torchvision, Foolbox, Matplotlib)

---

## 🚀 Results

- **Clean Test Accuracy**: ~72%  
- **Attack Success Rates**:
  - FGSM: ~83%  
  - PGD: ~92%  

---

## 🎨 Visualizations
- Training loss curve  
- Clean vs. adversarial images (FGSM & PGD)  
- Perturbation heatmap  

---

## 📝 Conclusion
- CNNs are **highly vulnerable** to adversarial attacks.  
- Even small, imperceptible changes can cause massive misclassification.  
- Adversarial training improves robustness, but with a trade-off in clean accuracy.  
- Future work: stronger defenses (certified robustness, preprocessing defenses, robust architectures).  

---
