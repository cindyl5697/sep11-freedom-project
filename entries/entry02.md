# Entry 2
### 11/30/2020

Today I explored [Firebase](https://firebase.google.com) from the [Freedom Project Tool list](https://docs.google.com/document/d/1oJFrErlAZvB-0V923QGOm4X3CwiceJsKot2R6Jz8Mdc/edit) that may help me determine final my freedom tool. I notice how [Firebase](https://firebase.google.com) can help me build my Freedom Project with the help from [youtube tutorial](https://www.youtube.com/results?search_query=javascript+firebase).

Through the Engineering Design Process, I have defined my problem of creating my project, which is the struggle of students and adults forgetting their tasks. To solve the problem, I research the tool I'm using and how it can apply to my project as well as how it can solve real-life problems. Therefore I need to learn about Firebase and how Firebase can help me build my project. I learn that Firebase is storage that helps the user to keep their information. For example, Duolingo, a language site/app that uses Firebase, where the user would use Duolingo to practice their language skills through different levels. As they passed each "level" of language skills, Firebase would store the user's information and "score level" that helps to user to move on to a new "level"; as well as storing user's information after the user exit the site/app. Firebase helps the user refresh the page/re-enter the app, and their language skill "level" would still be there without anything removed or reset. I'm also on the first step of brainstorming how my project is going to solve the problem. For me to create the project with **Firebase**, I have to think of multiple possibilities for others to use my project, which is a **to-do list**.
<Br>

In this code shown below, the <body> section contains the title of the project using the code ```<h1> Testing Firebase </h1>```.  To test out the "Enter" button and our input, we start off using  ```<form placeholder = "text"> </form>```(line 3 of the code) follow by an input tag ```<input id = "usertext" type="text" placeholder = "Enter your text"> </input>```(line 4), which shows that the user can type input or the task they put. After the input tag in line 4, we use the button tag in line 5 ```<button id="button" onclick="data()"> Enter </button>```  to show that once the user inputs their task and click the button, their inputs task would be in the console.log. Although this is our testing code, we would this code something that we have in mind for the project.
<br>

```
<body>
 <h1> Testing Firebase </h1>
 <form placeholder = "text"> </form>
 <input id = "usertext" type="text" placeholder = "Enter your text"> </input>
 <button id="button" onclick="data()"> Enter </button>
 <script src="https://www.gstatic.com/firebasejs/8.1.1/firebase-app.js">
</script>
 <script src="https://www.gstatic.com/firebasejs/8.1.1/firebase-analytics.js"></script>
 <script>
 var firebaseConfig = {
 apiKey: "AIzaSyCCIdGo1CZ8uUnUrmeo-vwfQgkr3PLs4R0",
 authDomain: "tinkering-52eea.firebaseapp.com",
 databaseURL: "https://tinkering-52eea.firebaseio.com",
 projectId: "tinkering-52eea",
 storageBucket: "tinkering-52eea.appspot.com",
 messagingSenderId: "102162150983",
 appId: "1:102162150983:web:340d7b6fceb0b17134e362",
 measurementId: "G-XCRFENWZWE"
 };
 // Initialize Firebase
 firebase.initializeApp(firebaseConfig);
 firebase.analytics();
 </script>
```
<br>

The last three set of Javascript code are from firebase to help us make the testing product clickable, as shown below:
``` <script src="https://www.gstatic.com/firebasejs/8.1.1/firebase-app.js">
</script>
 <script src="https://www.gstatic.com/firebasejs/8.1.1/firebase-analytics.js"></script><script>
 var firebaseConfig = {
 apiKey: "AIzaSyCCIdGo1CZ8uUnUrmeo-vwfQgkr3PLs4R0",
 authDomain: "tinkering-52eea.firebaseapp.com",
 databaseURL: "https://tinkering-52eea.firebaseio.com",
 projectId: "tinkering-52eea",
 storageBucket: "tinkering-52eea.appspot.com",
 messagingSenderId: "102162150983",
 appId: "1:102162150983:web:340d7b6fceb0b17134e362",
 measurementId: "G-XCRFENWZWE"
 };
 // Initialize Firebase
 firebase.initializeApp(firebaseConfig);
 firebase.analytics();
 </script>
 ```

<br>
I have decided to use ***Firebase*** for my freedom project as my final freedom project tool. For now, my main focus is to build a ***To-do List.*** Since my focus right now is creating a to-do list, Firebase helps me store my users' to-do tasks into the list, so whenever my users can come back to/refresh the page, they can mark tasks as completed, or they can add more tasks to the list. I think making a to-do list (and a timer on the side) can help everyone. Students, like me, can use it as a way to study and keep up with their tasks while having a study timer to track time. Adults can use it as an ingredient or grocery list, and a timer can help them keep aware of their cooking time or any timer usage. Although there are many to-do list apps out there, I want to make sure my to-do list is simple and easy to use for everyone. A lot of to-list contains grouping (where you have to categorize your to-do tasks), having able to comments on your task bullet point, timed due date, or task completion percentage. My idea of a to-do list is minimalist and easy to use without having distractions. I want my product to have a clear and clean visual that easy to use and doesn't need too much thought while putting your task into the application (To-Do list title, add tasks in bullet point form, and an optional due date).

<br>
</br>

The skills I used are How to Google and How to read. My skill in how to google has helped me learn the basic idea about Firebase or youtube tutorials for my project. When I first search ["What is Firebase Javascript"](https://www.google.com/search?safe=strict&client=safari&rls=en&ei=LIHFX9uwFeGv5NoP2ZaEiAI&q=what+is+firebase+javascript&oq=what+is+firebase+javascript&gs_lcp=CgZwc3ktYWIQAzICCAA6BAgAEEc6BAgAEA06BggAEAcQHlCeTVjXV2CtWmgAcAF4AIABWYgB-wSSAQE4mAEAoAEBqgEHZ3dzLXdpesgBCMABAQ&sclient=psy-ab&ved=0ahUKEwjb9pvytqvtAhXhF1kFHVkLASEQ4dUDCAw&uact=5), Google provided me a lot of informational sites, such as explaining the basics of Firebase from [this article author's experience](https://medium.com/firebase-developers/what-is-firebase-the-complete-story-abridged-bcc730c5f2c0). Through this skill, I learn how to search and filter (command-F) for relevant information about my project. Learning how to google also helps me find this amazing [youtube tutorial](https://www.youtube.com/watch?v=pSVHDk4hK8Y) about how to create a to-do list. The skill of "How to read" is another thing that connects to How to google. To know how to read is the key to finding relevant information about my project [This site](https://medium.com/firebase-developers/what-is-firebase-the-complete-story-abridged-bcc730c5f2c0) that I previously introduced has helped me knows the basics information about firebase and how firebase works. I think the skills "How to Google" and "How to read" have to help me know what my project is going to be about and use them for my future steps in the process of building this project.

<br>


[Previous](entry01.md) | [Next](entry03.md)

[Home](../README.md)