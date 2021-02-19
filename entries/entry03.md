# Entry 3
##### 02/10/2021

Today I continue to explore [Firebase](https://firebase google com) from the [Freedom Project Tool list](https://docs google.com/document/d/1oJFrErlAZvB-0V923QGOm4X3CwiceJsKot2R6Jz8Mdc/edit) by learning deeper about Firebase, as well as continuing to test some code out I made my final decision to use [Firebase](https://firebase google.com) as my final Freedom Project tool  I also continue to explore and learn "how to make" my freedom project, to-do list by watching this [youtube tutorial](https://www.youtube com/results?search_query=javascript+firebase) 
_________________
In my previous Engineering Design Process, I have already defined the problem of creating my project, which is the struggle of students and adults forgetting their tasks  To solve that problem, I research the tool and know how it can apply to my project  I also think about the solutions that can help to correspond to solve real-life problems  
<br>
Through the Engineering Design Process, I am still researching Firebase and how Firebase can help me build my project  This time, I learn from [this website](https://firebasetutorials.com/what-can-firebase-do/) that Firebase has four categories Develop, Quality, Analytics, and Grow  I focus on the first half of the main category Develop, which contains Authentication, Database, and Storage 
<br> 
Authentication considers as registration for your apps such as username/email and password  The database is considered as storage, or accessible for your data  There are two types of databases: Real-time database and Cloud Firestore  Both databases help to sync and storage the data  The "Storage" helps the user to store the information/task they have input  I found this very important to my project because user's task(s) needs to be store for the user to keep their task(s) in mind (In the following paragraph 2 would fully explain my knowledge of the category Develop in firebase)  
<br>
At the same time, I am also in the "Steps of brainstorming" even more possible and started to plan the most promising solution of my project  To create a project with firebase isn’t easy, and I need to think of more possibilities for others to use my **to-do list**  I also start planning my project with my partner, Nina Li  We first started to plan the base of our project (HTML and SCRIPT JS) with the help of the [youtube tutorial](https://www youtube.com/results?search_query=javascript+firebase)  
_________________
To explain the category Develops that contains Authentication, Database, and Storage from paragraph four: 
Authentication considers as registration for your apps such as username/email and password  The idea of Authentication such as sign-in/log-in for our social media or email that interact daily  I don't think I need it, for now, I think it will be helpful in the future  
There are two types of databases, as I stated above paragraph: Real-time database and Cloud Firestore  Both databases help to sync and storage the data  
The Real-time Database means when you add some data into your Firebase app, and it will instantly be added into the Firebase Realtime Database  To cooperate in society (given example from the website) such as text message, you send some text and instantly through the real-time database, database informs the user of the text message from the notification 
The Cloud Firestore allows you to store your data in the cloud  It can sync across all your devices and share them among multiple users  Cloud Firestore helps my freedom project of a "TO-DO List" by allowing the user to input their task easily  The tasks that the user put would automatically be placed  
The "Storage" helps the user to store the information/task they have input  I found this very important to my project because the task needs to be store for the user to keep in mind  Without storage, there's no point in using my project, if it only one-time use  Firebase would allow the user and me to store the information  Take google Doc, as an example, every time the user refreshes the page/re-enter the google doc, and their information would still be store and sync without anything removed or reset 
<br>
</br>
I have decided to use **Firebase** for my freedom project as my final freedom project tool  Right now, my main focus is to plan and build a **TO-DO List**  I learn that Firebase helps me store my users' to-do tasks  Whenever my users can come back to/refresh the page, they can mark tasks as completed, or they can add more tasks to the list 
A TO-DO List helps students, like me, allows us to keep up with their tasks while adults can use it for anything such as a grocery list or keep their tasks in one place  My idea of a to-do list is minimalist and easy to use without having distractions compare to other TO-DO List that is cause confusion and complication  
<br>
</br>
_________________
In this code shown below (is the continuation/additional input of the code from the previous entry), the <body> section contains a title of the task selection using the code ```<p class="header"> Task </p>```(line 1)  ``` <div class="container">
<div class="the_task_container">``` the following 2 lines shows the class containers for the code that will be explain in the following code snippet  In the next following 2 lines of code helps us introduce the button for the task ```<div class = "the_task_data">
<p id="the_task_title"></p>``` The div tag helps contain the task title, which is a placeholder when you enter your task  ```<div id="the_task_tools">``` (line 6) is demonstrate the tools options such as done, edit, and delete  ``` <button id="task_done_button" onclick="task_done();"> <i class="fa fa-check"> </i> </button>``` (line 7) demonstrate a placeholder check mark emoji, which is known as “ <i class="fa fa-check”>”  This button allows the user to click and mark their task as done  ```<button id="task_edit_button" onclick="task_edit();"> <i class="fa fa-pencil"> </i> </button>```(line 8) allows user to click and edit the task based on the “<i class="fa fa-pencil”>” (a pencil emoji)  Finally the ```<button id="task_delete_button" onclick="task_delete();"> <i class="fa fa-trash"> </i> </button>``` (line 9) allows user to delete their task off the list  Line 13-18 ```<p class="header" > Finish Task </p>
<div class="container">

<div class="task_container">
<div class = "task_data">
<p id="task_title">Task Title 1 </p>
</div>``` show the lines of “Finish Task” which have a container of the with a placeholder task title  This means that after your task is completed, the task will fall into the “Finish task” section  

<br>
<br>
The code shown below will show the full code we have done 
```
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
```
```
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
<br>
Based off from the video, we also add  
```function data() {
var text = document getElementById("usertext") value;
console log(text);
}
```

In SCRIPT JS  After you write a task and click enter, the input will be store in the console log  the following 3 lines in the SCRIPT.JS

```
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
The code in the SCRIPT JS helps to store the function of the button  If the user wants to mark the task done using the button of the placeholder checkmark, it will store the function of the button “done”  By pressing the checkmark button, It'll also show “task_done” in the console log  Since this is our testing code, this code is the base foundation that helps us to keep up the function for the next step of the project (even if the code doesn't fully work yet) 
<br>
</br>
_________________
The skills I used are How to Google, How to read, debugging, and embrace failure. My skill in how to google has helped me find the basic idea about Firebase. When I search "What can firebase do?", Google provided me a lot of informational sites/blogs such as [this blog page](https://blog.back4app.com/firebase/), which that talk about the background history and information about firebase. Through this skill, I learn how to search and read by the filter (command-F) to find relevant information and skimming through the page. Learning “How to read” have to help me gain knowledge about Firebase. From [this page](https://firebasetutorials.com/what-can-firebase-do/), I learned that Firebase has four categories, Develop, Quality, Analytics, and Grow. I already talk about the first half of the first categories, Develop, above. Through google, I continue to follow the [youtube turtorial](https://www.youtube.com/watch?v=pSVHDk4hK8Y) and continue to tinkling my project. As I developed a basic knowledge/foundation of my project code, I learn how to debug multiple codes out. It causes me to embrace failure codes and continue to debug till the code work. Although it is a frustrating situation, to have a decent project in the end, I have to face failure as not every code will work as you wanted. I think the skills "How to Google" and "How to read" have to help me know the basic history or summary of my project. The skills “debugging” and “embrace failure” will also appear a lot on my journey on this creative project. It allows me to use them for my future steps as I continue to be in the process of building this project.



[Previous](entry02.md) | [Next](entry04.md)

[Home](../README.md)