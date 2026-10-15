# AI-Training

## Book: Grokking 
## Day 01

### Theory
#### Dataset
- **Dataset** - is collection data use to train, check or rate Machine Learning.
- ex: We can build forecast score model base on learning time -> a **tabular dataset**.
- In table have:
  -- Each row -> a sample.
  -- Each column -> a attribute or value need forecast.
  -- All table -> a dataset.

#### Feature and Labels
- **Features** - input information models use to learn and forecast. ex: Hours studies, Attendance (attendance tracking and timekeeping management features).
- **Label** - target value model need to learn the way by forecast. ex: Exam score.
- The way data enter to model:
<img width="636" height="189" alt="image" src="https://github.com/user-attachments/assets/eb6d96cc-b9ea-46b0-be7b-4d5ef956b7d2" />
- **Features** and **Labels** not fixed to every dataset. It depend on the problems that need to solve.
- ex: In a student data table:
  -- Want to predict exam scores -> Exam score là **label**.
  -- Want to predict attendance rate -> **Attendance** become to **label**.
  --> define prediction objectives before choose **features** and **label**.
