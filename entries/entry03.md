# Entry 3
### 02/10/2021

Today I continue to explore [Firebase](https://firebase.google.com) from the [Freedom Project Tool list](https://docs.google.com/document/d/1oJFrErlAZvB-0V923QGOm4X3CwiceJsKot2R6Jz8Mdc/edit) by learning deeper about Firebase, as well as continuing to test some code out. I made my final decision to use [Firebase](https://firebase.google.com) as my final Freedom Project tool.  I also continue to explore and learn "how to make" my freedom project, to-do list by watching this [youtube tutorial](https://www.youtube.com/results?search_query=javascript+firebase).

_________________

In my previous Engineering Design Process, I have already defined the problem of creating my project, which is the struggle of students and adults forgetting their tasks. To solve that problem, I research the tool and know how it can apply to my project. I also think about the solutions that can help to correspond to solve real-life problems.
<br>
___

Through this Engineering Design Process, I am still researching Firebase and how Firebase can help me build my project. This time, I learn from [this website](https://firebasetutorials.com/what-can-firebase-do/) that Firebase has four categories Develop, Quality, Analytics, and Grow.  I focus on the first half of the main category Develop, which contains Authentication, Database, and Storage.
<br>

Authentication considers as registration for your apps such as username/email and password. The database is considered as storage, or accessible for your data. There are two types of databases: Real-time database and Cloud Firestore. Both databases help to sync and storage the data. The "Storage" helps the user to store the information/task they have input.  I found this very important to my project because user's task(s) needs to be store for the user to keep their task(s) in mind (In the next two paragraphs, I would fully explain my knowledge of the category Develop in firebase).
<br>

 At the same time, I am also in the "Steps of brainstorming" even more possible and started to plan the most promising solution of my project.  To create a project with firebase isn’t easy, I need to think of more possibilities for others to use my <b>to-do list</b>.  I also start planning my project with my partner, Nina Li. We first started to plan the base of our project (HTML and SCRIPT.JS) with the help of the <a href="https://www.youtube.com/watchI ?v=pSVHDk4hK8Y"> youtube tutorial</a>.
<br>

_________________

To explain the category Develops that contains Authentication, Database, and Storage from paragraph four:
<br>
Authentication considers as registration for your apps such as username/email and passwords. The idea of Authentication such as sign-in/log-in for our social media or email that interact daily. I do not think I need it for my project.
There are two types of databases, as I stated above paragraph: Real-time database and Cloud Firestore. Both databases help to sync and storage the data.
<br>

The Real-time Database means when you add some data into your Firebase app, and it will instantly be added into the Firebase Realtime Database. To cooperate in society (given example from the website) such as text message, you send some text and instantly through the real-time database, database informs the user of the text message from the notification.
<br>

The Cloud Firestore allows you to store your data in the cloud. It can sync across all your devices and share them among multiple users. Cloud Firestore helps my freedom project of a "TO-DO List" by allowing the user to input their task easily. The tasks that the user put would automatically be placed.
<br>

The "Storage" helps the user to store the information/task they have input. I found this very important to my project because the task needs to be store for the user to keep in mind.  Without storage, there's no point in using my project if it only one-time use. Firebase would allow the user and me to store the information. Take google Doc, as an example, every time the user refreshes the page/re-enter the google doc, and their information would still be store and sync without anything removed or reset.
<br>
_________________

I have decided to use **Firebase** for my freedom project as my final freedom project tool. Right now, my main focus is to plan and build a **TO-DO List**.  I learn that Firebase helps me store my users' to-do tasks. Whenever my users can come back to/refresh the page, they can mark tasks as completed, or they can add more tasks to the list. I am also in the process of learning the difference between a real-time database and a firestore. 
A TO-DO List helps students, like me, allows us to keep up with their tasks, while adults can use it for anything such as a grocery list or keep their tasks in one place. My idea of a to-do list is minimalist and simple to use without having distractions compare to other TO-DO List that is cause confusion and complication.
<br>

_________________

This code shown below is the continuation/additional input of the code from the previous entry (An explanation of the code).
<br>
</br>
The <body> section contains a title of the task section (line 1), and line 2 + 3 <div> tags help to contain the following lines of code:
```HTML
<p class="header"> Task </p> // line 1 
```
``` HTML
<div class="container"> // line 2 
<div class="the_task_container"> line 3
```
Line 4 and 5 help us introduce the button for the task.
```HTML
<div class = "the_task_data"> // line 4
<p id="the_task_title"></p> // line 5
```

Inside div tag helps contain the tools of done, edit, and delete icons shown below.
```HTML
<div id="the_task_tools"> //line 6
            <button id="task_done_button" onclick="task_done();"> <i class="fa fa-check"> </i>  </button> // line 7
            <button id="task_edit_button" onclick="task_edit();"> <i class="fa fa-pencil"> </i>  </button> // line 8
            <button id="task_delete_button" onclick="task_delete();"> <i class="fa fa-trash"> </i>  </button>// line 9
``` 
Line 6 demonstrates the div tag that will contain the tool buttons such as done, edit, and delete.
Line 7 demonstrates a button that allows the user to click and mark their task as "done" using the placeholder checkmark icon, ```<i class="fa fa-check”>”```
Line 8 allows the user to click and edit the task with the button of a pencil icon. ```<i class="fa fa-pencil”>```
Line 9 allows user to delete their task off the list with the button that would show a trash icon. ```<i class="fa fa-trash”>``` 

The lines of “Finish Task” have a container with a placeholder task title.
It means that after your task is completed, the task will fall into the “Finish task” section.
Line 13-21 below:
>
```HTML
<p class="header" > Finish Task </p> //line 13 
<p class="header" > Finish Task </p> //line 14
    <div class="container"> // line 15
      <div class="task_container"> // line 16
        <div class = "task_data"> // line 17
          <p id="task_title">Task Title 1 </p> // line 18
        </div> // line 19
      </div> // line 20
    </div> // line 21
```

Based off from the [youtube tutorial](https://www.youtube.com/results?search_query=javascript+firebase), we also add the code below demostrates that when the user input a task and press "Enter", the input would appears on the console.log.
```javascript
function data() {
var text = document getElementById("usertext") value;
console log(text);
}
```

The following three lines in the SCRIPT.JS, After you write a task and click enter, the input will be store in the console.log:

```javascript
function add_task(){
console log("add_task");
}
function task_done(){
console log("task_done");
}
function task_edit(){
console log("task_edit");
}
function task_delete(){
console log("task_delete");
}
```

The code in the SCRIPT.JS helps to store the function of the button. If the user wants to mark the task done using the button with the checkmark; it will store the function of the button “done, and show “task_done” in the console.log.  It is our testing code, so the code is the base foundation that helps us to keep up the function for the next step of the project. For now, the code doesn't fully work yet.
<br>
</br>
_________
Here is the codes that we have currently done/explain: 
````HTML
HTML:
<!--input to-do task part-->
<p class="header"> Task </p>
<div class="container">
<div class="the_task_container">
<div class = "the_task_data">
<p id="the_task_title"></p>

<div id="the_task_tools">
button id="task_done_button" onclick="task_done();"> <i class="fa fa-check"> </i> </button>
<button id="task_edit_button" onclick="task_edit();"> <i class="fa fa-pencil"> </i> </button>
<button id="task_delete_button" onclick="task_delete();"> <i class="fa fa-trash"> </i> </button>
</div>
</div>
<!--task finish-->
<p class="header" > Finish Task </p>
<div class="container">

<div class="task_container">
<div class = "task_data">
<p id="task_title">Task Title 1 </p>
</div>
````

```javascript
SCRIPT JS:
function data() {
var text = document getElementById("usertext") value;
console log(text);
}
function add_task(){
console log("add_task");
}
function task_done(){
console log("task_done");
}
function task_edit(){
console log("task_edit");
}
function task_delete(){
console log("task_delete");
}
```
_________________
The skills I used are How to read and debug/debugging. My skill in how to read by the filter (command-F) allows me to find relevant information. It also leads me skims through the page more quickly without spending too much time on irrelevant ideas. From [this website](https://firebasetutorials.com/what-can-firebase-do/) and skims through the page, I learned that Firebase has four categories, Develop, Quality, Analytics, and Grow. I already talk about the first half of the first categories, Develop, above. 

As I developed a basic knowledge/foundation of my project code, I learn how to debug multiple codes out. I continue to follow the [youtube turtorial](https://www.youtube.com/watch?v=pSVHDk4hK8Y) and continue to tinkling my project. Although it is frustrating to debug the code, I realized that debugging codes makes my future coding more easily and effectively for my project. The skills "How to read" have to help me learn more basic history or summary of my project as the skills “debugging” will also appear a lot on my journey on this creative project. It allows me to use them for my future steps as I continue to be in the process of building this project.

_________________


[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)