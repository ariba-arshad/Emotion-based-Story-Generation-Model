# Emotion-based Story Generation Model

---
## Introduction
Storytelling is a fundamental part of human culture and communication. With advancements in natural language processing (NLP), there is potential to revolutionize storytelling by automating the creation of narratives.  

This project combines a **fine-tuned GPT-2 model** (achieving **92.85% accuracy** in emotion classification) with **Gemini-1.5-Flash-Latest** to generate **emotionally resonant, family-friendly stories**. By leveraging **prompt engineering** and **model integration**, we ensure **coherent, engaging, and structured narratives** tailored to user-specified emotions.  

---
## Problem Statement
Manually crafting emotionally engaging and personalized stories requires significant time, effort, and expertise. Existing automated tools often struggle with **coherence, emotional consistency, and user personalization**.  

This project aims to develop a **story generation model** that not only **automates storytelling** but also **incorporates emotion recognition**, ensuring cohesive, engaging narratives with consistent emotional tones.

---
## Dataset for Emotion Classification

  - Kaggle dataset(parulpandey/emotion-dataset) having a collection of tweets in three files (training.csv, test.csv, validation.csv)
  - two columns (text, label)
  - 16,000 rows in training.csv and 2,000 rows in both test.csv and validation.csv
  - Label column had six unique values: sadness (0), joy (1), love (2), anger (3), fear (4), surprise (5)
     
---
## Project Architecture

We used Kaggle T4 x 2 GPU to fine-tune the model. The pipeline consists of:
1. **Emotion Classification Model (GPT-2 Fine-Tuned)**
   - Classifies user input into emotional categories with **92.85% accuracy**
   - Helps guide story development based on detected emotions  

2. **Story Generation Model (Gemini-1.5-Flash-Latest)**
   - Uses **structured prompt engineering** for high-quality, coherent stories  
   - Generates **family-friendly, engaging narratives** tailored to emotions  

3. **Integration Layer**
   - Ensures smooth interaction between emotion recognition and story generation  
   - Maintains **consistency in tone, mood, and storytelling structure**  

---
## Technologies Used
- **Natural Language Processing (NLP)**
- **Machine Learning & AI (GPT-2 & Gemini-1.5-Flash-Latest)**
- **Prompt Engineering**
- **Python (Flask, TensorFlow/PyTorch)**

---
## How It Works
1. **User Input** → User provides a prompt or theme for the story  
2. **Emotion Detection** → The GPT-2 model classifies the input's emotional tone  
3. **Story Generation** → Gemini-1.5 generates a structured, family-friendly story  
4. **Refinement** → Prompt engineering ensures coherence & emotional consistency  
5. **Output** → The final story is delivered to the user  
