# AI-900 Study Notes - Day 1

## AI Workloads

### Core AI Concepts

**Artificial Intelligence**  
The ability of computer systems to **perform tasks that typically require human intelligence**, like learning, reasoning, problem-solving, perception, and language understanding, by analyzing data to find patterns, make decisions, and act autonomously.

**Machine Learning**  
A specialized subfield of artificial intelligence (AI) that focuses on building systems that **"learn" from data rather than being explicitly programmed** for a specific task.

### AI Workload Types

#### 🧠 Natural Language Processing

Focuses on **understanding human language**. NLP tasks include:

- Text analysis (summarization, sentiment analysis)
- Key phrase and entity extraction
- Language translation
- Conversational Language Understanding

#### 👁️ Computer Vision

Enables machines to **interpret and understand visual inputs** (images or videos):

- Image classification and object detection
- Facial detection/recognition
- Optical Character Recognition (OCR)

#### 🗣️ Speech

AI techniques that **process and understand spoken language**:

- Speech recognition (speech to text)
- Speech synthesis (text to speech)

#### 📄 Information Extraction

Azure provides tools for building AI-powered information extraction solutions:

- Document Intelligence
- AI Search
- Vision Analysis
- Video Indexer
- Content Understanding

#### ✨ Generative AI

Involves **creating new content** using AI models:

- Generate text, images, code, or audio that mimic human-created content
- Relies on Large Language Models (LLMs)
- Examples: Copilot, ChatGPT

## Responsible AI

#### ⚖️ Fairness

AI models are trained using data, which is generally sourced and selected by humans. There's substantial risk that the data selection criteria, or the data itself reflects unconscious **bias** that may cause a model to produce discriminatory outputs. AI developers need to take care to minimize bias in training data and test AI systems for fairness.

#### 🛡️ Reliability and Safety

AI is based on probabilistic models; it **can make mistakes**. AI-powered applications need to take this into account and mitigate risks accordingly.

#### 🔒 Privacy and Security

Models are trained using data, which may include **personal information**. AI developers have a responsibility to ensure that the training data is kept secure, and that the trained models themselves can't be used to reveal private personal or organizational details.

#### 🌍 Inclusiveness

The potential of AI to improve lives and drive success should be **open to everyone**. AI developers should strive to ensure that their **solutions benefit all parts of society** and don't exclude some users.

#### 🔍 Transparency

AI can sometimes seem like "magic", but it's important to make **users aware of how the system works** and **take decisions** and any **potential constraints or limitations** it may have.

#### 📋 Accountability

Ultimately, the people and organizations that develop and distribute AI solutions are accountable for their actions. It's important for organizations developing AI models and applications to define and **apply a framework of governance** to help ensure that they apply and meet any **ethical and legal standards** for their work.

### 📝 Responsible AI Quick Reference

| Principle                 | Key Focus                             | Action Items                                                                                |
| ------------------------- | ------------------------------------- | ------------------------------------------------------------------------------------------- |
| **⚖️ Fairness**           | Bias mitigation                       | • Take many factors into account                                                            |
| **🛡️ Reliability/Safety** | Mistakes/harm prevention              | • Proper testing and validation before launch                                               |
| **🔒 Privacy/Security**   | Personal information (PII) protection | • Secure data handling and storage                                                          |
| **🌍 Inclusiveness**      | Accessibility for everyone            | • Enlist diverse people during model training<br>• Reflect the population using the product |
| **🔍 Transparency**       | "How" and "why" understanding         | • Clearly explain model decisions<br>• Make outputs understandable and justifiable          |
| **📋 Accountability**     | Governance framework                  | • Ethical and legal standards<br>• Oversee and monitor                                      |

## Machine Learning

### ML Process Flow

```
Train → Validate → Iterate → Reduce Loss
```

### Key Concepts

**Features**  
The **input variables (attributes)** used to make a prediction.

**Labels**  
The target outcome **we want to predict**.

**Training Dataset**  
Used to **train** the model (fit the model's parameters).

**Validation Dataset**  
A held-out portion used to **evaluate** the model's performance on unseen data and tune it.

### ML Types

#### 📊 Supervised Learning

_Uses labeled data: [x₁, x₂, x₃], y_

##### Regression

- **Purpose**: Predicting numeric values
- **Output**: Continuous numbers (how much/how many)
- **Example**: Predicting house prices

##### Classification

- **Purpose**: Predicting categories or class labels
- **Output**: Discrete classes
- **Types**:
  - Binary ("spam" vs "not spam")
  - Multiclass (movie genres)
- **Example**: Email spam detection

#### 🔍 Unsupervised Learning

_Uses unlabeled data: [x₁, x₂, x₃]_

##### Clustering

- **Purpose**: Groups similar data points into clusters
- **No predefined labels**
- **Example**: Grouping customers based on purchasing behavior

### 📝 Quick Reference

**Labels vs Features**

> You want to predict **\<label>** based on **\<features>**

**ML Type Decision Tree**

```
Do you have labels?
├── Yes → Supervised ML
│   ├── Predicting numbers → Regression
│   └── Predicting categories → Classification
└── No → Unsupervised ML
    └── Finding groups → Clustering
```
