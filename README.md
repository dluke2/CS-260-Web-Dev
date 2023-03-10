# CS-260-Web-Dev
CS 260 Web Dev for Winter 2023

Startup Application:

Sales Pitch:
Have you ever tried to split the cost of something, when several people paid for it? For example, difficulty can arise when separate people have booked lodging or paid for food during a trip. The Expense Splitter application makes it so groups of people can record expenses for an event, then calculate the amount each person needs to pay to even out the expenses across the group. Once the calculation is complete, the group can be sure that everyone has paid their fair contribution to the event.

Key Features:
- Secure login over HTTPS
- Ability for admin to create new and delete old events
- Ability for admin to add or remove participants from events
- Ability for participants to input expenses (description and amount)
- Ability to edit expenses
- Live calculations
- Store results

![Application - Main](https://user-images.githubusercontent.com/123618573/215209048-bc01d015-4123-4ad0-a337-a219b43b9db4.jpg)
![Application - Manage](https://user-images.githubusercontent.com/123618573/215209121-e9910ad6-1804-457b-b159-fa90c5d52f93.jpg)
![Application - Add](https://user-images.githubusercontent.com/123618573/215209160-ff436334-4a9f-45a2-add0-712b99e29bef.jpg)
![Application - Calculations](https://user-images.githubusercontent.com/123618573/215209180-bedaacd8-b0cb-40de-9b3f-1b8d69bc4921.jpg)

AWS:
User name: dluke2 /n
My server's IPv4 address: http://18.223.130.210/
REMINDER - Release elastic IP for my instance at end of class

Caddy:
Learning VI is a much faster way of opening and making edits to files. It also doesn't require me to download things off of a server, then pushing changes.

Simon/HTML:
There are so many ways to do similar things in HTML. For example, I tried looking into the difference between menu and ul, and they can be used for the same things, although menu should be used for hyperlinks. I also realized the importance of seeing changes in real time. My live connection would pull up a file directory rather than the html page, so I need to get that figured out. I instead had to use CodePen, then copy the html back into VS Code, which was annoying because VS code has better completion. Using the right tools for the job makes it a lot easier.

CSS:
Making something visually appealing was difficult. I ended up just making a monstrosity to practice. However, I learned the value of understanding color combinations and proportions, as it was a lot more difficult than I expected to make something visually appealing.

Simon CSS: Just getting a base for head, body, and footer are important. Once that is in place, everything should fit well. A good way to do this is to set the header and footer with flex: 0, and the body at flex: 1. Using bootstrap can make customization difficult.

DOM is going to be vital for my project. The code here https://codepen.io/dluke2/pen/MWqpooM?editors=1010 will help me with my startup application. I'll need to learn to read in inputs, then edit arrays with the information to modify the table.

Simon-CSS: Reading in inputs is interesting. To disply what has already been inputed, I need to use the following structure. The .player_name is a class. The following JavaScript shows how to capture and display data.

function login() {
  const nameEl = document.querySelector("#name");
  localStorage.setItem("userName", nameEl.value);
  window.location.href = "play.html";
}

    const playerNameEl = document.querySelector('.player-name');
    playerNameEl.textContent = this.getPlayerName();
    
Startup JavaScript: I struggled to make this work, I ended up having to change the way I wanted to do things. I struggled a lot with the math elements. I wanted to assign who would pay who, but this became a mess. It was easier just to determine how much everyone owed, which reduces the usefulness of the calculator. 
Luckily, the assignments we had in CodePen helped me figure out how to create the table and helped a lot. I stubbled across the contenteditable=true feature, which made capturing data easier. I started to use a lot of forms, but that got messy. I learned that getMonth() returns the letter, so I made an array instead to get the month name.
