# 🧠 OOP Based Trivia Quiz Game (CLI Edition)

An interactive, object oriented command line trivia quiz game built in **Python 3**, designed to mimic real world quiz systems with clean, modular, and extensible code architecture. This application serves as a practical demonstration of Object Oriented Programming (OOP) principles and best practices in software design.

Developed as part of my structured Python development journey under the mentorship of **Dr. Angela Yu**, this project builds upon foundational logic and transforms it into a scalable solution using class based modeling. It encourages a deeper understanding of core Python programming patterns, while offering an engaging gameplay experience in the terminal.

---

## 📖 Overview

This trivia game immerses users in a series of curated True/False questions sourced from a structured dataset. The program dynamically presents questions, evaluates user input in real time, and tracks performance with continuous feedback.

Internally, each component is built around a specific responsibility: `Question` objects model the data, `QuizBrain` drives the gameplay loop and logic, and `data.py` acts as the source of quiz content. The architecture enables clear separation of concerns, enhanced code readability, and simplified future expansions such as question randomization or API integration.

This project exemplifies how robust programming principles can be applied to even the simplest of games to simulate structured, real world software behavior.

---

## 🧰 Technologies & Concepts Used

- **Python 3.10+**
- **Object Oriented Programming (OOP):**
  - Class based architecture with clear separation of concerns
  - Instance variables and method encapsulation
  - Composition for collaborative behavior across classes
- **Modular Programming:**
  - Source code is distributed across dedicated modules for logic, data, and models
- **Control Flow and Logic Structures:**
  - Conditional branching (`if/else`) and loops for iterative gameplay
- **Input/Output Handling:**
  - Command line interaction for dynamic user input and response feedback
- **Score Tracking Mechanism:**
  - Real time updates and post game results
- **Data Representation:**
  - Custom classes to transform dictionary data into usable objects

This codebase showcases how foundational concepts like data modeling, logic flow, and modularity can be combined to build structured, testable, and maintainable software.

---

## 🎮 Gameplay Mechanics

1. **Initialization:**
   - A list of questions is defined as dictionaries in `data.py`.
   - Each dictionary is instantiated as a `Question` object and added to a `question_bank`.

2. **Game Loop:**
   - The `QuizBrain` class manages the main loop and presents one question at a time using `next_question()`.
   - The user responds with `True` or `False`, and the answer is evaluated using `check_answer()`.

3. **Scoring:**
   - The score is incremented for each correct response.
   - After each question, the correct answer is displayed along with the user’s current score.

4. **Completion:**
   - When all questions are answered, the final score and total number of questions are displayed.

This gameplay loop is designed for clarity, engagement, and easy extensibility. Features like timed rounds, difficulty levels, or GUI enhancements can be integrated seamlessly.

---

## 📁 Project Structure

```
oop-trivia-quiz-game/
    ├── main.py             # Entry point for running the quiz game
    ├── data.py             # Contains the question dataset
    ├── question_model.py   # Models each question as an object
    ├── quiz_brain.py       # Handles quiz flow, scoring, and logic
    └── README.md           # Project documentation
```

---

### 🛠️ How to Run

> ⚠️ Make sure Python 3 is installed on your system.

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/oop-trivia-quiz-game.git
   ```

2. **Navigate to the project folder**
   ```bash
   cd oop-trivia-quiz-game
   ```

3. **Run the script**
   ```bash
   python main.py
   ```

---

## 📟 Sample Output

```
Q.1: A slug's blood is green. (True/False): true
You got it right!
The correct answer was: True.
Your current score is: 1/1

Q.2: The loudest animal is the African Elephant. (True/False): true
That's wrong.
The correct answer was: False.
Your current score is: 1/2

Q.3: Approximately one quarter of human bones are in the feet. (True/False): true
You got it right!
The correct answer was: True.
Your current score is: 2/3

Q.4: The total surface area of a human lungs is the size of a football pitch. (True/False): true
You got it right!
The correct answer was: True.
Your current score is: 3/4

...

Q.12: A few ounces of chocolate can kill a small dog. (True/False): true
You got it right!
The correct answer was: True.
Your current score is: 9/12

You've completed the quiz.
Your final score was: 9/12
```

---

### ✅ Key Highlights

- 🔧 **Object Oriented Design**  
  Utilizes a clean and extensible OOP structure with well defined classes (`Question`, `QuizBrain`, and externalized `data`) to encapsulate logic, responsibilities, and behavior.

- 🧠 **Real Time Logic & Validation**  
  Implements dynamic question iteration, answer checking, score tracking, and user feedback simulating an interactive quiz experience via the command line interface.

- 🎯 **Separation of Concerns**  
  Divides the core logic across multiple modules to promote code reusability, readability, and maintenance efficiency adhering to software engineering best practices.

- 🗂️ **Modular Architecture**  
  Each Python file is purpose built: `main.py` handles game flow, `data.py` stores trivia content, `question_model.py` defines question entities, and `quiz_brain.py` orchestrates logic.

- 🧪 **Foundational Python Mastery**  
  Reinforces practical applications of key Python concepts including classes, lists, loops, user input handling, conditionals, and data abstraction.

- 💻 **CLI Based Interaction**  
  Fully terminal driven interface offers a responsive user experience with immediate scoring and feedback.

---

### 🙌 Credits

This project was crafted as part of my structured journey toward mastering core Python programming concepts and object oriented design principles. It was developed under the mentorship of **Dr. Angela Yu** as part of the **“100 Days of Code: The Complete Python Pro Bootcamp”** a highly acclaimed and immersive program focused on building real world applications through modern Python practices.

Special appreciation goes to the open source community, educators, and mentors whose invaluable resources continually inspire cleaner code, modular thinking, and a passion for lifelong learning.
