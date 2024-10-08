# Dynamic-IRT

1. Each row is one student's data, each column is one feature.

2. For each chapter level feature, the corresponding column startw with 
ch##_ (e.g., ch01_).

3. The column is organized in a way that starts with review questions.
- Example: ch01_a1_review1_01, represents the first end-of-chapter quiz's first question performance (0 or 1).
- We didn't include free resposne questions in the dataframe, all included questions are those being graded.
- For some chapters, there might be no end-of-chapter quiz or two end-of-chapter quizzes. Thus the numbers of columns for each chapter's question are not the same.

4. Then after each chapter's end-of-chapter quiz questions, we have engagement features (e.g., ch01_d_mean), the middle identifier represents corresponding feature.
- d_mean: Average length of session durations in minutes
- d_max: Maximum length of session durations in minutes
- er: Ratio between engaged time and total reading time
- n: Number of reading sessions

5. At the end for each student:
- Gender: What best describes your gender?
- Race: Which of the following categories describe you? If you'd like to use more than one category or if you'd like to use a category not provided, please select "prefer to self-describe" and answer the next question.
- Math_anxiety: In general, I tend to feel very anxious about mathematics.
- Memorization_belief: I expect that this course will require a lot of memorization.
- Utiltiy_1: What I'm going to learn in this class will be useful in the future.
- Utility_2: What I'm going to learn in this class will be relevant to my everyday life.
