# Entry 4
### 04/25/2021

In this freedom project, my partner and I continued to explore [Firebase](https://firebase.google.com) and decided to use [firestore](https://firebase.google.com/products/firestore). We are currently trying to figure out how firestore works by following this [youtube video playlist](https://www.youtube.com/watch?v=4d-gIPGzmK4&list=PL4cUxeGkcC9itfjle0ji1xOZ2cjRGY_WB). We also continue making a workable to-do list by watching the [tutorial](https://www.youtube.com/results?search_query=javascript+firebase) mention that blog.

_________________

In this Engineering Design Process, I am in between steps "Plan the most promising solution" and "create a prototype." We found out that Cloud Firestore is more fitted for our project, which helps store the data and keep using the information they have input. firestore allows user to store their data in the cloud. It helps my freedom project "TO-DO LIST" because the user's task will automatically sync to the system. We (Nina and I) already start planning the base on HTML and Script.JS even though it is not fully completed yet.

_________________

I have decided to use **Firebase** for my freedom project as my final freedom project tool. At this moment, I am testing out the firestore database. I plan to create a workable **TO-DO LIST**. Testing firebase firestore allows me to store user's input more efficiently.

This is our current code below:

The first script tag allows us to make the code work in Firebase, allowing Firebase App Tools into HTML file. While the second script tag allows Cloud Firestore to be the feature and into inputs/HTML to go through. These two script tags code are essential in working with Firebase and firestore.
```HTML
<script src="https://www.gstatic.com/firebasejs/8.1.1/firebase-app.js"></script>
<script src="https://www.gstatic.com/firebasejs/8.2.1/firebase-firestore.js"></script>
```
 The script shown below is added into the HTML file from the Firebase service allowing Firebase to work in our repl.it.
```html
<script>
      var firebaseConfig = {
        apiKey: "AIzaSyBqpFbx2BD0gokHFkjG7_dgjTp_4F28RTU",
        authDomain: "firestore-testing-9095c.firebaseapp.com",
        databaseURL: "https://firestore-testing-9095c.firebaseio.com",
        projectId: "firestore-testing-9095c",
        storageBucket: "firestore-testing-9095c.appspot.com",
        messagingSenderId: "257330495741",
        appId: "1:257330495741:web:3f252dfece211887f5be94",
        measurementId: "G-S63PKJ1VQZ"
      };
      // Initialize Firebase
      firebase.initializeApp(firebaseConfig);
      firebase.firestore();
    </script>
```

The code below show our currently TESTING code we did:

```html
 <!-- input to-do task part -->
    <p class="header"> Task </p>
    <div class="container">
      <div class="the_task_container">
        <!-- Task -->
        <p id="usertext" type="text" placeholder="Start A Task"/></p> <!-- 4 place that the task will show up -->
        <div class = "the_task_data">
          <p id="the_task_title"> </p>
          <div id="the_task_tools">
            <button id="task_done_button" onclick="task_done();"> <i class="fa fa-check"> </i>  </button>
            <button id="task_edit_button" onclick="task_edit();"> <i class="fa fa-pencil"> </i>  </button>
            <button id="task_delete_button" onclick="task_delete();"> <i class="fa fa-trash"> </i>  </button>
          </div>
        </div>
      </div>
    </div>
    <!-- task finish -->
    <p class="header" > Finish Task </p>
    <div class="container">
      <div class="task_container">
        <div class = "task_data">
          <p id="task_title">Task Title 1 </p>
        </div>
      </div>
    </div>
```

The code above demonstrates buttons for the task to edit, delete or mark task done. Our current plan is to make the to-do list easier to use. We also include a selection for "Finish Task." Although this is our testing code, we are still trying to make the most efficient to-do list possible.


```js
var db = firebase.firestore();
db.collection("lists")get().then((doc) => {
})

//4
function data() {
  var text = prompt("Start a task");
  document.getElementById('usertext').innerHTML = text;
  console.log(text);
}
data();

function add_task(){
  console.log("add_task");
}
function task_done(){
  console.log("task_done");
}
function task_edit(){
  console.log("task_edit");
}
function task_delete(){
  console.log("task_delete");
}
```
The code line 1-2 above allows us to know which know collection document we want to grab. Although the code above is incomplete, we are still trying to figure out how it works. I learn that .get() and doc are very important in firestore because they will get the document information from the firestore. In other words, it will get the data from Firestore and apply it to the HTML as I'm currently researching more about it.

(TO BE UPDATED BY TOMORROW MORNING, STILL DOING IN THE PROCESS OF DOING THE CODE BELOW RIGHT NOW). 

_________________

In planning for my MVP with my partner Nina, we are still learning what firestore is and how it works. Although I'm are still confused about firestore, we want to continue to self-teach and cooperate with our project. We are also in the step of adding more HTML and CSS and testing trial and error. Although we make the input/entering task work by prompt and save the user's input. We are in the process of trying to make the buttons work as we wanted, so these are our next step plan.

_________________

The skills I use are **Debugging**, **Problem Decomposition**, and **Time Management**. Problem Decomposition allowed me to understand the topic in different parts quickly. Since I struggle to learn about Firebase and firestore, I break the topics into small parts to know. Although it seems time-consuming, I want to fully understand how firebase/firestore works as it plays a significant role in my project. Debugging helps me know how the code is not going to be workable the first time. I have to debug the code with patience as I have so many trials and errors. I have to watch multiple videos to understand the basic idea of firebase/firebase. One of these [video](https://www.youtube.com/watch?v=2Vf1D-rUMwE) has helped me understand firestore, as well as the [this video](https://www.youtube.com/watch?v=4d-gIPGzmK4&list=PL4cUxeGkcC9itfjle0ji1xOZ2cjRGY_WB) I have mentioned earlier. Time management is another skill I learn this process. I have to learn to time manage more effectively since I don't want to cram all my idea into the project. Even though time management is hard for me right now, I have to find time to work on this project and find time for doing school work. In this process, I leave a day of the week to focus on studying what firestore is and how it works. I try to follow the tutorial I found on google and youtube to understand what is going on. Time management allows me to spend time on the topic I'm not sure about with breaks in between instead of letting all the big topics into my brain and forcing myself to understand. 


[Previous](entry03.md) | [Next](entry05.md)

[Home](../README.md)