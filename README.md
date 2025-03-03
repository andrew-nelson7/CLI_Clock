# What does this project do and what does it solve?

- This program is a 12 and 24 clock that runs in the console and allows for time offsets to support different timezones. This solves the issue of keeping track of multiple timezones by allowing users to custom the time offset while maintaining the basic functions of the clock.

# What was done well?

- The UI is consistent with the prompt and display 

# How can the code be improved?

- OS Specific APIs: Much of this program uses Windows specific APIs like (GetAsyncKeyState and SetConsoleCursorInfo) the program could instead use larger libraries like ncurses to perform similar actions and be cross-compatible with linux
- Lack of functions: Much of this program resides in the main block which hinders code readability, it would be a good idea to break the program into smaller blocks expressed as functions

# What was the most challenging piece of code to write

- The most challenging part of the code to write was the UI where I needed to intelligently space text and write over existing text using cursor manipulation

# What skills used in this project is particularly transferable to other projects?

- The use of real-time keyboard reading is notably transferable as many games and gui applications require user interaction from the keyboard.
- The ability to render characters in ASCII my moving the cursor is very important many console type applications. While on Windows many applications have a gui, on linux the CLI is king and being able to render text well on linux applications can be very important

# How was this project made maintainable, readable, and adaptable?

- This code makes use of popular windows libraries which allows the code to be better maintained.
- The code also features numerous comments before every major block of code to improve readability
