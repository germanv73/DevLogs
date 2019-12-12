<!--
### Day 0: February 30, 2016 (Example 2)
##### (delete me or comment me out)

**Today's Progress**: Fixed CSS, worked on canvas functionality for the app.

**Thoughts**: I really struggled with CSS, but, overall, I feel like I am slowly getting better at it. Canvas is still new for me, but I managed to figure out some basic functionality.

**Link(s) to work**: [Calculator App](http://www.example.com)
-->

# Java Log

### November 14, 2019

#### Project BookSystem

**Progress**: Initiated a terminal/cmd program that consists of a simple library/book store system. This program will keep basic book information such as, author, publisher, genre and price. No input prompts will be made, all information will be hardcoded into the program. An array will exist which contains a quantity for each book sold and will prompt a list of each book sold and the total charge for each book.

**(update)**
Publisher class has two variables, Name and State. Book class has four variables, Title, Author, Publisher (class), and Price. In addition to the standard setters and getter,  the Book class will also have a calculateCharge method that will take a integer for the quantity and will multiply with the Price variable to determine the total price. The last two classes will be Fiction class which will inherit the Book class and add one additional variable, FictionCode, and the NonFiction class which will have one additional variable as well called CategoryCode.

### December 11, 2019

#### Project BookSystem

**Progress**: Finished creating both Fiction and NonFiction classes. I am not 100% certain about Fiction and NonFiction inheriting Book class, but I did look up a reference book to get a quick idea of how it works. I will not be able to test both classes until I create a test class in order to call the two classes.

Started BookSystem class which will contain the main method. So far I have String array of arrays which contains each book's information. Also created a second integer array that contains the quantity amount for each book.

### December 12, 2019

#### Project BookSystem

**Progress**: Today I worked on the book system application. In the BookSystem class, I created another array, bookArray, which will hold all the Book objects for each book created in the process. The next step would be walking through dataArray (array of arrays) and determine if a Fiction Book or NonFiction Book will need to be created.

...

I used an if statement with a String.equals() method in order to determine if dataArray[x][0] is equal to Fiction. If it does not equal Fiction, it will go through an else statement. Next, I will need to figure out how to create a Fiction/NonFiction object inside both if/else statements so that they can be stored in the bookArray.

...

The first thing I had to figure out was how to place an instance in the bookArray. I already knew that dataArray had 8 total books, so when I initiated bookArray, I made it the same length as dataArray. This also told me that as I started to walk through the dataArray, I would be able to use the counter and assign it to bookArray. So in other words, the first counter (book1) in dataArray would be created in the first index of bookArray.

Now that I had figure out how to place the new Book information in its array, I had to figure out how to create a new Fiction/NonFiction book. This was actually pretty easy, just use the counter to determine which book you were currently on in dataArray. Then, use the index of that counter array to determine the parameters that would need to be passed to the Fiction/NonFiction constructor. This is where I became a bit confused when it came to passing the Publisher reference to the Non/Fiction constructor. The quick solution I came up with was the create a separate instance of a Publisher class, and pass that reference to the Non/Fiction constructor. This did work, but I am currently unsure if there is another way around this or if it is the only way to do this process. I'll look further into this at a later date.

...

The last thing I did in BookSystem was I used the quantities found in quantityArray and called the calculateCharge method in Book class to find the total charge for each book * quantity. I printed the book Title and the total for that book in terminal and I also combined this into a String message in order to print it out in a dialog box.

And on this that note, this program is complete.
