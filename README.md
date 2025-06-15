# Text Classification (multi-class classification)

Created a multi-class text classification model to categorize Indonesian tweets related to the 2024 presidential election into 8 national resilience components (Astagatra) using CNN-BiLSTM architecture.

## Steps Performed:

### Text Preprocessing
- Removed text inside square brackets (`[ ]`)
- Removed URLs and special characters
- Filtered out random long characters (>15 letters)
- Removed punctuation
- Applied case folding
- Trimmed extra whitespaces
- Removed Indonesian stopwords
- Applied stemming using Sastrawi

### Exploratory Data Analysis
- Generated word frequency analysis
- Visualized top terms using WordCloud

### Data Preparation
- Label encoding for 8 Astagatra categories
- Resampling to balance class distribution

### Text Tokenization & Embedding
- Tokenized tweets using Keras tokenizer
- Used pretrained Word2Vec embeddings for Indonesian

### Model Development
- Built a CNN-BiLSTM architecture
- Added embedding, convolutional, BiLSTM, and dense layers

### Model Training & Evaluation
- Split data into training and validation sets
- Trained model using categorical cross-entropy loss
- Achieved 96% validation accuracy
