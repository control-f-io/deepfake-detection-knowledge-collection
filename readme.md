# Overview

This repository is a collection of the latest deepfake detection methods 2024.


## I. Fully Generated AI Content vs. Manipulated Originals (Deepfakes): Key Differences and Applications

### I.1. **Fully Generated AI Content**

These are created **entirely from scratch** using AI algorithms, without any real-world original footage or media. The most common technique used for fully generated content is Generative Adversarial Networks (GANs), which can produce highly realistic media that never existed.

---


### I.2. **Manipulated Originals or Deepfakes**

These involve **modifying real existing media** (e.g., video, images, or audio) to make it appear altered. AI is used to change specific elements within the original media while keeping the core content intact.

#### **Main Differences**:

| **Aspect**                | **Fully Generated AI Deepfakes**                                    | **Manipulated Originals**                                      |
|---------------------------|---------------------------------------------------------------------|----------------------------------------------------------------|
| **Source Material**        | No original source; everything is generated from scratch by AI.     | Based on real, existing media (images, videos, audio).         |
| **Realism**                | Completely synthetic; may look real but depicts imaginary people or scenes. | Realistic but altered versions of real people or events.       |
| **Creation Process**       | Generated by training models to create entirely new faces, voices, etc. | AI is used to manipulate specific aspects of real footage.     |
| **Usage**                  | Often for creating fictional characters, avatars, or synthetic media. | Commonly used for misinformation, face-swapping, or voice dubbing. |
| **Detectability**          | Can be easier to detect because the people depicted don’t exist.    | Harder to detect as it builds on real-world footage, making it more believable. |
| **Flexibility**            | Offers more creative freedom as it doesn’t rely on real-world limitations. | Limited to the original source material and its manipulation.   |

<br>

---

---

## II.Manipulated Original, Deepfakes

Deepfakes come in several different forms, based on the type of manipulation and the media format being altered. These are the most common types of deepfakes:

### II.1. **Video Deepfakes**
   - **Face-Swapping**: This is the most well-known type of deepfake, where the face of one person in a video is swapped with another person's face. AI algorithms can map the facial expressions and movements from one person onto another, making it look like someone is saying or doing things they never did.
   - **Lip-Syncing**: In this type, the facial movements, especially around the mouth, are altered to match a new audio track, giving the impression that a person is saying something completely different from the original recording.
   - **Full-Body Deepfakes**: These deepfakes modify not just the face but also the entire body of a person in a video. The AI can replicate someone’s gestures, posture, and body movements.

---

### II.2. **Audio Deepfakes**
   - **Voice Mimicking/Cloning**: Using audio data, deepfake technology can create a synthetic version of a person’s voice. This can be used to make the person appear to say things they never actually said. It’s often used in combination with video deepfakes but can also exist as standalone voice recordings.
   - **Text-to-Speech (TTS) Deepfakes**: AI-generated voices based on a person’s speech patterns. These systems take text input and produce audio output in the style of a particular individual’s voice, often indistinguishable from the real thing.

---

### II.3. **Image Deepfakes**
#### <u>*II.3.1 Papers*</u>:

| Paper Name                                                                        | Publication Date | Method Name                      | Detection Modality                      | Feature Modality                     | Supervised/Unsupervised | Code                                                                                      |
|-----------------------------------------------------------------------------------|------------------|-----------------------------------|----------------------------------------|--------------------------------------|------------------------|-------------------------------------------------------------------------------------------|
| TruFor: Leveraging All-Round Clues for Trustworthy Image Forgery Detection         | CVPR 2023        | TruFor                           | Image Forgery Detection & Localization | High-level and low-level features    | Supervised             | https://github.com/grip-unina/TruFor                                                       |
| Hierarchical Fine-Grained Image Forgery Detection and Localization                | CVPR 2023        | HiFi-Net                         | Image Forgery Detection & Localization | Multi-scale high-frequency features  | Supervised             | https://github.com/CHELSEA234/HiFi_IFDL                                                    |
| Generalizing Face Forgery Detection with High-Frequency Features                  | CVPR 2021        | High-frequency feature extraction | Face Forgery Detection                 | High-frequency and low-level textures| Supervised             | No Code                                                                                   |
| Towards Universal Fake Image Detectors That Generalize Across Generative Models   | CVPR 2023        | Nearest Neighbor, Linear Probing  | Real vs. Fake Classification           | Vision-Language Model Features       | Supervised           | https://github.com/WisconsinAIVision/UniversalFakeDetect                                   |
| Fake It Till You Make It: Learning Transferable Representations                   | CVPR 2023        | Transferable Representations      | ImageNet Classification                | Synthetic Images (Stable Diffusion)  | Supervised             | https://europe.naverlabs.com/research/computer-vision/imagenet-sd/#pretrained-models       |
| Learning on Gradients: Generalized Artifacts Representation                       | CVPR 2023        | LGrad                            | GAN-generated Image Detection          | Gradient-based feature extraction    | Supervised             | https://github.com/chuangchuangtan/LGrad                                                   |

#### <u>*3.2 Glossary*</u>:

- ***Datasets***:

  - **HiFi-IFDL Dataset**: <br> A dataset for fine-grained forgery detection, with CNN-based synthetic images and forgery masks.
<br>

  - **CelebA-HQ**: <br> High-quality version of CelebA, featuring celebrity face images used in manipulation detection.
<br>

  - **LSUN**: <br> Dataset with various object categories like scenes and vehicles.
<br>

  - **ImageNet**: <br> Large-scale image classification dataset. The ImageNet-1K subset includes 1,000 classes.
<br>

  - **ImageNet Clone (ImageNet-SD)**: <br> Synthetic dataset mimicking ImageNet, generated by models like Stable Diffusion.
<br>

  - **CoG Benchmark**: <br> Dataset for testing concept generalization in visual representation models.
<br>

  - **CelebA-Spoof**: <br> Dataset designed for face anti-spoofing tasks.

<br>

- ***Models and Architectures***:

  - **CNN**: <br> Neural network architecture designed for processing images.
<br>

  - **Xception Model**: <br> Efficient CNN architecture developed by Google.
<br>

  - **ResNet/ResNet50**: <br> CNN architecture using residual connections to improve training in deep networks.
<br>

  - **GAN (Generative Adversarial Network)**: <br> Model used for generating realistic synthetic images.
<br>

  - **ProGAN**: <br> GAN architecture designed for generating high-quality images.
<br>

  - **StyleGAN/StyleGAN2**: <br> GAN models known for producing realistic, high-quality images.
<br>

  - **Vision Transformer (ViT)**: <br> Transformer-based model adapted for image classification tasks.
<br>

  - **CycleGAN**: <br> GAN used for image-to-image translation without paired training data (eg. style transfer).
<br>

  - **BigGAN**: <br> GAN architecture for generating diverse, high-quality images.
<br>

  - **Latent Diffusion Model (LDM)**: <br> Diffusion model that refines noisy inputs to generate clear images.
<br>

  - **Autoencoder**: <br> Neural network for efficient encoding, often used in synthetic image generation.
<br>

  - **SegFormer**: <br> Transformer-based architecture for semantic segmentation, adapted for forgery localization.
<br>

  - **HiFi-Net**: <br> Hierarchical network for detecting and classifying forgery attributes at different resolutions.
<br>

  - **Frozen Network**: <br> Pre-trained model whose weights remain fixed during training (eg. CLIP for feature extraction).
<br>

  - **Patch-Level Classification**: <br> Divides images into smaller patches to classify regions as real or fake.

<br>

- ***Neural Network Components and Mechanisms***:

  - **Attention Mechanism**: <br> Focuses on important regions of input data to improve learning.
<br>

  - **Channel-Wise Attention**: <br> Emphasizes or suppresses specific features within channels.
<br>

  - **Self-Attention**: <br> Computes relationships between different parts of an image to enhance focus.
<br>

  - **Residual Connection**: <br> Shortcut connection that helps pass information across layers in deep networks.
<br>

  - **Pooling Layer/Block**: <br> Downsamples feature maps or combines local features into global representations.
<br>

  - **Anomaly Map**: <br> Highlights unusual areas in an image that may indicate manipulation.
<br>

  - **Anomaly Localization Map**: <br> Pixel-level map showing regions of manipulation within an image.
<br>

  - **Residual-Guided Spatial Attention**: <br> Highlights important spatial regions by using residual information.

<br>

- ***Attention and Fusion Modules***:

  - **Cross-Modality Attention**: <br> Models interactions between different data types (eg. RGB images and noise maps).
<br>

  - **Dual Cross-Modality Attention (DCMA)**: <br> Captures correlations between RGB images and high-frequency noise maps.
<br>

  - **Cross-Modal Fusion**: <br> Combines information from different modalities to improve detection.
<br>

  - **Cross-Modal Feature Rectification**: <br> Adjusts features from different modalities to enhance detection performance.
<br>

  - **Residual-Guided Feature Fusion**: <br> Fuses residual and spatial features to improve detection accuracy.

<br>

- ***Image Processing and Feature Extraction****:

  - **Feature Fusion**: <br> Combines multiple feature sets (eg. RGB and high-frequency features).
<br>

  - **Multi-Scale Feature Extraction**: <br> Captures image details at different scales to enhance detection.
<br>

  - **High-Frequency Features**: <br> Sharp changes in brightness or color used to detect forgeries.
<br>

  - **Low-Level Features**: <br> Basic image elements like edges and textures.
<br>

  - **Mesoscopic Features**: <br> Intermediate features used to detect tampering.
<br>

  - **Gradient-Based Features**: <br> Extracted from image gradients to highlight key areas distinguishing real from fake.
<br>

  - **Generalized Artifact Representation**: <br> Captures artifacts from generative models for generalized forgery detection.
<br>

  - **Steganalysis Features**: <br> Derived from noise patterns in images, used to detect manipulations.

<br>

- ***Image Manipulation and Forgery Techniques***:

  - **Face Blending**: <br> Merging a fake face with a real image, often leaving blending artifacts.
<br>

  - **Splicing**: <br> Copying and pasting sections from one image to another.
<br>

  - **Fully Synthesized**: <br> Forgery where the entire image is generated, with no real image content.
<br>

  - **Forgery Trace**: <br> Artifacts or inconsistencies in manipulated faces used for detection.
<br>

  - **Image Laundering**: <br> Modifying an image (e.g., resizing, recompression) to reduce the chance of detection.
<br>

  - **Cheapfakes**: <br> Basic image manipulations created using conventional tools (e.g., splicing), not deep learning.

<br>

- ***Image Analysis in the Frequency Domain***:

  - **DCT (Discrete Cosine Transform)**: <br> Converts spatial data into frequency domain for forgery analysis.
<br>

  - **Frequency Domain Analysis**: <br> Analyzes image frequency components to detect manipulations.
<br>

  - **Fourier Transform**: <br> Transforms data into frequency domain to reveal hidden artifacts.
<br>

  - **High-Pass Filter**: <br> Removes low-frequency components, emphasizing high-frequency details.
<br>

  - **Laplacian of Gaussian (LoG)**: <br> Edge detection method used to enhance forgery traces.

<br>

- ***Detection and Generalization Techniques***:

  - **Cross-Database Detection**: <br> Model trained on one database and tested on another.
<br>

  - **Cross-Domain Generalization**: <br> Detects fake images across different domains or categories.
<br>

  - **Cross-Model Detection**: <br> Detects manipulations created by different generative models.
<br>

  - **Nearest Neighbor Classification**: <br> Classifies images based on their closest neighbors in feature space.
<br>

  - **Noise Refinement**: <br> Process in diffusion models that progressively removes noise during image generation.

<br>

- ***Evaluation Metrics and Loss Functions***:

  - **AUC (Area Under the Curve)**: <br> Measures model performance based on true and false positives.
<br>

  - **Average Precision (AP)**: <br> Summarizes precision-recall trade-offs across thresholds.
<br>

  - **Binary Cross-Entropy Loss**: <br> Measures the difference between predicted and actual class labels in binary classification.
<br>

  - **Weighted Cross-Entropy Loss**: <br> Assigns different weights to classes for better balance.
<br>

  - **Dice Loss**: <br> Measures overlap between predicted segmentation and ground truth.
<br>

  - **InfoNCE Loss**: <br> Contrastive learning loss function used to learn useful representations.
<br>

  - **Oracle Accuracy**: <br> Upper-bound accuracy of a model when the decision threshold is optimized on test data.

<br>

- ***Post-Processing and Artifacts***:

  - **Post-Processing**: <br> Operations applied to images after creation which introduce detectable artifacts.
<br>

  - **Blending Artifacts**: <br> Inconsistencies at boundaries between synthetic and real regions.
<br>

  - **JPEG Artifacts**: <br> Compression artifacts like blockiness, which are helpful in forgery detection.

<br>

- ***Tools for Forensic Detection***:

  - **SRM (Steganalysis Rich Model) Filters**: <br> Extract high-frequency noise from images to detect subtle inconsistencies.
<br>

  - **Noiseprint**: <br> Noise fingerprint used to detect inconsistencies in camera-origin data.
<br>

  - **Noiseprint++**: <br> Enhanced version of Noiseprint for more robust detection.
<br>

  - **Bayesian Neural Networks**: <br> Provide uncertainty estimates along with predictions.
<br>

  - **Confidence Map**: <br> Map indicating the reliability of predictions to reduce false positives.

<br>

- ***Other Concepts and Techniques***:

  - **Grad-CAM**: <br> Generates visual explanations by highlighting important regions for model predictions.
<br>

  - **Linear Probing**: <br> Evaluates learned features by training a simple classifier on frozen feature representations.
<br>

  - **Self-Supervised Learning**: <br> Model learns from data without explicit labels.
<br>

  - **Transfer Learning**: <br> Applies knowledge from one task to another to improve model performance.
<br>

  - **Adversarial Examples**: <br> Intentionally manipulated inputs designed to deceive machine learning models.

<br>
<br>

---


### II.4. **Text Deepfakes**
   - **AI-Generated Text**: This is not a typical deepfake, but text-based deepfakes involve AI tools that can generate misleading or fabricated articles, comments, or posts, mimicking the writing style of specific individuals or news outlets to manipulate opinions.

---

### II.5. **3D Deepfakes (Holograms & Avatars)**
   - **Digital Avatars**: In some cases, deepfakes go beyond just videos and are used to create 3D avatars or holograms of individuals that can be controlled in real-time. These avatars can be used in virtual worlds, video games, or even live broadcasts.
   - **Holographic Deepfakes**: These are more advanced 3D projections where a deepfake version of someone can appear as a hologram in real-world environments, often used in performances or public events.

---

### II.6. **Interactive Deepfakes (AI Companions)**
   - **AI Chatbots and Virtual Assistants**: These deepfakes involve creating interactive AI entities that can mimic a real person's voice, behavior, or personality in a conversation e.g. chat. This is an evolving area where deepfake technology and AI-driven virtual companions or assistants merge.

Each type of deepfake can be used for different purposes, ranging from entertainment and satire to harmful misinformation, identity theft, or political manipulation. As the technology advances, the lines between what’s real and what’s fake become harder to discern, raising ethical and legal concerns.

---
---

## III.Collection of Papers & Code 2024

| Paper Name                                                                                       | Publication Date | Method Name                                     | Detection Modality | Feature Modality      | Supervised/Unsupervised     | Code                                                                 |
| ------------------------------------------------------------------------------------------------ | ---------------- | ----------------------------------------------- | ------------------ | --------------------- | --------------------------- | -------------------------------------------------------------------- |
| Faster Than Lies: Real-time Deepfake Detection using Binary Neural Networks                      | 2024             | Binary Neural Networks (BNNs)                   | Image              | Frequency and Texture | Supervised [Lanzino, 2024]  | https://github.com/fedeloper/binary_deepfake_detection              |
