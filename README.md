# MindGame
1.	Theme: " MindGame "
2.	Summary:
2.1.	Objectives: 
The project implements an online educational game and an administrative part for its settings aimed at familiarizing with curious facts related to nature and the animal world. The goal is to acquire new knowledge in a fun and interactive way, implemented in the form of a game.
The target groups to which the project is directed include:
•	Students in primary and basic education;
•	Users wishing to combine gameplay with gaining new knowledge in a given subject area.
And the innovative educational environment implemented in the form of a game will stimulate interest in obtaining new knowledge.

2.2.	Main stages in the implementation of the project:
•	Researching the topic and consulting with subject area teachers;
•	Searching for information in textbooks and study aids;
•	Selection and editing of files and code;
•	Shaping the visual appearance of the web application;
•	Compilation of accompanying text and advertising documents;
•	Presentation to children from primary and basic school years and other interested groups.

2.3.	Level of complexity of the project: The main problems in the preparation and realization of the product occurred in:
•	Creating the necessary images and audio files and implementing them in the code;
•	Compiling JS and PHP code;
•	Integration of external libraries and APIs ( Application Programming interface )
•	Shaping the design.


2.4.	Logical and functional description of the solution:

General description
MindGame consists of three main modules – an online educational game for obtaining new facts and knowledge and an administrative module for creating and managing game data.
After starting the game, a home screen is loaded from which users can select the theme of the game .
 

Game start screen
Currently there are three modes (Animals, Rivers and Mountains), and the good organization of the code allows for easy upgrading with new themes.
The game is multilingual, and in addition to the facts, the entire interface also supports changing the language of messages. At the moment, two languages are supported (Bulgarian and English), but adding a new language is done by localizing messages in an exported text file.
After selecting a theme, the user is directed to the main game screen. Its goal is to find the positions of all pairs of identical cards in the optimal time. After each correct move, the player learns an interesting fact in the relevant subject area. Upon successful completion of the game, the best results are reported in a special column.


Functionality
•	Each time the game is started, random positions for the card pairs are generated, optionally using the internal random number generator or one provided by an external API;
•	In the lower right corner of the screen, an appropriate image points to the current topic
•	After starting the game with a funny animation, an animated helper is visualized, which communicates interesting facts with each successfully detected pair of cards;
•	In the result section, successfully completed games are counted - ended with the opening of all pairs of cards within two minutes. The remaining time is counted and visualized by the game;
•	The records section stores the five best scores achieved by the players, upon achieving one the player is required to enter their name to be reflected in the leaderboard.
 


Menu #1
The menu consists of three buttons and displays the current topic:
 

Menu #1
•	Animals - Ability to switch to an animal theme
•	Mountains - Ability to switch to a mountains theme
•	Rivers - Ability to switch to a rivers theme
Menu #2
The menu consists of five buttons:
 

Menu #2
•	Facts - When clicked, you will be redirected to the Admin Board , which allows you to view the facts, enter the admin module and test the API providing the facts.
 
Admin Board Interface

•	Stop sound - ability to start/stop background sound
•	Change language - the ability to switch the interface and in-game facts in different languages
•	Rules - a window with a brief description of the rules of the game
•	Contacts - window with developer contact information

Module for purchasing designs
The game has a shop that provides the opportunity to purchase card designs as well as change the background.
 

Administrative module
The facts that are used can be generated from different sources:
•	Embedded in the application as a text file;
•	APIs external to the system providing such services;
•	Using the administration API of the developed application, which provides facts on a random basis from those stored in the database.

For this purpose, a web interface was developed with functionality for viewing, adding and editing facts and thematic areas.
Unregistered users can only view the facts entered in the database and filter them by topic:


Registered users are divided into the following roles:
Administrator( admin)
✔	It is possible to edit the roles and rights in the administration module
✔	Has rights to perform basic CRUD operations on facts and categories
✔	Has the right to view all users, edit their roles and remove them
 
teacher _ _ 
✔	Has rights to perform basic CRUD operations on facts and categories
 
viewer _ _ 
✔	Has the right to review facts and categories


The administrative module is available on public hosting at the following URLs:
https://facts.vtbg.eu/

https://facts.vtbg.eu/admin/

2.5.	Implementation :
Used libraries and software technologies :
•	HTML
•	JavaScript
•	CSS
•	Bootstrap
•	jQuery
•	ClippyJS
•	PHP
•	Laravel

Software used :
•	Adobe Photoshop ( trial ) - to create the design of images in the application;

•	Visual Studio Code ( free ) – development environment (IDE);

•	Apache - web server for the administrative part of the application

•	 MySQL – relational database management system used in the administrative part of the application

•	Microsoft Office - to create the accompanying documentation and presentations.

2.6.	Application Description: 

The online game can be launched both locally (loading the home page index.html from the game folder) in the browser, and by loading the corresponding home URL from a web server. The game is available on public hosting 
at the following URL: https://mindgame.vtbg.eu/ 
To work with the administrative part of the application, it is necessary to install it on a working web server.
2.7.	Conclusion: 
In games, children set certain goals for themselves, strive to achieve them and experience joy from their achievements. In today's technological world, students find it difficult to stay focused on learning that is conducted using traditional educational approaches. The use of educational games contributes to increasing motivation and acquiring new knowledge.
MindGame app enables students to easily access new facts and knowledge using modern web technologies.

