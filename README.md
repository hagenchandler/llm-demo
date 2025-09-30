# 🤖 LLM Tokenization & Generation Demo

An interactive web-based demonstration showing how Large Language Models (LLMs) tokenize text and generate responses. Watch in real-time as the model processes input, calculates probabilities, and selects the next token!

## Features

-  Live Tokenization** - See how your input text is broken down into tokens with unique IDs
-  Probability Visualization** - Watch real-time probability distributions for candidate tokens
-  Adjustable Speed** - Control generation speed from 100ms to 2000ms per token
-  Token Limit Control** - Set maximum tokens to generate (3-20)
-  Natural Stopping** - Simulates how LLMs use special `<END>` tokens to complete responses
-  Score Tracking** - View logit scores and how they convert to probabilities via softmax
-  Educational Explanations** - Learn how token IDs relate to probability calculations

## 🚀 Live Demo

Vercel: https://llm-demo-ten.vercel.app/

## Screenshot

![LLM Demo Screenshot](https://via.placeholder.com/800x500?text=LLM+Demo+Screenshot)

*Replace with actual screenshot once deployed*

## How It Works

1. **Input Text** - Enter any prompt (e.g., "The weather today is")
2. **Tokenization** - Text is split into tokens, each assigned a unique ID
3. **Score Calculation** - The model calculates logit scores for possible next tokens
4. **Softmax Conversion** - Logits are converted to probabilities that sum to 100%
5. **Token Selection** - The highest probability token is selected
6. **Repeat** - Process continues until `<END>` token or max limit is reached

## Technical Details

- **Pure HTML/CSS/JavaScript** - No frameworks or dependencies required
- **Simulated Vocabulary** - Uses a 50,000 token vocabulary (simulated)
- **Realistic Softmax** - Implements proper softmax function for probability calculation
- **Token ID Hashing** - Generates consistent token IDs using hash functions

## Local Development

1. Clone the repository:
```bash
git clone https://github.com/YOUR-USERNAME/REPO-NAME.git
cd REPO-NAME
```

2. Open `index.html` in your browser:
```bash
# On macOS
open index.html

# On Linux
xdg-open index.html

# On Windows
start index.html
```

Or use a local server:
```bash
# Python 3
python -m http.server 8000

# Python 2
python -m SimpleHTTPServer 8000

# Node.js (with npx)
npx http-server
```

Then visit `http://localhost:8000`

## Educational Use Cases

Perfect for:
- **Students** learning about NLP and LLMs
- **Educators** teaching machine learning concepts
- **Presentations** demonstrating how AI language models work
- **Workshops** on tokenization and probability distributions

## Customization

You can easily customize:
- **Response templates** - Edit the `responses` object in the JavaScript
- **Token vocabulary** - Modify the `vocab` array for different candidate tokens
- **Speed ranges** - Adjust min/max values in the speed slider
- **Styling** - Update the CSS styles in the `<style>` section
