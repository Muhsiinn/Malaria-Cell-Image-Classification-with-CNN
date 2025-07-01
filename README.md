🖼 Dataset
Source: NIH Malaria Dataset

27,558 images (equal number of Parasitized and Uninfected samples)

Images are cell-level and labeled as:

0: Uninfected

1: Infected

🧱 Model Architecture
Input: 64x64 RGB images

Conv2D + ReLU + MaxPooling2D (x3)

Flatten → Dense(64) → Dense(1) with sigmoid activation

Loss: binary_crossentropy

Optimizer: adam

🎯 Accuracy
Training accuracy: ~94.8%

Validation accuracy: ~94.6%

Model generalizes well with no visible overfitting

🧪 How It Works
Images are loaded and resized to 64x64

Normalized to range [0, 1]

Labels assigned: 1 for infected, 0 for uninfected

Model trained using model.fit()

Tested on individual unseen images

