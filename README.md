# Final_project
# Personalized Video Generation

This project automates the creation of **educational videos** using **Generative AI**. Users can input any query (e.g., "Explain Pythagoras Theorem"), and the system generates:
- A relevant explanation using Google Gemini (Generative AI),
- AI-generated images with Stable Diffusion,
- Voice narration with gTTS (Text-to-Speech),
- A complete video using MoviePy,
- A quiz based on the video with answer evaluation using Sentence Transformers.

### 🔍 Use Case
- Personalized learning content
- Rapid creation of explainer videos
- Interactive educational tools

---

## 🛠️ Features

✅ Accepts any user query on a topic  
✅ Option to choose **Focus** (Theory / Application / General)  
✅ Option to choose **Duration** (1–3 minutes)  
✅ Generates:
- Detailed explanation (via Gemini)
- Image prompts for each scene
- AI visuals using Stable Diffusion
- Text-to-speech audio (gTTS)
- Merged video with MoviePy

✅ Bonus: Asks a **quiz question** based on the video explanation and evaluates your answer using **semantic similarity** (SentenceTransformers)

---

## 📦 Tech Stack

| Module              | Tool / Library                          |
|---------------------|-----------------------------------------|
| LLM (Text Gen)      | Google Gemini API                       |
| Visual Generation   | Stable Diffusion (via Diffusers)        |
| Text-to-Speech      | gTTS (Google Text-to-Speech)            |
| Video Creation      | MoviePy                                 |
| Answer Evaluation   | Sentence Transformers (Cosine Similarity) |
| Frontend            | Streamlit (for user interface)          |

---

## 🧠 AI Workflow

1. **Text Explanation**:  
   Gemini generates a structured explanation for the topic.

2. **Prompt Engineering**:  
   The explanation is turned into **visual prompts** for each scene.

3. **Image Generation**:  
   Each prompt is fed into **Stable Diffusion** to generate matching visuals.

4. **Voice Generation**:  
   The explanation is converted into **audio using gTTS**.

5. **Video Creation**:  
   Images + Voice + Captions combined using **MoviePy**.

6. **Quiz Creation & Evaluation**:  
   - Gemini generates a quiz question.  
   - User answers it.  
   - Score is calculated using **semantic similarity**.

---
