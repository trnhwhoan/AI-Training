<img width="731" height="736" alt="image" src="https://github.com/user-attachments/assets/113b1b6e-d730-47fa-94ae-6555691335e1" /># AI-Training

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
- User can adjusting general-purpose models to maximize performance on a specifically task.

####






 



