# Overview

This repository is a collection of the latest deepfake detection methods 2024.

## Fully Generated AI Content vs. Manipulated Originals (Deepfakes): Key Differences and Applications

### 1. **Fully Generated AI Content**

These are created **entirely from scratch** using AI algorithms, without any real-world original footage or media. The most common technique used for fully generated content is Generative Adversarial Networks (GANs), which can produce highly realistic media that never existed.

### 2. **Manipulated Originals or Deepfakes**

These involve **modifying real existing media** (e.g., video, images, or audio) to make it appear altered. AI is used to change specific elements within the original media while keeping the core content intact.


### **Main Differences**:

| **Aspect**                | **Fully Generated AI Deepfakes**                                    | **Manipulated Originals**                                      |
|---------------------------|---------------------------------------------------------------------|----------------------------------------------------------------|
| **Source Material**        | No original source; everything is generated from scratch by AI.     | Based on real, existing media (images, videos, audio).         |
| **Realism**                | Completely synthetic; may look real but depicts imaginary people or scenes. | Realistic but altered versions of real people or events.       |
| **Creation Process**       | Generated by training models to create entirely new faces, voices, etc. | AI is used to manipulate specific aspects of real footage.     |
| **Usage**                  | Often for creating fictional characters, avatars, or synthetic media. | Commonly used for misinformation, face-swapping, or voice dubbing. |
| **Detectability**          | Can be easier to detect because the people depicted don’t exist.    | Harder to detect as it builds on real-world footage, making it more believable. |
| **Flexibility**            | Offers more creative freedom as it doesn’t rely on real-world limitations. | Limited to the original source material and its manipulation.   |


## Manipulated Original, Deepfakes

Deepfakes come in several different forms, based on the type of manipulation and the media format being altered. These are the most common types of deepfakes:

### 1. **Video Deepfakes**
   - **Face-Swapping**: This is the most well-known type of deepfake, where the face of one person in a video is swapped with another person's face. AI algorithms can map the facial expressions and movements from one person onto another, making it look like someone is saying or doing things they never did.
   - **Lip-Syncing**: In this type, the facial movements, especially around the mouth, are altered to match a new audio track, giving the impression that a person is saying something completely different from the original recording.
   - **Full-Body Deepfakes**: These deepfakes modify not just the face but also the entire body of a person in a video. The AI can replicate someone’s gestures, posture, and body movements.

### 2. **Audio Deepfakes**
   - **Voice Mimicking/Cloning**: Using audio data, deepfake technology can create a synthetic version of a person’s voice. This can be used to make the person appear to say things they never actually said. It’s often used in combination with video deepfakes but can also exist as standalone voice recordings.
   - **Text-to-Speech (TTS) Deepfakes**: AI-generated voices based on a person’s speech patterns. These systems take text input and produce audio output in the style of a particular individual’s voice, often indistinguishable from the real thing.

### 3. **Image Deepfakes**
   - **Face-Morphing**: This technique blends the facial features of two or more people in images to create a composite that looks like multiple individuals. This is often used in fake ID creation or social media account impersonation.
   - **Face Aging or De-Aging**: AI can modify the age of a person in an image, making them look significantly older or younger, which is often used in media, film, and entertainment.

### 4. **Text Deepfakes**
   - **AI-Generated Text**: This is not a typical deepfake, but text-based deepfakes involve AI tools that can generate misleading or fabricated articles, comments, or posts, mimicking the writing style of specific individuals or news outlets to manipulate opinions.

### 5. **3D Deepfakes (Holograms & Avatars)**
   - **Digital Avatars**: In some cases, deepfakes go beyond just videos and are used to create 3D avatars or holograms of individuals that can be controlled in real-time. These avatars can be used in virtual worlds, video games, or even live broadcasts.
   - **Holographic Deepfakes**: These are more advanced 3D projections where a deepfake version of someone can appear as a hologram in real-world environments, often used in performances or public events.

### 6. **Interactive Deepfakes (AI Companions)**
   - **AI Chatbots and Virtual Assistants**: These deepfakes involve creating interactive AI entities that can mimic a real person's voice, behavior, or personality in a conversation e.g. chat. This is an evolving area where deepfake technology and AI-driven virtual companions or assistants merge.

Each type of deepfake can be used for different purposes, ranging from entertainment and satire to harmful misinformation, identity theft, or political manipulation. As the technology advances, the lines between what’s real and what’s fake become harder to discern, raising ethical and legal concerns.

## Detecting Deepfakes: a Collection of Papers & Code 2024

| Paper Name                                                                                       | Publication Date | Method Name                                     | Detection Modality | Feature Modality      | Supervised/Unsupervised     | Code                                                                 |
| ------------------------------------------------------------------------------------------------ | ---------------- | ----------------------------------------------- | ------------------ | --------------------- | --------------------------- | -------------------------------------------------------------------- |
| Faster Than Lies: Real-time Deepfake Detection using Binary Neural Networks                      | 2024             | Binary Neural Networks (BNNs)                   | Image              | Frequency and Texture | Supervised [Lanzino, 2024]  | https://github.com/fedeloper/binary_deepfake_detection              |
