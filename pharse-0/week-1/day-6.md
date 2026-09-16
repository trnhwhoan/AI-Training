# AI-Training

## Book: AI Engineering
## Chapter 1

### From Large language Models to Foundation Models
#### Issue of the traditional LLM
- Traditional language models are mainly limited to text, but real-world information also includes images, audio, video, 3D data, and other modalities.
- To handle real-world tasks, language models are being extended to support multiple data modalities. Models such as GPT-4V and Claude 3 can understand both text and images, while some models can also process video, 3D assets, and protein structures.

#### Multimodal
- **multimodality** is ability handle datas. 
- Supporting multiple modalities makes AI models more powerful and useful for different applications.

#### Foundation models
- **Foundation models** is a background model can use to build many AI applications.
- LLM focus on handle and create language, FM larger, can become to background for many applications.
- A Foundation model can be handle: text, image, audio, video,...

#### Multimodal model
- **Multimodal model** is a model can working to more than one type of data.
- A multimodal model have ability create content = large multimodal model (LMM).
- Multimodal model create the next token base on text token, image token, or any type of token belonging to the modalities supported by the model.
- Multimodal model also needs data to develop.
- Self-supervision also work like multimodal models.
  - ex: OpenAI used a varian of self-supervision is natural language supervision to training language-image model CLIP in the 2021. They find out these couple (image,text) in the internet. Therefore, they create a dataset include 400 million couple image-text without bear the cost of manual labeling. So, CLIP become to the first model can generalize to various image classification tasks without additional training.
- Large language models - LLMs
- Large multimodal models - LMMs

#### CLIP
- **CLIP** is an embedding model receive training to create these embedding collab for text, image.
- Embedding is vectors try to perform meaning of original data.
  - ex:
    * "cat" → [0.2, 0.8, 0.1, ...]
    * "kitten" → [0.3, 0.7, 0.2, ...]
    * "car" → [0.9, 0.1, 0.6, ...]
- These multimodal embedding models like CLIP is underlying platform generative multimodal models like Flamingo (a vision language model of Google), LLaVA (Large Language and Vision Assistant - a LMM model), Gemini.

#### Transformation of foundation models
- Foundation models transfer from Task-specific models to General-purpose models, can work multiple types of tasks as a same time.
- **Task-specific model** built for a specific mission.
- **General-purpose model** trained to perform multiple tasks.
- User can adjusting general-purpose models to maximize performance on a specifically task.

#### 3 technical to adjust foundation model on demand
- **Prompt engineering**: I can write detailed instructions and examples about describe of desired product.
- **Retrieval-Augmented Generation - RAG**: I can connect model with a database contain reviews of customer.
- **Fine-tuning**: I can continue training the model on a dataset comprising high-quality product descriptions.

### Adapting Existing Models

- Adapting an existing powerful model is usually easier, faster, and cheaper than building a model from scratch. Foundation models reduce AI development costs and time to market.
- However, task-specific models still have advantages. They may be smaller, faster, and cheaper to use.

### Build or Buy Decision
- AI teams must decide whether to build their own model or use an existing model.
- The decision depends on factors such as cost, data, time, performance, control, and deployment requirements.

  






 



