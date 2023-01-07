# Video Poker Calculator
It is an offline, command-line video poker hand calculator and trainer program. Please keep in mind this is a hobby project. I have no plans for a GUI application and little free time for constant maintenance. If you want a GUI, consider forking it and writing one.

## Warnings
This program contains elements of gambling, but everything is virtual. You may only use it if you are of the legal age, and your jurisdiction permits them. 

## What is Video Poker?
Video poker is a digitalized five-card draw poker game. Gameplay initiates after placing a bet and pressing the deal button. The machine then displays five cards to the player, who may hold or discard up to every card as desired. They can press the draw button to finalize their hand, and the machine reveals the remaining cards not thrown away. If that hand is a paying hand, it will pay the player of that quantity on the pay table, in which the game concludes. Many variations of video poker exist, with the most common being multi-hand.

There is a site called VideoPoker.com, which enables users to play and practice video poker that is faithful to the ones encountered in casinos. Those wanting to attempt can create an account on this site for free. The only thing they will spend on is a member's subscription. Moreover, numerous member benefits deliver a healthy experience for all users alike. It includes training to become a perfect player to minimize the house edge!

## About This Program
It simulates a typical single-hand video poker machine in the comfort of your place of residence. Its current features include:

* Many popular games are supported, including Jacks or Better, Bonus Poker, Double Double Bonus, and wild card games such as Joker Poker and Deuces Wild.
* Training mode. It provides feedback for any incorrectly played hands according to perfect play. No feedback for best play otherwise.
* The analysis of any hand is available as long it is not in training mode. It will reveal relevant information about what to hold and enter, the expected return, the win percentage, and possible hand combinations on the redraw.
* Modify the bet and the game's pay table on the fly. By default, it uses the highest-paying one. You can also save that pay table to a file for later use instead of having to do it every time.
* Have itself play hands automatically. Hit Control-C to return to manual play.
* Real machines auto holds dealt royal flushes whenever it pops up. However, the program does not do so for the analysis.

**NOTE**: There is no point in supporting multi-hand, as the strategy does not change from single-hand apart from volatility.

## Building Instructions
It is not difficult to build. The tools required for building are just any C++ compiler. To compile this program, open a terminal window of your choice and copy-paste the command below.
```
g++ -Ofast -s -march=native main.cpp -o VPCalculator
```
In addition, I created a makefile to automate the building process for you. If your system has GNU Make, simply type ```make```, and you are good to go!

## How To Use
The program immediately starts a game of Jacks or Better without any arguments.
