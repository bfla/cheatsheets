# Hugging Face

## Basic Examples

### Text classification
```python
from transformers import pipeline
import pandas as pd

classifier = pipeline('text-classification')
text = 'Foo bar'
outputs = classifier(text)
pd.DataFrame(outputs)
```

### Named Entity Recognition
```python
ner_tagger = pipeline('ner', aggregation_strategy='simple')
outputs = ner_tagger(text)
pd.DataFrame(outputs)
```

### Question Answering
```python
reader = pipeline('question-answering')
question = 'What does the customer want?'
outputs = reader(question=question, context=text)
pd.DataFrame([outputs])
```

### Summarization

### Translation

## Recommended Papers
- [Attention is all you need](https://arxiv.org/abs/1706.03762): The transformer architecture
- [Universal Language Model Fine-Tuning for Text Classification](https://arxiv.org/abs/1801.06146): UMLFiT transfer learning method
- [Improving Language Understanding by Generative Pre-Training](https://openai.com/blog/language-unsupervised): GPT 1 
- [BERT: Pre-Training of Deep Biderectional Transformers for Language Understanding](https://arxiv.org/abs/1810.04805)
- [Sequence to Sequence Learning with Neural Networks](https://arxiv.org/abs/1409.3215)
- [The Unreasonable Effectiveness of Recurrent Neural Networks (Karpathy)](https://oreil.ly/Q55o0)
