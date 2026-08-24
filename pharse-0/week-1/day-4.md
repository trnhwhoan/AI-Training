# AI-Training

## Book: AI Engineering
## Chapter 1

### Opened-ended outputs
- Opened-ended is a language models have a tập token nhất định. Và form these token, it can be ghép thành vô số câu different.
- ex: Vocabulary: I, am, a, student, software, developer,....
  > "I am a student."
  > "I am a student software developer."
  > "I am a student learning AI."
  > .......
=> fixed vocabulary -> infinite possible outputs
- Model can be create many sentences form a token file hữu hạn
- generative -> generative AI.
### Completion machine
- Completion machine is a machine sẽ complete văn bản nếu được cung cấp 1 đoạn chưa hoàn thành từ user.
- ex:
  - Prompt (from user): " To be or not to be"
  - Completion (from language model): ", that is the question."
- Đáp án mà language model đưa ra dựa trên xác suất và không đảm bảo chính xác.
> Về mặt kĩ thuật, a masked language model like BERT also can be use to create text if
- Nhiều tác vụ like translation, summary, coding,....can be mô hình hoá thành tác vụ completion.
- ex: dịch thuật
  - Frompt: "How are u in Vietnamese is..."
  - Completion: "Bạn khoẻ không?"
- But không phải lúc nào đáp án cũng chính xác. Đáp án được đưa ra dựa trên những patterns/relationships mà languague model đã học trong training process.
- In autoregressive models like GPT, the model generates text by predicting one token at a time and using the generated token as part of the context for predicting the next token.
- Completion machine chỉ có nhiệm vụ viết tiếp, bằng cách nhìn vào token trước rồi viết ra câu tiếp theo.
- ex:
  - Frompt: "What is the capital of Vietnam?"
  - Completion: "What is the capital of Thailand?"
- 









