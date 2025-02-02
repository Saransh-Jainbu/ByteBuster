# Spheron YAML (ICL) Generator

## Demo

We have temporarily disabled the chatbot feature due to monetary constraints. However, you can check out our demo video showcasing the project:

[Google Drive Demo Link](https://drive.google.com/drive/folders/17PXAFSUd2G_1uTZ9R6-0ScDzPVnAaoXi)

## Google Colab Notebook

To verify our work and understand our implementation, you can check our Google Colab notebook:

[Colab Notebook](https://colab.research.google.com/drive/1EmNPYj16DwusqdVbgIkQVPn88Tk4SmKM?usp=sharing)

## Overview

Spheron uses an Infrastructure Composition Language (ICL) in YAML to define and manage deployments. Writing YAML configurations manually can be cumbersome for developers, requiring them to memorize keys, properties, and structures. This project automates YAML generation to streamline the deployment process and make it more user-friendly.

## Goal

Automate YAML generation using Retrieval-Augmented Generation (RAG) and FAISS.

## Output

Valid YAML configuration.

## Key Components

- **FAISS**: For semantic search.
- **RAG**: For context-aware YAML generation.

## Technical Architecture

1. Load and process ICL documentation into chunks.
2. Build FAISS index for efficient similarity search.
3. Generate embeddings using Sentence Transformers.
4. Retrieve relevant chunks using FAISS.
5. Generate YAML using DeepSeek-Coder-1.3B.
6. Validate the generated YAML.

## Features

- **Automated YAML Generation**: Eliminates the need for developers to write YAML manually.
- **Validation & Error Prevention**: Ensures that the generated YAML adheres to Spheron’s ICL specifications, preventing misconfigurations.
- **Easy Iterations**: Allows users to refine or regenerate YAML configurations.

## Tech Stack

- **Frontend**: Next.js (React-based framework for fast and scalable web applications)
- **Backend**: DeepSeek-Coder-1.3B for YAML generation
- **Storage**: FAISS for efficient similarity search and retrieval
- **NLP & Embeddings**: Sentence Transformers for context-aware processing
- **Validation**: Custom validation logic to ensure YAML correctness and prevent syntax errors

## Installation & Setup

### Prerequisites

- Node.js (v16+ recommended)
- npm or yarn

### Steps

1. Clone the repository:
   ```sh
   git clone https://github.com/your-repo/spheron-icl-generator.git
   cd ByteBuster/yamlize/
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Start the development server:
   ```sh
   npm run dev
   ```
4. Open `http://localhost:3000` in your browser.

## Expected Outcomes

- **Faster onboarding** for developers who no longer need to learn Spheron ICL syntax manually.
- **Improved efficiency** by reducing time spent on YAML configuration.
- **Error-free configurations** through real-time validation and iteration.

## Contribution

Contributions are welcome! Feel free to submit issues or pull requests.

## License

MIT License
