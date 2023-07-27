
#Quiz App

This project is a React web application quiz. The user has to answer 10 questions from the "Biology" category, and their score is recorded and displayed in real time.

In the MainBody component, the useState and useEffect hooks are used to manage the application state and to make a request to the "Open Trivia Database" API to get the quiz questions. When the page loads, a single request is made to the API using axios.get and the results are stored in the info state using the setInfo function.

The questions and answers are displayed based on the info, number, and score states. If info has elements and number is less than the length of the question list, the next question and corresponding answer options are displayed. The answers are shuffled randomly before display.

When a response is selected, it is checked if it is correct by comparing it to the correct response of the current question. If the response is correct, number and score are updated using the set functions, otherwise only number is updated. Thus, the user moves on to the next question, and their score increases if they answered correctly.

When all questions have been answered or no question information is available, a quiz completion message and the final score are displayed. The user has the option to reset the quiz by clicking the "Reset" button, which reloads the page.

This project can be an interactive and fun way for users to test and improve their general knowledge.
