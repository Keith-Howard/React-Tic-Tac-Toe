# React-Tic-Tac-Toe
This is a Tic Tac Toe game, player X always goes first and you take turns clicking on squares until one of the players wins or there is a draw. The program will tell you who goes next and it will tell you which player won or if no one won.

# Installation
To run this program
Make sure you have Node.JS installed on your computer.
Download the JSX, HTML and CSS files from the repository.
In order to run this you need to have a local web server.
    How to install local web server
    In VS Code open project folder where all files have been unzipped
    In Terminal window execute npm init
    In Terminal window execute npm install -g HTTP-Server
    In Terminal window type HTTP-Server
    In Terminal window copy URL procided and paste into your browser HTTP://127.0.0.1:8000
    This will start the program on the browser

# Road Map
Some features that could be implemented are adding winning statistics, not allowing another player to click a square after it has already been click, changing how player is set (originally it is set to 0 and 1, I would change it to X and O) and highlight winning squares.

To implement the Player Statistics you will create a useState for stats and initialize it to an empty array in the board component because player and who won is already handled by the board component so they are local to the component. The stats would be displayed in a div on the board.

Another change to implement would be not allowing another player to click the same button. Currently you can click the button again and it will change the player value. This can be done in the Square component. There is a state called filled in the square component that is set to false. It is set to true when it has been click by a player. You can set a ternary condition to check for filled === true and disable the button if true.

# License Information
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
