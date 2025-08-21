A lightweight and interactive Quiz Plugin for websites and applications. Built with HTML, CSS, and JavaScript, it allows you to easily embed customizable quizzes to engage your users, test knowledge, or collect feedback.

Features

 Multiple Choice Questions – Supports single or multiple correct answers.

 Auto Scoring – Tracks user score in real-time.

 Modern UI – Clean, responsive, and mobile-friendly design.

 Reusable Plugin – Easily integrate into any project with minimal setup.

 Next/Previous Navigation – Smooth flow between questions.

 Final Score Display – Shows results at the end of the quiz.

 Customizable – Add your own questions, answers, and styles.

 Installation

Download or clone this repository.

Include the plugin files in your project:

<link rel="stylesheet" href="quiz.css">
<script src="quiz.js"></script>


Add a container for the quiz:

<div id="quiz-plugin"></div>
<script>
  initQuiz("quiz-plugin", {
    theme: "dark",
    shuffleQuestions: true,
  });
</script>


That’s it! The quiz is ready to run. 

 Usage

Add your questions inside quiz.js (or load from a JSON file).

Each question contains:

question → The question text.

answers → Array of answer choices with text & correct.

Example:

const questions = [
  {
    question: "Which one is the largest animal in the world?",
    answers: [
      { text: "Shark", correct: false },
      { text: "Blue Whale", correct: true },
      { text: "Elephant", correct: false },
      { text: "Giraffe", correct: false }
    ]
  }
];

 Plugin Options

You can customize the quiz behavior with options:

Option	Type	Default	Description
theme	string	light	"light" or "dark" theme
shuffleQuestions	boolean	false	Randomize question order
shuffleAnswers	boolean	true	Randomize answer options
showScore	boolean	true	Show score at the end
 Example
<div id="my-quiz"></div>
<script>
  initQuiz("my-quiz", {
    theme: "light",
    shuffleQuestions: true,
    showScore: true
  });
</script>

 Technologies Used

HTML5

CSS3 (modern styling + animations)

JavaScript (ES6)

 Roadmap

 Basic quiz with scoring

 Next/Previous navigation

 Timer-based quizzes

 Question categories (e.g. Science, History, Tech)

 Export quiz results
