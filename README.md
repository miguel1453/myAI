# Don Mike - Los Portales Supermarket AI Assistant

[![Live Demo](https://img.shields.io/badge/Vercel-Live%20Demo-blue)](https://my-ai-lilac.vercel.app/)

## Overview
**Don Mike** is an AI chatbot built for employees at Los Portales Supermarket. It answers questions about the employee handbook and assists with complex customer inquiries, like “I don’t have papers but I want a license.” Many customers are undocumented or unfamiliar with U.S. systems, and Don Mike centralizes our knowledge to empower employees to respond without needing to call the owner or a specialist.

- **Purpose**: Provide instant access to handbook info and customer guidance.  
- **Target Audience**: Los Portales Supermarket employees.  
- **Tone**: Grumpy, direct, and comedic—modeled after my dad’s no-nonsense style.

Live demo: [https://my-ai-lilac.vercel.app/](https://my-ai-lilac.vercel.app/)

## Features
- **Knowledge Base**: Answers drawn from 6 curated documents (employee handbook, government guides).  
- **RAG**: Uses Retrieval-Augmented Generation to fetch relevant info.  
- **Personality**: Direct and slightly mean, with a humorous edge.

## Knowledge Base
The current dataset includes 6 text files sourced from:  
- *Manual del Miembro del Equipo de Los Portales Supermarket* (employee handbook).  
- *Carolina del Norte Guía sobre Huracanes*.  
- *Emergency Guide for Immigrant Families*.  
- *NC Driver Handbook Spanish*.  
- *Integrated Care Rounds: Serving Families with Mixed Immigration Statuses*.  
- *Small Business Resource Guide*.  

**Curation**: PDFs, PPTs, and Docs were converted to `.txt` files and uploaded to Pinecone.

## Tech Stack
- **Backend**: Built on the `myAI` framework with RAG via Pinecone.  
- **Frontend**: Deployed on Vercel.  
- **APIs**: OpenAI for generation, Pinecone for vector storage.  

## Setup (For Developers)
1. Clone the repo:  
   ```bash
   git clone https://github.com/miguel1453/myAI.git
   ```
2. Install dependencies:  
   ```bash
   npm install
   ```
3. Configure environment variables (e.g., OpenAI API key, Pinecone credentials) in `.env`.  
4. Run locally:  
   ```bash
   npm run dev
   ```
5. Deploy to Vercel: Follow the [Class 13 Async Tutorial](link-to-tutorial-if-available).

## Customization
- **Identity**: Configured in `identity.ts` (e.g., `AI_NAME: "Don Mike"`, `AI_TONE: "enojon y directo"`).  
- **Prompt**: Tweaked to be grumpy and direct: “You are Don Mike, a no-nonsense HR assistant…”  
- **Future Plans**: More personalized features incoming.

## About the Creator
**Miguel Angel**  
Hijo, hermano, amigo, y amante de la tecnología.  
This project is part of a UNC course mid-term, showcasing AI for business applications.

## License
MIT License - feel free to fork and adapt!

---
Created by Miguel Angel, March 2025
