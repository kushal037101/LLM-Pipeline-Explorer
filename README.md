# LLM Pipeline Explorer 2.0
An interactive, modern educational platform for exploring how Large Language Models work internally.

Live Demo: https://llm-pipeline-explorer-newton-64f0.vercel.app

## Features Overview

1. **Tokenization Lab**
   - Live subword tokenization (BPE & WordPiece approximation)
   - Real-time token highlighting and color-coded chips
   - Token inspector (Token ID, byte breakdown, unicode points, category)
   - Dynamic vocabulary compression slider
   - Strategy comparison: BPE (GPT-style) vs WordPiece (BERT-style) vs Character-level vs Word-level
   - Token statistics: character count, word count, token count, compression ratio, estimated cost

2. **Embedding Galaxy (3D Semantic Space)**
   - Interactive 3D vector space (Three.js WebGL with offline Canvas 3D fallback)
   - 7 semantic clusters: Animals, Technology, Programming, Emotions, Food, Science, Royalty
   - Interactive analogies: "King - Man + Woman = Queen" vector math visualization
   - Nearest-neighbor search with cosine similarity connection rays
   - Custom word & sentence embedding projection
   - Search, auto-rotate, cluster filtering, and PCA dimensionality reduction explanations

3. **Vector Space Explorer**
   - 2D/3D interactive coordinate plane with draggable vector arrowheads
   - Live cosine similarity calculator with angle $\theta$ arc and visual gauge
   - Vector arithmetic playground: Addition, Subtraction, Interpolation
   - Distance metrics: Cosine Similarity, Dot Product, Euclidean ($L_2$) Distance, Manhattan ($L_1$) Distance

4. **Attention Mechanism Visualizer**
   - Interactive token-to-token Attention Graph with glowing connection arcs
   - Multi-Head Attention selector (Syntactic, Coreference, Semantic, Positional)
   - Interactive $N \times N$ Attention Matrix Heatmap
   - Step-by-step Query, Key, Value (QKV) mathematical breakdown
   - Coreference resolution demonstration (e.g. "The cat sat on the mat because it was tired")

5. **Transformer Architecture**
   - Interactive blueprint of the modern Decoder-only Transformer stack
   - Clickable components: Tokenizer, Embeddings, RoPE, Multi-Head Attention, RMSNorm, SwiGLU MLP, LM Head, Softmax
   - Live forward-pass simulation with animated data pulses
   - Tensor dimension tracking and mathematical formulas at every stage

6. **LLM Playground**
   - Realistic token-by-token inference simulator
   - Parameter controls: Temperature (0.0 to 2.0), Top-P (0.1 to 1.0), Top-K, Max Tokens, System Prompt
   - Real-time Top-5 candidate token probability distribution chart at each generation step
   - Token usage counter (Prompt, Completion, Total)

7. **What-If Engine & Experiments**
   - Side-by-side sentence comparison (Sentence A vs Sentence B)
   - Diff analysis: Shared tokens, Added tokens, Removed tokens
   - Vector distance and cosine similarity meter
   - Dynamic natural language semantic insight generator
   - 6 Interactive Presets: Synonyms, Meaning Shift, Opposites, Token Explosion, Sentence Length, Semantic Distance

8. **AI Glossary & Knowledge Quizzes**
   - Comprehensive searchable dictionary of LLM terminology
   - Interactive self-test quizzes with instant feedback and scoring
   - Global **Beginner 💡 / Engineer ⚙️** mode toggle that updates explanations application-wide

## How to Run

Simply open `index.html` in any modern web browser:
```bash
# Direct browser opening
open index.html

# Or with a local web server (optional)
python3 -m http.server 8080
```
No build process, npm install, or external API keys are required.

