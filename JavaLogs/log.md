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

### December 14, 2019

#### Book Review

**Progress**: I am using the **Java How To Program Early Object 10e** book to learn/review numerous topics. Today, I went through chapter 4 which covered control statements. The first control statement it covered was the **if** statement. After that, it added the **if...else** statement. With this statement, it covered how to created nested if...else statements and it also gave pointers on common mistakes I should look out for. One thing I did learn that I had not done so previously was the **Conditional Operator (?:)** for the if statement. I am not entirely sure how to use this method but it will definitely be something I look into a bit further and see which way I can incorporate it into my programming.

Then I reviewed the **while** statement along with a **sentinel-controlled while loop**. The difference between a non-sentinel while loop is that we previously know how many times the while loop will have to complete. But with the sentinel-controlled loop, we are not sure when the loop will have to terminate.

### December 15, 2019

#### Video Course

**Progress**: Started a video course that will go over JSP (JavaServer Pages), Servlets, and JDBC topics. So far, I have covered the JSP fundamentals which included **Expressions**, **Scriptlets**, and **Declarations**. These files are used in **.jsp** files with HTML markup is used to build webpages with Java code used throughout the page. Expressions are defined by **<%= some Java expression %>**. These are used to call a small/simple Java function. Scriptlets are defined by **<% some Java code: 1 to many lines %>**. These can be used when more than one line of Java code needs to be used in order to call a function or several items need to be completed. And lastly, Declarations are defined as **<%! variable or method declaration %>**. Declarations are used to declare methods in the .jsp file. The method can then be called from anywhere in the same .jsp file.

It is recommended to keep Scriptlets and Declarations to a minimum in the .jsp file. For this reason, it is recommended to create a separate Java Class which will have house all the heavy lifting Java code. the .jsp file can then call this Java Class with a simple Expression. This should help make the .jsp file easily maintainable.

The course then went into reading user input from a form that was used in an HTML file. Several types of inputs were reviewed such as Drop-Down Lists, Radio Buttons, and Checkboxes. After the user inputs the information, the data that confirmed and displayed using a .jsp file using Expressions and Scriptlets. These methods were simple and straightforward but will require several practice problems to ensure that I am able to fully comprehend the topic.

### December 16, 2019

#### Video Course

**Progress**: Today, I went back and reviewed the JSP Fundamentals previously covered. One of the items that I had previously not understood was the **session** object. I only remembered seeing it used in my code, but I did no understand exactly what session meant. After going back and reviewing this again, I now understand that the JSP built-in object **session** is a unique session for each individual user of a web app and several items can be stored to that session that can not be accessed by any other user.

### December 29, 2019

#### Video Course

**Progress**: Reviewed State Management with JSPs which included more information on the **session** object. After reviewing this, I covered the new subject of **Cookie**'s. I created a simple webpage that asked the user to make a selection and the webpage was then updated to reflect the choice the user made.

I also looked into the difference between ArrayList<> and List<>. During one of the examples I was doing for a JSP, they created a **List<String> items = new ArrayList<String>()**, so I questioned why was the item not created as a List<String> as well.

### December 30, 2019

#### Video Course

**Progress**: Covered the subject about **JSP Standard Tag Library (JSTL)**. I only partially covered the Core tags such as **<c:forEach>**, **<c:if>**, and the **<c:choose>** tag that is paired with the **<c:when>** tag and the **<c:otherwise>**; the choose tag works exactly like a switch statement. I practiced these tags by building a table dynamically.

### January 1, 2020

#### Video Course

**Progress**: I went over Function tags which included **length**, **toUpperCase**, **statsWith**, **split**, and the **join** functions.I did find the Java documentation which provided a bigger list of Core and Function tags. Then I covered the section about **Internationalization** and how it is used in to provide multiple languages for websites.

### January 2, 2020

#### Video Course

**Progress**: I covered **Servlet** fundamentals and compared the differences between Servlets and JSPs. I covered how to read data from forms, how to create a webpage dynamically, and the difference between **GET** and **POST**.

### January 4, 2020

#### Video Course

**Progress**: Covered how to integrate both Servlets and JSPs together and briefly looked into the **MVC (Design-View-Controler) Design Pattern**. Created a simple application that had a Student (first name, last name, and email), a StudentDataUtil class which created instances of Students, and a Servlet which handled the browser request/response. The Servlet first calls a method in StudentDataUtil which creates several instances of Student. The instances are saved in a List, and the list is then set as an attribute of the request object. Then, still in the Servlet,  we create a dispatcher with the **RequestDispatcher** class, which will call the page (or JSP) where the data will be sent. Then finally, you **forward** the request and the response with the dispatcher. After this, the JSP then loads, which will build a table with the data from each Student instance that was created. This created a table dynamically which contained a First Name, Last Name, and Email.

I then looked into MySQL server database and reviewed some of the documentation for installation. I spent between 1-2 hours installing and setting up my environment. I successfully used JDBC to connect to MySQL from my application.

### January 7, 2020

#### Video Course

**Progress**: Started a new web application project that consisted of a simple student database. The first class is the **Student** class which will have an id, first name, last name, and email address. After this, I created a **StudentDbUtil** class which will do all all of the heavy lifting behind the screen. In this class, there is a DataSource for a connection pool, and there also is a **Connection**, **Statement**, and **Result** objects so handle my sql processes. Once this utility class initiates, it sends a query to the MySQL database and returns all of the students currently available. Finally, it closes all connections from the DB and returns the connection to the connection pool.

Then **StudentControllerServlet** is the next class in this application. This class initially calls the **StudentDbUtil** class so that it can make make the connection and return the data from the the database. This servlet also provides the JDBC information (DataSource) needed in order to connect to the DB. The util class then processes the **doGet** method by calling a **listStudents** method and passing the **request** and **response**. The listStudents method then creates a list of Student objects from the data that was returned by the StudentDbUtil class. In this same method, we set the attribute as part of the the request object so that we can later use this information in our JSP. And finally, the same listStudents method then dispatches the request to the appropriate JSP, **list-students.jsp** and forwards both the **request** and **response** objects.

Finally, the **list-students.jsp** will then call the **.getAttribute** method from the request object in order to obtain the list of students. Since this method only returns a list of objects, we downcast it to **(List<Students>)** so that we can save the data to a List object. And from this point, we then put together our HTML so that we can display all the information is a table in three differenct columns, **First Name**, **Last Name**, and **Email**.

### January 9, 2020

#### Video Course

I went back and removed all of the scriplet code I used in the JSP file, and substituted it with JSTL instead. This required that I install the JSTL jar files in my project, and then replace the scriplet code with the appropriate JSTL tag.

After adding the JSTL tags, i then created a **web.xml** file that would direct the the user to a welcome file while using my development URL. This will help with keeping a URL more presentable in the long run. I also learned you can use this xml file to direct the user to other index files in different formats.

### January 10, 2020

### Video Course 
