# AI-Training

## Book: Grokking Machine Learning
## Week 3 - Day 3

### Underfitting & Overfitting
#### Training Data & Testing Data
- **Training Data** - data used to model learning.
  
- **Testing Data** - data is set aside to test the model's predictive capability on data it has not previously encountered.

- ex: Glowee have 1.000 record about visits and revenue.
  Divide the data as follows:
  
  <img width="610" height="169" alt="image" src="https://github.com/user-attachments/assets/e8a85a34-576e-4df2-bc12-c94d04fb19e5" />

Model learn on 800 samples, then evaluated on 200 samples.

- *Why should data be split?*

  If we only evaluate a model on the data it has already learned from, we cannot know whether it will perform well on new data.

#### Underfitting
- **Underfitting** happen when model too simple to learn the true law of data.

- ex: Glowee's revenue increase follow visits but tends to curve, while model only try to fit it using a simple straight line.
  <img width="394" height="330" alt="image" src="https://github.com/user-attachments/assets/27aa114a-ea70-456f-841e-78c3d5f51727" />

  Common signs:
    -- Training Error high
  
    -- Testing Error high
  
    -- Model has not yet learned enough patterns from the data

#### Overfitting
- **Overfitting** happen when model learn too close training data, even including *noise* or the details lack any discernible pattern.

<img width="729" height="470" alt="image" src="https://github.com/user-attachments/assets/4c112b84-bd72-404c-99cc-047477033764" />

  Common signs:
    -- Training Error low
   
    -- Testing Error significantly higher
    
    -- Model generalize difficult on new data

  #### Compare Underfitting and Overfitting

  
| Criteria | Underfitting | Overfitting |
| :--- | :---: | ---: |
| Model | Too simple | Too complicated |
| Training Error | High | Low |
| Testing Error | High | Often high |
| Ability to learn patterns | Not enough | Learn through noise |
| General capability | Least | Least |






  
