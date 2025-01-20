# AptitudeTest

A Python package for conducting aptitude tests with randomly generated questions and a timed interface.

## Features

- Random question selection from a pool.
- 1-minute timer for each question.
- Dynamic quiz length based on user input.
- Scoring and result display at the end of the quiz.

## Installation

To install the package, run:

```bash
pip install aptitudetest

```
## Test the quiz 
```
from quiz_questions import conduct_quiz, get_random_questions, questions_pool
    
num_questions = int(input("Enter the number of questions for the test: "))
    
if num_questions > len(questions_pool):
    print("Not enough questions in the pool. Please choose a smaller number.")
else:
    selected_questions = get_random_questions(questions_pool, num_questions)
    conduct_quiz(selected_questions)

```

