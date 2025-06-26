# Week-2

## 🏗️ Model Architecture

- **Base:** EfficientNetV2B0 (pretrained on ImageNet)
- **Custom Head:**
  - `GlobalAveragePooling2D`
  - `Dropout (rate=0.2)`
  - `Dense (Softmax activation for 10 classes)`
- **Training Config:**
  - Optimizer: `Adam (lr=0.0001)`
  - Loss: `SparseCategoricalCrossentropy`
  - Metric: `Accuracy`
  - Epochs: `15`
  - Early Stopping: `patience=3`, `restore_best_weights=True`

---

## 📈 Evaluation Metrics 

- ✅ **Training Accuracy:** 0.9864
- ✅ **Validation Accuracy:** 0.9567
- ✅ **Test Accuracy:** 0.9433
- ✅ **Test Loss:** 0.1627
- ✅ **F1 Scores:** 0.94
