# AI-Training

## Book: AI Engineering
## Chapter 1

### Introduction
- Before 2020, ML had already been used to create many applications, like: product recommendations, fraud detection, and churn prediction.
- After 2020, the scale increase helps AI models became to strong and can to do tasks than before.
### Foundation models
#### Language models
-A language model is a model that can predict information based on the context of one or more languages.
ex: When the context is: "My favorite color is ___", ta language model that has learned English will predict "blue" rather than "car" because it uses the context of the sentence to predict the most likely word.
#### The statistical nature of language
- Using statistics to analyze language has existed for a long time, ex: Sherlock Holmes used the frequency of letters in English to decode a message. Later, Claude Shannon developed more sophisticated statistical methods to model English. Concepts such as entropy were introduced and are still important in modern language modeling.
#### Token
- Token is the basic unit of a language model.
- A token can be a character, word or part of a word.
  => model does not necessarily process text word by word.
#### Tokenization
- Tokenization is the process of converting from text to tokens.
ex: "I can't wait to buils awesome AI applications." - divided into 9 tokens by GPT-4 from OpenAI.
- For GPT-4, 1 token = 3/4 the length of a word.
#### Vocabulary
- Vocabulary is the set of all tokens that a model can work.
- Vocabulary's size depends on the model và tokenization.
ex: Mixtral 8x7B → vocabulary: 32,000
    GPT-4 → vocabulary: 100,256





