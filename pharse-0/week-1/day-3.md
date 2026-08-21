# AI-Training

## Book: AI Engineering
## Chapter 1

### Why do language models use token as their unit instead of word or character?
- Tokens allows models chia 1 từ ra thành nhiều phần có ý nghĩa.
ex: "cooking" => "cook" and "ing"
- Có ít token độc nhất hơn vocab độc nhất.
ex: vocab sẽ có: cooking, cooker, cooks, cooked,.., thì mỗi từ phải được lưu thành 1 unit riêng
    còn với token thì có thể ghép các phần vào để tạo thành từ, thì thay vì phải lưu như vocab thì token chỉ cần lưu: cook, ing, er, s, ed,..
  => điều này giúp model được tối ưu hơn
- Token also help the model xử lí những từ chưa biết.
ex: Khi model gặp "chatgpting", model sẽ không hiểu nguyên cụm từ mà nó sẽ chia ra từng phần "chatgpt" and "ing" như ý đầu tiên để xử lí. Điều đó giúp model có thể hiểu được những từ chưa biết thông qua việc chia từ ra thành nhiều phần.
- Token cân bằng giữa chữ và từ. Nó không quá nhỏ như chữ mà cũng không lớn như từ.
#### Masked language models & Autore-gressive language models
##### Masked language models
- Masked language models is a model có khả năng điền vào chỗ trống dựa trên ngữ cảnh.
ex: Khi có context "My fav ___ is blue" thì Masked language model sẽ dự đoán từ bị thiếu là "color".
- Masked language model thường được dùng cho những non-generative like: sentiment analysis and text classification. Ngoài ra, it can be đảm nhiệm những nhiệm vụ cần hiểu hết ngữ cảnh như code debugging.
##### Autore-gressive language model
- Auto-gressive language models is model can be dự đoán token tiếp theo dựa trên token trước nó.
ex: My
    My favorite
    My favorite color
    My favorite color is
    My favorite color is blue.
  => continually generate one token after another.
##### Sự khác nhau giữa Masked language models và Autore-gressvie language models
- Autore-gressive language models đoán the next token dựa theo token phía trước, và nó không thể nhìn token phía sau vì chưa có token nào phía sau.
ex: Tính năng "tiên đoán văn bản" có trên bàn phím của các thiết bị iOS. Khi người dùng gõ chữ, thì nó sẽ căn cứ vào chữ phía trước để gợi ý chữ tiếp theo dựa trên thói quen dùng từ của người dùng.
    GPT considers the current context and learned relationships to calculate the probability of possible next tokens, then selects a suitable token.
- Masked language models đoán những từ bị bỏ trống ở bất cứ vị trí nào trong câu, tức là nó có thể nhìn được token trước và sau chỗ cần điền.
ex: Khi làm các dạng bài điền từ trong bài tập tiếng Anh, chúng ta phải đọc những từ ở trước và ở sau để điền từ phù hợp.








