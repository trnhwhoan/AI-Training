# AI-Training

## Book: Grokking Machine Learning
## Chapter 1

### Setting Expectations
- Before building an AI application, it is important to define what success looks like and how it will be measured.
- The most important metrics should reflect business impact, such as the percentage of tasks automated, response speed, productivity improvements, and labor savings.
- However, business performance alone is not enough. AI applications also need a clear **usefulness threshold**, which defines how good the system must be before it becomes useful to users.
- Important metrics can include response quality, latency, cost per inference request, interpretability, fairness, and customer satisfaction.
- Latency can be measured using metrics such as **TTFT (Time to First Token)**, **TPOT (Time Per Output Token)**, and total latency. The acceptable level depends on the specific use case.

### Milestone Planning
- After defining measurable goals, teams should evaluate existing models to understand their current capabilities and determine how much additional work is required.
- AI development also faces the **last mile challenge**. Foundation models can make it relatively easy to build an impressive prototype, but turning that prototype into a reliable production product can take much longer.
- Progress from an early prototype to acceptable performance may be fast, while improving the final percentages of quality becomes increasingly difficult because of edge cases, hallucinations, and other product issues.

### Maintenance
- When done initial goal, need thinking about change over time and how will undergo maintenance.
- Building product base on foundation models = accept keep up with that change speed.
- These limits had changes:
  - context length increasingly long
  - output better than
  - inference faster than
  - inference cheaper than
- The chart show that: ability of model increase when inference's cost strong decrease.
- However, the good update also cause be **friction**.
- Company must often: **Cost-benefit analysis** with technical decision.
- Company can building all infrastructure circle a third-party provider, but that provider can meet finance issues or cease operations.

#### Changing 
- When these model provider gradually use similar APIs, transfer from this model to that model becomes easier.
- Model have:
  - **quirks** - a behavior, reaction or error can repeat of AI/LLM
  - **strengths**
  - **weaknesses**
- When change model, developer also can edit:
  - **workflow + prompts + data**
- If system hasn't good infrastructure for: **versioning + evaluation** => each change model is crazy =)

#### Regulations
- **Regulations** are difficult to adapt to.
- AI can relate to:
  - **compute** - compute power or compute infrastructure like GPU, CPU TPU and network system.
  - **talent**
  - **data**
  - **national security**
  - **privacy**
  - **intellectual property**
- So, AI can maybe subject to very strict legal regulation.
#### Intellectual Property
- Regulations regarding IP and AI are still evolving.
- If your product is built upon a model trained using data from others, are intellectual property rights over your product always guaranteed?
  -> This is a reason causing some company heavy depend on IP, like game studio, it is advisable to exercise caution when using AI.

### The AI Engineering Stack
- AI engineering is evolving rapidly, with new tools, models, techniques, and applications appearing constantly.
- Instead of trying to follow every new trend, developers should focus on understanding the fundamental building blocks of AI engineering.
- AI engineering evolved from ML engineering.
- AI engineering and ML engineering have significant overlap.
- Some companies treat AI engineering and ML engineering as the same role, while others define AI engineering as a separate role.
- ML engineers can expand their skills into AI engineering, but AI engineers do not necessarily need previous ML engineering experience.
