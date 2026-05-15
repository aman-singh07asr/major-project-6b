
# Artify – AI Text-to-Image Generation Service

## Overview
Artify is a modern AI-powered text-to-image generation web application built using:
- FastAPI (Backend)
- Stable Diffusion XL
- HuggingFace Diffusers
- React + Tailwind CSS (Frontend)
- CUDA GPU Support
- Image History Gallery

The project allows users to:
- Enter prompts
- Generate AI images
- Download images
- View generation history
- Demonstrate AI image generation in real time

---

## Features
- Beautiful modern UI
- AI-generated images using Stable Diffusion
- FastAPI backend API
- Prompt history
- Download generated image
- Teacher-friendly architecture
- Easy deployment

---

## Recommended Hardware
Minimum:
- RTX 3060 (6GB+ VRAM)
- 16GB RAM

Recommended:
- RTX 4060 / 4070 / 4080

---

## Project Structure

artify_project/
├── backend/
├── frontend/
├── docs/
├── requirements.txt

---

## How To Run

### 1. Create Virtual Environment

```bash
python -m venv venv
```

### 2. Activate Environment

Windows:
```bash
venv\Scripts\activate
```

Linux/Mac:
```bash
source venv/bin/activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Start Backend

```bash
cd backend
uvicorn main:app --reload
```

Backend runs at:
http://127.0.0.1:8000

### 5. Start Frontend

Open new terminal:

```bash
cd frontend
npm install
npm run dev
```

Frontend runs at:
http://localhost:5173

---

## Real Life Demonstration

Example prompts:
- "Cyberpunk city at night"
- "Indian village in monsoon"
- "Futuristic BMW bike in neon lights"
- "AI professor teaching robots"

Explain to professor:
1. User enters text prompt
2. Frontend sends request to backend
3. Stable Diffusion model converts text into latent embeddings
4. Diffusion process generates image step-by-step
5. Image returned to frontend
6. User downloads/generated image

---

## Future Improvements

- Voice-to-image generation
- AI image editing
- Video generation
- Fine-tuning on custom datasets
- Multi-language prompt support
- User accounts
- Cloud deployment
- Real-time collaborative generation
- Image-to-image generation
- AI safety filtering

---

## How AI Works Internally

Stable Diffusion uses:
- Transformer text encoder
- U-Net diffusion model
- Variational Autoencoder (VAE)

Steps:
1. Prompt converted into embeddings
2. Noise generated
3. AI gradually removes noise
4. Final image created

