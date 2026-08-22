# AI-Training

## Book: AI Engineering
## Chapter 1

### Why do language models use token as their unit instead of word or character?
- Tokens allow models to divide one word into multiple meaningful parts.
- ex: "cooking" => "cook" and "ing"
- There are fewer unique tokens than unique words.
- ex: vocab will have: cooking, cooker, cooks, cooked,.., then each word has to be stored as a separate unit, while with tokens, the parts can be combined to create words. So instead of storing words like in the vocab, tokens only need to store: cook, ing, er, s, ed,.. => this helps make the model more efficient.
- Tokens also help the model process unknown words.
- ex: When the model encounters "chatgpting", the model may not understand the whole word, so it can divide it into parts "chatgpt" and "ing" like the first point to process it. This helps the model understand unknown words by dividing them into multiple parts.
- Tokens balance between characters and words. It is not too small like a character and not too large like a word.

#### Masked language models & Autore-gressive language models
##### Masked language models
- Masked language models are models that can fill in the blank based on the context.
- ex: When the context is "My fav ___ is blue", the masked language model will predict the missing word as "color".
- Masked language models are often used for non-generative tasks like: sentiment analysis and text classification. Besides that, it can handle tasks that require understanding the whole context like code debugging.

##### Autore-gressive language model
- Autoregressive language models are models that can predict the next token based on the previous token.
- ex: My => My favorite => My favorite color => My favorite color is => My favorite color is blue.
     => continually generate one token after another.

##### The difference between Masked language models and Autoregressive language models
- Autoregressive language models predict the next token based on the previous token, and they cannot see the token behind because there is no token behind yet.
- ex: The "predictive text" feature on iOS device keyboards. When users type, it uses the previous text to suggest the next word based on the user's word usage habits.
      GPT considers the current context and learned relationships to calculate the probability of possible next tokens, then selects a suitable token.
- Masked language models predict missing words at any position in a sentence, meaning that they can see the token before and after the blank.
- ex: When doing fill-in-the-blank exercises in English, we have to read the words before and after the blank to fill in the appropriate word.








