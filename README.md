# Quiz Application (Python)

A Python quiz application built using dictionaries and loops to evaluate user responses and display scores.
## Features
- Multiple quiz questions
- Automatic score calculation
- Simple terminal-based interface
- Beginner-friendly logic

## Technologies Used
- Python
- Dictionary
- Loops
- Conditional statements

## Code
```python
print("WELCOME TO PYTHON QUIZ")

score = 0

questions = {
    "What is the capital of India? ": "delhi",
    "Which keyword is used to define a function in Python? ": "def",
    "What is the output of 2 + 2? ": "4",
    "Which data type stores True or False? ": "boolean"
}

for question, answer in questions.items():
    user_answer = input(question).lower()
    if user_answer == answer:
        print("Correct ✅")
        score += 1
    else:
        print("Wrong ❌")

print("\nQuiz Completed!")
print("Your Score:", score, "/", len(questions))
