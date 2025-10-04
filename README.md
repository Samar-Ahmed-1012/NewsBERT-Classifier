# NewsBERT-Classifier
A fine-tuned BERT model that automatically categorizes news headlines into 4 topics (World, Sports, Business, Sci/Tech) with real-time web interface using Gradio.

Automated news categorization system using fine-tuned BERT transformer for real-time topic classification.

## Objective
Develop a high-accuracy classification system that categorizes news headlines into four topics: World, Sports, Business, and Sci/Tech for efficient content organization and analysis.

## Methodology

Architecture
- Base Model: BERT-base-uncased
- Fine-tuning: Transfer learning on AG News dataset
- Classification: 4-class linear head with softmax
- Tokenizer: BERT WordPiece (128 token length)

Training Approach
- Dataset: 3,000 samples from AG News
- Optimization: AdamW (lr=2e-5) with linear scheduling
- Epochs: 2 with batch size 8
- Framework: PyTorch + Hugging Face Transformers

Deployment
- Interface: Gradio web application
- Features: Real-time inference with confidence scores
- Access: Public URL sharing capability

📊 Key Results

Performance Metrics

Metric	Score

- Accuracy = 85-90% 

- F1-Score = 	86-89% 

- Inference =  Speed	< 100ms

Category Performance

- Category	F1-Score 

- Sports = 93.0% 

- Sci/Tech = 87.5% 

- World = 86.5% 

- Business = 83.5% 

## Key Observations
-- Efficient Fine-tuning: Achieved high accuracy with only 3,000 samples and 2 epochs
-- Sports Dominance: Clear vocabulary patterns yielded highest performance (93% F1)
-- Business Challenges: Slight confusion with World category in economic contexts
-- Production Ready: <100ms inference suitable for real-time applications

* Running on public URL: https://b3793e1ba7d8d377f1.gradio.live
