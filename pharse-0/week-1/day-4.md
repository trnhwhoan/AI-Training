# AI-Training

## Book: AI Engineering
## Chapter 1

### Opened-ended outputs
- Open-ended is a language model that has a fixed number of tokens. From these tokens, it can combine them into countless different sentences.
- ex: Vocabulary: I, am, a, student, software, developer,....
> "I am a student."
> "I am a student software developer."
> "I am a student learning AI."
> .......
=> fixed vocabulary -> infinite possible outputs
- The model can create many sentences from a finite set of tokens.
- generative -> generative AI.
### Completion machine
- Completion machine is a machine that completes text when it is provided with an unfinished piece of text by the user.
- ex:
  - Prompt (from user): "To be or not to be"
  - Completion (from language model): ", that is the question."
- The answer provided by the language model is based on probability and is not guaranteed to be correct.
- Technically, a masked language model like BERT can also be used to create text if
- Many tasks like translation, summarization, coding,.... can be modeled as completion tasks.
- ex: translation
  > Prompt: "How are you in Vietnamese is..."
  > Completion: "Bạn khỏe không?"
- But the answer is not always correct. The answer is generated based on the patterns and relationships that the language model learned during the training process.
- In autoregressive models like GPT, the model generates text by predicting one token at a time and using the generated token as part of the context for predicting the next token.
- Completion machine only has the task of continuing the text, by looking at the previous tokens and predicting the next token.
- ex:
  > Prompt: "What is the capital of Vietnam?"
  > Completion: "What is the capital of Thailand?"









