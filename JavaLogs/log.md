<!--
### Day 0: February 30, 2016 (Example 2)
##### (delete me or comment me out)

**Today's Progress**: Fixed CSS, worked on canvas functionality for the app.

**Thoughts**: I really struggled with CSS, but, overall, I feel like I am slowly getting better at it. Canvas is still new for me, but I managed to figure out some basic functionality.

**Link(s) to work**: [Calculator App](http://www.example.com)
-->

# Java Log

### November 14, 2019

**Progress**: Initiated a terminal/cmd program that consists of a simple library/book store system. This program will keep basic book information such as, author, publisher, genre and price. No input prompts will be made, all information will be hardcoded into the program. An array will exist which contains a quantity for each book sold and will prompt a list of each book sold and the total charge for each book.

**(update)**
Publisher class has two variables, Name and State. Book class has four variables, Title, Author, Publisher (class), and Price. In addition to the standard setters and getter,  the Book class will also have a calculateCharge method that will take a integer for the quantity and will multiply with the Price variable to determine the total price. The last two classes will be Fiction class which will inherit the Book class and add one additional variable, FictionCode, and the NonFiction class which will have one additional variable as well called CategoryCode.

### December 11, 2019

**Progress**: Finished creating both Fiction and NonFiction classes. I am not 100% certain about Fiction and NonFiction inheriting Book class, but I did look up a reference book to get a quick idea of how it works. I will not be able to test both classes until I create a test class in order to call the two classes.

Started BookSystem class which will contain the main method. So far I have String array of arrays which contains each book's information. Also created a second integer array that contains the quantity amount for each book.
