# Entry 5
##### 06/18/2021


In this freedom project, my partner and I are in the process of finishing our Freedom Project, TODO List using [Firebase](https://firebase.google.com). We decided to use [firestore](https://firebase.google.com/products/firestore) for our project. We are following this [youtube video playlist](https://www.youtube.com/watch?v=4d-gIPGzmK4&list=PL4cUxeGkcC9itfjle0ji1xOZ2cjRGY_WB) that help us incorporate our code to Firebase. 

_________________

In this Engineering Design Process, I am in the steps of "Test and evaluate the prototype", "Improve as needed", and "Communicate the results". Cloud Firestore is our fitted database to collect and store the task inputs. As I previous mention, Firestore allows user to collect and store their data in the cloud. It helps my freedom project "TO-DO LIST" because the user's task will automatically stored to the system. We (Nina and I) already created the base of Javascript. We also incoperate Firebase into our code by following youtube video playlist.  Throughout our process of finishing the Javascript and incoperate firebase, we encounter many errors. As we connect our code into firebase, we have difficulties making our task button save/delete the task in the beginning. After doing many error trials, we finally got to make our code connect to firebase. As we finish the code, I also communicate with my partner, Nina, to improve our TODO List. Since time run short, we decided to make a simple TODO List with simple design.

_________________

I am using **Firebase** for my freedom project as my final freedom project tool. This time, I am creating a firebase code that allows me to incoperate fireabase into my project and store user's input more efficiently.

Since we have make a workable TODO List, here is a code snippets explain our a part our TODO List. 
```JS
function toDo(text){
  var output = document.createElement('p'); 
 
 ```
↑The code above show that we created a function call toDO and its parameter (text) that helps us make the functions/actions work. 


 ```JS
  // adds task to todo
  document.querySelector('#todo').appendChild(output);
  
  // check icon
  var checkIcon = document.createElement('span');
  output.appendChild(checkIcon);
  checkIcon.classList.add('gg-check-r');
    
  // trash icon
  var trashIcon = document.createElement('span');
  output.appendChild(trashIcon);
  trashIcon.classList.add('gg-trash');
  ```

↑The code above is the add, complete, and delete icons. 

```JS
  // when trash icon is clicked, deletes task
  var allTrash = document.querySelectorAll('.gg-trash');
  allTrash.forEach(function(allTrash, trashIcon){
    allTrash.addEventListener("click",function(event){
  var remove = event.target.parentElement;
      remove.style.display = "none";
```
    
↑To set an example of making the icon work, we use a loop function, in the code above, to that allow the user to click on the trash button and their task would be deleted. 

```JS
      db.collection("todolist").get().then((snapshot) => {
        snapshot.docs.forEach(doc => {
          console.log(remove);
        });
      });
    });
  });
```
↑(Code above) At the same time, when the user clicked on the trash icon, the user's input task(s) is deleted in both Google Firebase and the page. This demonstrates that whenever the user refreshes the page, their deleted task would disappear. 

```JS 
output.innerHTML += text; 
```
  
↑The output makes a "p" tag, which means whenever the user inputs the task through the add button, ```output.innerHTML += text``` allows users to input and add their task into the TODO List. 
_________________



_________________




[Previous](entry04.md) | [Next](entry06.md)

[Home](../README.md)