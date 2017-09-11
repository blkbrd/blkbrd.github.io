---
layout: post
title: "Fun with Processing"
date: 2017-09-10
---

I decided to play with Processing just to brush up on my coding skills. I much prefer scripting. I stole my brother's homework and made some changes. I will update as I make it better!
<code> 
  
/* Edits on Robert Warner's Pong Game 8/30/2017
stopped paddles from escaping the playing space
added random board color to each time a point is scored
allowed ball to go any direction after point is scored
*/

float x = 400;

float y = 400;

float alt = -1;

float delX = random(3, 5);

float delY = random(2, 3);

float rect1Y = 350;

float rect2Y = 350;  

int score1 = 0;

int score2 = 0;

boolean player2Down = false; 

boolean player1Down = false;

boolean player1Up = false; 

boolean player2Up = false; 

float colors1 = 255;

float colors2 = 0;

float colors3 = 0;

void setup() {
  //creates play space

size (800, 800);

}

void draw() {

  //colors background, draws ball and center line

background(colors1, colors2, colors3);

fill(0, 0, 255);                                //color of paddles/ball

ellipse(x=x+delX, y=y+delY, 25, 25);

line(400, 0, 400, 800);



//if ball passes left boundary wall, increment score and reset position     

if (x<=0) {

score2++;

x = 400;

y = 400;

delX =  random(3, 5);                       //randomizes the magnitude between 3 and 5

delX = delX * random(-1, 1);                //randomizes the direction

delY =  random(2, 3);

delY = delY * random(-1, 1);                //randomizes the direction

colors1 = random(0, 255);                   //randomizes the background color

colors2 = random(0, 255);

colors3 = random(0, 255);

}

//if ball passes right boundary wall, increment score and reset position

if (x>=800) {

score1++;

x = 400;

y = 400;

delX = random(3, 5);

delX = delX * random(-1, 1);                //randomizes the direction

delY = random(2, 4);

delY = delY * random(-1, 1);                //randomizes the direction

colors1 = random(0, 255);

colors2 = random(0, 255);

colors3 = random(0, 255);

}



//draws text to screen

textSize(25);

text("Warner Pong", 325, 25);

text("Player 1 Score", 5, 25);

text(score1, 5, 55);

text("Player 2 Score", 625, 25);

text(score2, 770, 55);



//draws pong paddles

rect(0, rect1Y, 20, 100);

rect(780, rect2Y, 20, 100);



//logic for pong ball hittle paddle

if (x<32.5 && y>rect1Y && y<rect1Y+100) {

delX = -1.1 * delX;                        //reverse direction, speed up slightly

}



//logic for pong ball hittle paddle     

if (x>767.5 && y>rect2Y && y<rect2Y+100) {

delX = -1.1 * delX;                        //reverse direction, speed up slightly

}



//logic for pong ball hitting top or bottom wall

if (y>787.5 || y<12.5) {

delY = -1 * delY;                          //reverse direction

}

}



void keyPressed() {



//poll to see if key pressed; set boolean flag

if (key == 'q' || key == 'Q') {

player1Up = true;

}

if (key == 'a' || key == 'A') {

player1Down = true;

}

if (key == 'p' || key == 'P') {

player2Up = true;

}

if (key == 'l' || key == 'L') {

player2Down = true;

}



//give player one an opportunity to move, then give player2 an opportunity to move

//move player one if flag set

if (player1Up == true) {

if (rect1Y <= 0) {                                     //check to see if pong paddle is hitting the top wall

rect1Y = 0;                                          //dont let it move past the edge of the play space

} else {

rect1Y -=20;                                         //otherwise, let it move

}

player1Up = false;                                     //reset "move up" flag to false

} else if (player1Down == true) {

if (rect1Y >= 707.5) {

rect1Y = 707.5;

} else {

rect1Y += 20;

}

player1Down = false;

}

//move player 2 if flag set

if (player2Up == true) {

if (rect2Y <= 0) {

rect2Y = 0;

} else {

rect2Y -=20;

}

player2Up = false;

} else if (player2Down == true) {

if (rect2Y >= 707.5) {

rect2Y = 707.5;

} else {

rect2Y += 20;

}

player2Down = false;

}

}

</code>


