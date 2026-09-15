<img width="727" height="545" alt="image" src="https://github.com/user-attachments/assets/4493f461-3038-43ee-9fb8-cb40cd38596d" /># AI-Training

## Book: AI Engineering
## Chapter 1

### Self-supervision
#### Supervision
- Supervision is a method to training ML algorithms. It label data for any object/categories.
- However, supervision is expensive and time-consuming.
  - ex: I want to label one image for a person, cost is 5 cents, a million image = $50,000. But I could cross-check label quality, cost is double.

#### Self-supervision
- Self-supervision helps reduce the need for manual data labeling.
- The model can infer labels form the input data.
- Language modeling is self-supervised because the input sequence provides both the context and the target tokens.

#### Language model
- A language model learns to predict the next token from the given context.
  - ex: <img width="620" height="211" alt="image" src="https://github.com/user-attachments/assets/1ac83bac-904c-45fb-9f0d-353f34467cec" />
- A single sentence can generate multiple training samples.

#### BOS & EOS
- BOS (Beginning of Sequence) marks the start of a sequence.
- EOS (End of Sequence) marks the end of a sequence.
- These special tokens help the model process multiple sequence and know when to stop generating.

#### Self-supervised Learning
- Allows language models to learn from text sequences without manual labeling.
- Text is everywhere, allowing us to create massive amounts of training data and helping language models scale up to become LLMs.

#### LLMs & Parameters
- LLM (Large Language Model) does not have a fixed definition of size. A model's size is usually measured by the number of parameters.
- A parameter is a variable within an ML model that is updated during the training process. In general, the more parameters a model has, the greater its capacity to learn desired behaviors.
  - ex: GPT (2018) had 117 million parameters, while GPT-2 (2019) had 1.5 billion parameters.

#### Why Do Larger Models Need More Data?
- Because larger models have a greater capacity to learn, they need more training data to take advantage of that capacity and improve performance.


 




