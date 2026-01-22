# Persona-Conditioned LLM

This repository contains the complete source code and data for the "Persona-Conditioned LLM" project, divided into three main components: 
the interactive web application, the text evaluation pipeline, and the overall tool evluation materials.

# Repository Structure

capstone_final_app: Contains the source code for the "Persona Call App", a Next.js-based interactive application.
text_evaluations: Contains scripts and datasets used for evaluating Large Language Model (LLM) responses.

1. Persona Call App (capstone_final_app)
The Persona Call App is a web-based interface that simulates interactive conversations with AI personas.
It leverages a modern tech stack to provide real-time audio and text interaction.

# Tech Stack
Framework: Next.js (React)
UI/Styling: Tailwind CSS
AI Integration: OpenAI (GPT models), ElevenLabs (Text-to-Speech), Deepgram (Speech-to-Text)
Database: PostgreSQL (via Vercel/Neon)

# Getting Started
Navigate to the app directory:

cd capstone_final_app/capstone_app
Install dependencies:

npm install
Run the development server:

npm run dev
The application will be available at http://localhost:3000.

2. Text Evaluations (text_evaluations)
This directory contains the pipeline for generating, processing, and scoring text responses from various LLMs.

# Key Components

Response Generation: Scripts to fetch responses from models like Gemini, Claude, and OpenAI (process_prompts_*.py).
Data Processing: Tools to merge and format response data (merge_csv_files.py).

Scoring: The master_evaluator.py script (and related tools) that computes linguistic metrics for the generated text.
Data:
generated_prompts.csv: Input prompts.
master_scores.csv: comprehensive dataset containing model responses and their calculated scores.
