# AI-Training

## Book: Grokking Machine Learning
## Chapter 1

### Three Layers of the AI Stack
- An AI application stack can be divided into three main layers:

#### 1. Application Development
- This is the layer closest to the end user. Instead of building models from scratch, developers use existing models to create AI applications.
- Main responsibilities include:
  - AI interface
  - Prompt engineering
  - Context construction
  - Evaluation
- Application development focuses on giving models the right instructions, context, and tools, evaluating their outputs, and building useful interfaces for users.

#### 2. Model Development
- This layer focuses on developing and adapting models.
- Main responsibilities include:
  - Modeling and training
  - Dataset engineering
  - Inference optimization
  - Evaluation
- With foundation models, developers often do not need to train models from scratch. Instead, they can adapt existing models using techniques such as prompt engineering or finetuning.

#### 3. Infrastructure
- Infrastructure provides the underlying systems required to run AI models and applications.
- Main responsibilities include:
  - Compute management
  - Data management
  - Model serving
  - Monitoring
- Unlike application development, infrastructure requirements have changed less dramatically with foundation models. Models still require compute, data management, serving systems, and monitoring.

#### Growth of the AI Engineering Ecosystem
- The AI ecosystem grew rapidly after the introduction of foundation models such as Stable Diffusion and ChatGPT.
- The strongest growth has occurred in applications and application-development tools. Infrastructure has grown more slowly because many fundamental infrastructure requirements remain similar.
- Despite new technologies, many traditional ML engineering principles still apply, including systematic experimentation, evaluation, optimization, and feedback loops.

### AI Engineering vs. ML Engineering
- AI engineering evolved from ML engineering, so the two fields overlap significantly. However, building applications with foundation models introduces several important differences.

#### Key Differences
**1. Model development vs. model adaptation**
- Traditional ML engineering often requires teams to train their own models.
- AI engineering usually starts with foundation models that have already been trained. Therefore, the focus shifts from building models to adapting existing models.

**2. Larger models and higher computational requirements**
- Foundation models are usually much larger than traditional ML models. They require more compute and can have higher inference costs and latency.
- Therefore, inference optimization becomes especially important.

**3. Open-ended outputs**
- Traditional ML systems often produce close-ended outputs, such as a classification label.
- Foundation models can generate open-ended outputs such as text, images, or code. This flexibility makes them useful for many tasks but also makes evaluation much harder.

#### Model Adaptation
- There are two major approaches to adapting foundation models.
- **Prompt-based techniques** adapt a model without changing its weights. Developers provide instructions, context, and examples through the model input.
- Prompt engineering is easier to experiment with and usually requires less data.
- **Finetuning** modifies the model weights through additional training. It is more complex and requires more data and resources, but it can significantly improve model behavior for specialized tasks.

### Model Development
- Model development traditionally includes three major responsibilities:

#### Modeling and Training
- This includes designing model architectures, training models, and finetuning them.
- Traditional ML development requires knowledge of algorithms, neural networks, gradient descent, loss functions, and other ML concepts.
- With foundation models, deep ML knowledge is not always required to build an AI application because developers can use existing models. However, ML knowledge remains valuable for understanding and troubleshooting models.

#### Pre-training, Finetuning, and Post-training
- **Pre-training** trains a model from scratch. It is usually the most expensive and resource-intensive stage.
- **Finetuning** continues training an existing model using additional data to adapt it to specific tasks or requirements.
- **Post-training** refers to additional training performed after pre-training. It is conceptually similar to finetuning, although the term is often used for improvements made by model developers before releasing a model.
- Prompt engineering is different from training because it does not modify model weights.

#### Dataset Engineering
- Dataset engineering involves creating, collecting, cleaning, annotating, and managing data used to train or adapt AI models.
- Traditional ML often works with structured or tabular data and focuses heavily on feature engineering.
- Foundation models work more with unstructured data. Important tasks therefore include:
  - Deduplication
  - Tokenization
  - Context retrieval
  - Quality control
  - Removing sensitive or toxic data
- Training from scratch generally requires more data than finetuning, while finetuning requires more data than prompt engineering.

#### Inference Optimization
- Inference optimization focuses on making models faster and cheaper during execution.
- This has become especially important for foundation models because they are large and often generate tokens sequentially, which can increase latency and computational cost.
- Common optimization techniques include quantization, distillation, and parallelism.

### Application Development
- When many developers have access to the same foundation models, the model itself becomes less of a competitive advantage.
- Instead, differentiation increasingly comes from how the application is built.
- The application development layer mainly includes:
  - Evaluation
  - Prompt engineering and context construction
  - AI interfaces

#### Evaluation
- Evaluation is essential throughout the model adaptation process.
- It helps developers:
  - Compare and select models
  - Measure progress
  - Decide whether an application is ready for deployment
  - Detect production problems
  - Identify opportunities for improvement
- Evaluation is harder with foundation models because their outputs are often open-ended. A prompt can have many valid answers, so there may not be a single ground truth.
- Model performance can also change significantly depending on the prompting or adaptation technique being used.

#### Prompt Engineering and Context Construction
- Prompt engineering controls model behavior through input rather than modifying model weights.
- Good prompts provide not only instructions but also the context and tools required to complete a task.
- For more complex applications, developers may also need systems for context retrieval and memory management.

#### AI Interface
- The AI interface defines how users interact with an AI application.
- Common interfaces include:
  - Web, desktop, and mobile applications
  - Browser extensions
  - Chatbots
  - APIs and plugins
  - Voice interfaces
  - AR/VR interfaces
- Conversational interfaces also create new opportunities for collecting user feedback because users can describe their experiences naturally.
- For foundation-model applications, AI interfaces and prompt engineering become important responsibilities, while evaluation becomes even more important than in traditional ML.

### AI Engineering vs. Full-Stack Engineering
- AI engineering is becoming increasingly connected to full-stack and software engineering because foundation models make it easier to build applications without training models from scratch.
- Traditionally, ML engineering often followed this workflow:
**Data → Model → Product**
- Teams first collected data, trained a model, and then built a product around it.
- With foundation models, AI engineering can often reverse this process:
**Product → Data → Model**
- Developers can quickly build a product using an existing model, collect feedback and data from real users, and invest more heavily in data or model adaptation only after the product shows potential.
- This makes rapid prototyping and iteration especially valuable in AI engineering.
- Full-stack engineers can therefore have an advantage because they are able to quickly turn ideas into working products, collect feedback, and iterate.
### Chapter 1 — Final Takeaway
- AI engineering emerged because foundation models allow developers to build powerful AI applications without training every model from scratch.
- It evolved from ML engineering and still uses many of the same principles, but the focus has shifted toward **model adaptation, evaluation, prompt engineering, context construction, interfaces, and rapid product iteration**.
- A useful way to understand the field is through the three-layer AI engineering stack:
**Application Development → Model Development → Infrastructure**
- Foundation models do not eliminate traditional ML engineering. Instead, they change where engineering effort is concentrated and make AI application development accessible to a much broader group of developers.
