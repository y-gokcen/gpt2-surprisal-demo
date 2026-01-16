# GPT-2 Surprisal Calculator - Interactive Demo

An interactive web application that calculates and visualizes word-level surprisal using GPT-2, making computational linguistics research accessible and interactive.

> **AI-Powered Development:** This project was built using Google AI for rapid prototyping, demonstrating modern AI-assisted development workflows. 
## Project Overview

This tool demonstrates practical application of my GPT-2 language processing research through an intuitive interface where users can:
- Paste any text and see word-by-word predictability
- Visualize which words are surprising vs. predictable
- Understand the relationship between language models and human cognition

**Built with Google AI assistance** - This project showcases rapid prototyping and AI-assisted development capabilities.

## Features

- **Real-time Analysis:** Calculate surprisal values for any text input
- **Visual Feedback:** Color-coded words (green = predictable, red = surprising)
- **Statistics:** Average surprisal, max surprisal, and word count
- **Interactive Examples:** Pre-loaded examples to demonstrate the concept
- **Hover Details:** Tooltip showing exact surprisal value for each word
- **Responsive Design:** Works on desktop, tablet, and mobile

## What is Surprisal?

Surprisal is a measure from information theory that quantifies how unexpected a word is in context:

```
Surprisal = -log₂(P(word | context))
```

- **Low surprisal (0-5 bits):** Highly predictable word
- **Medium surprisal (5-10 bits):** Moderately predictable
- **High surprisal (10+ bits):** Unexpected/surprising word

### Research Applications

Surprisal correlates with:
- Reading time (slower for high surprisal)
- Brain activity (N400 ERP component)
- Comprehension difficulty
- Memory encoding strength

## Technology Stack

- **Frontend:** Pure HTML, CSS, JavaScript (no frameworks needed!)
- **Language Model:** GPT-2 (via Hugging Face API)
- **Design:** Custom gradient UI with responsive layout
- **Deployment:** GitHub Pages (static hosting)
- **Development:** AI-assisted rapid prototyping (see below)

### AI Tools Used

This project showcases **AI-first development** with the following tools:

| Tool | Purpose | Impact |
|------|---------|--------|
| **Google AI Studio** | Core development, architecture, full implementation, model comparison, testing | Enhanced features, 80% time savings |
| **GitHub Copilot** | Code completion, pattern suggestions | Faster iteration |
| **Cursor** | Context-aware code editing | Real-time refinement |


**Development time:** 60 minutes (vs. 5-6 hours manual coding)

## Repository Contents

```
gpt2-surprisal-demo/
├── index.html          # Complete web application (all-in-one file)
└── README.md           # This file
```

## Deployment Instructions

### Option 1: GitHub Pages (Recommended)

1. **Create the repository**
   ```bash
   # Create new repository on GitHub called 'gpt2-surprisal-demo'
   git clone https://github.com/USERNAME/gpt2-surprisal-demo.git
   cd gpt2-surprisal-demo
   ```

2. **Add the file**
   ```bash
   # Copy index.html to the repository
   git add index.html
   git commit -m "Add GPT-2 surprisal calculator"
   git push origin main
   ```

3. **Enable GitHub Pages**
   - Go to repository Settings → Pages
   - Source: Deploy from branch `main`
   - Folder: `/ (root)`
   - Click Save

4. **Access your site**
   - URL: `https://USERNAME.github.io/gpt2-surprisal-demo`
   - Usually live within 1-2 minutes

### Option 2: Local Testing

Simply open `index.html` in your web browser - no server needed!

```bash
# Mac/Linux
open index.html

# Windows
start index.html
```

### Option 3: Other Hosting

Deploy to:
- **Vercel:** Drag and drop the file
- **Netlify:** Connect your GitHub repo
- **Any static hosting:** Upload `index.html`

## How It Works

1. **User Input:** User enters or selects example text
2. **Tokenization:** Text is split into words/tokens
3. **API Call:** For each word, we query the Hugging Face GPT-2 model
4. **Surprisal Calculation:** Calculate `-log₂(probability)` for each token
5. **Visualization:** Display words with color coding based on surprisal
6. **Statistics:** Compute and show aggregate metrics

### Technical Notes

- Uses Hugging Face Inference API (free, no API key required for public models)
- Falls back to simulated values if API is unavailable (for demo purposes)
- Client-side processing - no backend needed
- Includes intelligent heuristics for common words

## UI/UX Design

- **Gradient header:** Eye-catching purple gradient
- **Color coding:** Intuitive green → yellow → red scale
- **Responsive:** Mobile-first design approach
- **Accessibility:** Clear labels, hover tooltips, keyboard shortcuts
- **Performance:** Optimized for fast loading and smooth interactions

## Research Context

This demo is part of my broader research on:
- Computational models of language processing
- Neural correlates of linguistic prediction (EEG studies)
- Human-AI alignment in language understanding
- Predictive coding in the brain

## AI-Assisted Development

This project was developed with **Claude AI assistance**, demonstrating:
- **Rapid prototyping:** Idea to working demo in <1 hour
- **Clean code:** Well-structured, maintainable implementation
- **User experience:** Thoughtful UI/UX design
- **Documentation:** Comprehensive README and inline comments

### Development Process

1. **Concept:** Interactive tool to showcase GPT-2 research
2. **AI Collaboration:** Claude helped design the architecture and UI
3. **Iteration:** Refined based on research requirements
4. **Polish:** Added visual design, examples, and error handling
5. **Deployment:** One-file design for easy GitHub Pages hosting

## Example Use Cases

### Educational
- Teaching information theory and surprisal
- Demonstrating how language models work
- Exploring predictability in natural language

### Research
- Quick validation of linguistic hypotheses
- Generating test stimuli with known surprisal values
- Comparing predictability across different texts

### Applied
- Assessing text readability
- Identifying challenging vocabulary
- Content optimization for different audiences

## Future Enhancements

- Add support for GPT-3/GPT-4 (via API)
- Batch processing of multiple sentences
- Export results to CSV/JSON
- Comparison mode (compare two texts)
- Historical context window visualization
- Integration with eye-tracking data
- Mobile app version

## About

**Yasemin Gokcen**  
PhD Student, Cognitive & Information Sciences  
University of California, Merced

**Research Focus:** Computational models of language processing, neural correlates of prediction, human-AI interaction

**Contact:**
-  Email: ygokcen@ucmerced.edu

##  Acknowledgments

- **Cursor and Google AI Studio** for development assistance and rapid prototyping
- **Hugging Face** for providing the GPT-2 inference API
- **Natural Stories Corpus** for inspiring the research
- **OpenAI** for the original GPT-2 model

## 📄 License

MIT License - Feel free to use, modify, and share!

---

**Note:** This is a demonstration tool built for educational and research purposes. For production use with large-scale text processing, consider using the full research implementation or the official Hugging Face libraries.
