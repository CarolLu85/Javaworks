Create an app that randomly picks 7 numbers from 1-5. Inform user that he/she will see the numbers for a few seconds and he/she should try to remember them. So, show the numbers to the user for a few seconds (You can find the instructions from the end of this exercise, how you can pause the app for a certain amount of time).

After the pause, clear the screen (instructions in the end of this exercise).

Then ask the user to type the numbers on by one.

In the end the app shows the right numbers and the numbers the user typed.
How You Can Pause the App
Place the following statement to the top of the code after using System;

try { // The pause will last 1 second Thread.sleep(1000); } catch(InterruptedException ex) { Thread.currentThread().interrupt(); }

Clear the screen

In Java & Eclipse there is no method for clearing the screen. Here is one solution that adds 20 line breaks and it seems a bit like the screen is cleared.

for (int i = 0; i < 20; ++i) System.out.println();