# Tech-Journal

## Observations on learning to program

*Tuesday, September 12th*

Notes from the API workshop:

Parts of an API call

| PART             | EXAMPLE                   |   
------------------ | ------------------------- |
| base URL         | http:/api.something.com   |
| version          | /v4/                      |
| resource/endpoint| words.json                |
| method           | randomWord                |
| quiery params    | ?includePartOfSpeech=noun |
| auth             | &api_key=123key           | 


Persisted model = gets saved in the database



*Wednesday, May 3rd*

Just after it started taking me less than 20 minutes of reading about my Git Shell errors on Stack Overflow, I found that GitHub allows to drag and drop the code directly from one's computer into the master branch. Have mixed feelings...

*Tuesday, April 4th*

From **The Master Algorithm**:

“Science goes through three phases, which we can call the Brahe, Kepler, and Newton phases. 
In the Brahe phase, we gather lots of data, like Tycho Brahe patiently recording the positions of the planets night after night, year after year. In the Kepler phase, we fit empirical laws to the data, like Kepler did to the planets’ motions. In the Newton phase, we discover the deeper truths. Most science consists of Brahe- and Kepler-like work; Newton moments are rare. Today, big data does the work of billions of Brahes, and machine learning the work of millions of Keplers.”

*Monday, April 3rd*

From **The Master Algorithm**:

“The Industrial Revolution automated manual work and the Information Revolution did the same for mental work, but machine learning automates automation itself [...] If you’re a lazy and not-too-bright computer scientist, machine learning is the ideal occupation, because learning algorithms do all the work but let you take all the credit. On the other hand, learning algorithms could put us out of our jobs, which would only be poetic justice.”

“Machine learning is the scientific method on steroids. It follows the same process of generating, testing, and discarding or refining hypotheses. But while a scientist may spend his or her whole life coming up with and testing a few hundred hypotheses, a machine-learning system can do the same in a fraction of a second. Machine learning automates discovery. It’s no surprise, then, that it’s revolutionizing science as much as it’s revolutionizing business.”

*Sunday, April 2nd*

From **The Master Algorithm**:

“[A]s of today people can write many programs that computers can’t learn. But, more surprisingly, computers can learn programs that people can’t write. We know how to drive cars and decipher handwriting, but these skills are subconscious; we’re not able to explain to a computer how to do these things. If we give a learner a sufficient number of examples of each, however, it will happily gure out how to do them on its own, at which point we can turn it loose. at’s how the post office reads zip codes, and that’s why self-driving cars are on the way.”

“In farming, we plant the seeds, make sure they have enough water and nutrients, and reap the grown crops. Why can’t technology be more like this? It can, and that’s the promise of machine learning. Learning algorithms are the seeds, data is the soil, and the learned programs are the grown plants. A machine-learning expert is like a farmer, sowing the seeds, irrigating and fertilizing the soil, and keeping an eye on the health of the crop but otherwise staying out of the way.”

“The goal of AI is to teach computers to do what humans currently do better, and learning is arguably the most important of those things: without it, no computer can keep up with a human for long; with it, the rest follows.”

*Saturday, April 1st*

From **The Master Algorithm**: There are 5 main schools of thought in relation to machine learning

“Symbolists view learning as the inverse of deduction and take ideas from philosophy, psychology, and logic. Connectionists reverse engineer the brain and are inspired by neuroscience and physics. Evolutionaries simulate evolution on the computer and draw on genetics and evolutionary biology. Bayesians believe learning is a form of probabilistic inference and have their roots in statistics. Analogizers learn by extrapolating from similarity judgments and are influenced by psychology and mathematical optimization.”

“Thee symbolists’ master algorithm is inverse deduction, the connectionists’ is backpropagation, the evolutionaries’ is genetic programming, the Bayesians’ is Bayesian inference, and the analogizers’ is the support vector machine. In practice, however, each of these algorithms is good for some things but not others. What we really want is a single algorithm combining the key features of all of them: the ultimate master algorithm. ”

*Wednesday, March 28th, 2017*

Should one learn Hadoop first to be able to learn Spark?

“For developers, there is almost no overlap between the two. Hadoop is a framework in which you write MapReduce job by inheriting Java classes. Spark is a library that enables parallel computation via function calls.”
http://aptuz.com/blog/is-apache-spark-going-to-replace-hadoop/

*Tuesday, March 27th, 2017*

Should remember: 

all() means all the values iterated over are non-False;
any() means any (any number) are non-False

*Tuesday, March 21st, 2017*

Working on Superficial Robot. Keep adding weather check, color check, shape check, etc. Started doing yoga every morning - everything hurts.

*Monday, March 20th, 2017*

Downloaded half a dozen different connectors, but none of them work; most tell to download some other version of Python. 

Decided to export the database into a csv file instead and parse it. It works.

*Saturday, March 18th, 2017*

From documentation for Python-SQL connector: 

“Python scripts often build up and tear down large data structures in memory, up to the limits of available RAM. Because MySQL often deals with data sets that are many times larger than available memory, techniques that optimize storage space and disk I/O are especially important. For example, in MySQL tables, you typically use numeric IDs rather than string-based dictionary keys, so that the key values are compact and have a predictable length” (good to know)

*Monday, March 13th, 2017*

Saw %d and %s in someone’s SQL code. Thought they mean “anything ending with an “s” or ending with a “d” but it didn’t make sense in that context. Turns out, these are type specifiers; %d is used for integer values, %s - for string values. %% is used for percent values. 

*Monday, February 27th, 2017*

Re.Bayesian methods:

“[P]rior usage is a very easy way to deal with proportions data. This is an easy way to deal with things like upvote data, click-through rates, conversion rates, when making decisions regarding ad campaigns, item prioritization, or similarity metrics. The priors here help make sure that things don't get too extreme when there's too little data.”

From Quora:
https://www.quora.com/What-are-the-advantages-of-Bayesian-methods-over-frequentist-methods-in-web-data


*Monday, February 20th, 2017*

Continuing with Tableau.

*Friday, February 17th, 2017*

To connect MySQL to Tableau:

Connect -- to a server -- more servers -- MySQL 
Choose databases
Choose join type
Click orange button “sheet 1” (bottom left corner)
Note: “dimensions” and “measures”

Columns: Color family + measure values
Rows: Color + measure values

*Thursday, February 16th, 2017*

Disabled the safe mode in MySQL Workbench to mass update without using the key:

Edit - Preferences - SQL Editor - Safe update (uncheck the checkbox at the bottom)

Requires reconnecting to the server:

Query - Reconnect to Server

*Tuesday, February 14th, 2017*

To iterate in a list of lists
use a variable that is a list itself!
crime_rates = []

for row in five_elements:
    # row is a list variable, not a string.
    crime_rate = row[1]

    # crime_rate is a string, the crime rate of the city
    crime_rates.append(crime_rate)

This is fascinating, kind of!

*Monday, February 13th, 2017*

Nice quote from Quora re. Data scientists: they “serve as the ambassador between the data and the company.”

How do Data Scientists use statistics:
https://www.quora.com/How-do-data-scientists-use-statistics

Started following William Chen’s Storytelling with Statistics feed:
https://datastories.quora.com/

*Wednesday, February 8, 2017*

Steps of a data science project, from
https://www.dataquest.io/blog/data-science-portfolio-project/

Watch the scope (restrict it so that it can be accomplished in a reasonable amount of time)
Find data
Find additional data for context
Find background on data
See first 5 lines of each dataset
Add surveys (if available) to data
Look for an attribute common for all/most sets
Clean the data, get rid of irrelevant segments, condense sets if necessary
Handle missing rows, etc.
Unify the data into one dataset (pandas.concat) 
Compute correlations (corr in Pandas)
Visualize (on a map, scatterplot, etc.) 


%matplotlib inline

	full.plot.scatter(x='total_enrollment', y='sat_score')


More research to better understand the correlations
Write a story
“With data science, the story is never truly finished. By releasing analysis to others, you enable them to extend and shape your analysis in whatever direction interests them”

*Wednesday, January 25, 2017*

Reading on differences between regular (frequentist) statistics vs Bayesian. 

Bayesian includes a concept called 'influence of prior beliefs'.

Can be applied to solving multi-armed bandit problem (=the trade-off between exploration and exploitation)

Re. bandit problem, from Wikipedia:

“Originally considered by Allied scientists in World War II, it proved so intractable that, according to Peter Whittle, the problem was proposed to be dropped over Germany so that German scientists could also waste their time on it.”

*Sunday, January 15, 2017*

New idea for an Android game. The game is based heavily on dialogue and may be called Introvert vs. Small Talk. The player encounters friendly characters who talk nonstop. As long as the player stays engaged with the characters, he loses energy. 

*Monday, February 9, 2017*

Just after I learned the game loop and collision detection turned out tetris is one of the most copyrighted games in existence. 

“The first tetris game was made by a Soviet developer in 1984. He hadn’t received any royalties until he moved to the US in 1991 and opened a Tetris Company in 1996. The company “has copyrighted and trademarked every aspect of the game, such as the playfield dimensions, the shapes of the blocks, and the next piece.” 

The Tetris Foundation (the copyright owner) sends copyright infringement notices to Apple store and Google Play store forcing them to remove dozens of tetris-like games every year.

*Tuesday, December 20th, 2016*

Re. simple tetris game:

“A standard Tetris playing field has 16 rows and 10 columns. We can represent this in a multidimensional array, containing 16 sub-arrays of 10 elements.” 

Tetrominoes also can be represented by multidimensional arrays!


1
2
3
tetromino.shape = [[1,1],
                               [1,1]];
tetromino.topLeft = {row: 0, col:4};



*Thursday, December 15th, 2016*

Want to know in advance what data structures I’ll be learning soon. Reading a (relatively) brief overview of most common ones. 

Doubly linked lists: each element is wrapped in a node; each node contains references to the previous and the next element. Iterations are slower than even in arrays. Don’t understand why anyone would choose this structure then.

Binary tree: consists of nodes, each one has two children; the left child is always less than its parent, the right child is always greater. The worst case performance remains logarithmic.

log(n) has a graph where the rise of the curve decelerates as n increases:

Hash map: has a set of keys each mapping to an element. If I’m not mistaken, in Python it was called a dictionary. Performance degrades as the table fills up.

Stack: elements can be pushed (=added) to the end of it or popped (=removed), also from the end.

Queues: elements are added at the end and removed from the front. The element that spent in the queue the longest will be the first to be removed. Interesting.

*Wednesday, December 14th, 2016*

Enrolling in Algorithms & Data Structures and Android Programming for the next semester. But can’t wait the whole month and enrolled in a Princeton algorithms course on Coursera. 

Someone on Quora advises to learn data structures first, and then algorithms. They 
also say that more complex data structures are not necessarily harder to understand.

*Sunday, December 11th, 2016*

Preparing for the Java final exam. 
Selection sort: easy to write but is the least efficient; has a complexity of n2. 
Binary search. Exception handling.

*Saturday, December 10th, 2016*

Begin to understand the game loop better. It is needed to make the passage of time in the game consistent. It makes the speed of the game consistent across devices that themselves have different speed. Updates are aware of how much time the loop took. If the loop finished early, waits instead of overworking the graphics card. 

*Friday, December 9th, 2016*

A menu always overlaps the app bar rather than serving as an extension. 

Want to create an app with a really really bad design (to make it easy to grasp what bad design is and avoid it). The app should include: elaborate icons (all of different sizes), minimal padding, 15 different fonts, system bar in the middle of everything, 60 options to choose from (font size ranging from 300 dp to 2 dp), menus everywhere, and most importantly, Kafkaesque infinite loop-like navigation (inspired by AT&T and Kaiser Permanente).

*Thursday, December 8th, 2016*

The SurfaceView punches a hole in its window to allow its surface to be displayed - don’t understand why it works this way yet.

And then there’s a method
setZOrderOnTop(boolean onTop)
which controls whether the surface view's surface is placed on top of its window.

*Wednesday, December 7th, 2016*

Most games use a game loop. Should it be in the main thread or in a separate thread? 
From Stack Overflow: can use the loop in main if the game is very simple.

Although, “the reason people often recommend using a separate thread is because they don't want heavy processing to interfere with UI interactivity.” 

Now I remember having separate classes for logic and GUI in a simple rock-paper-scissors game I wrote recently.

*Monday, December 5th, 2016*

The greatest contemporary physicist according to a lay person (myself included) is Stephen Hawking because his name is the first/the only one that comes to mind. Theoretical physicists consider Edward Witten to be the best; Witten is the only physicist who received the Fields Medal. 

Before becoming a physicist Witten received a BA in history and worked as a journalist for a couple years.

People with a background in humanities pursuing computer science, he should be our role model! 

*Sunday, December 4th, 2016*

From Material Design, Typography: Dynamic type enables large type when the length of the text in a layout is unknown (wow, didn’t know that).

*Saturday, December 3rd, 2016*

Continuing w/Material Design Manual: turned out to be larger than I expected. Many of my vague intuitions are confirmed, yet many more things are unexpected and fascinating. 

Different aspects of an icon (curvature radius, extending elements) should be 2dp in size. 

Use opacity instead of grey (they didn’t say why but I guess it’s because hard coding things is a bad practice anyway).

A gradient over an image to make the text on top more readable is called a scrim.

*Thursday, December 1nd, 2016*

Reading Google material design manual. 

All materials are solid and flat (1dp) yet there is a z axis (perpendicular to the screen). 

When the button is pressed, its elevation increases (counterintuitive, is real life the opposite is happening). Elevated materials cast shadows (I believed shadows in flat design look tacky in 90% of the cases). 

Materials move along curved lines (arches) because it looks more natural to a human eye (the speed of a falling object doesn’t increase evenly either). This is great to know - would have taken me a long time to realize myself that the movement along an arch looks better.

*Wednesday, November 30th, 2016*

dp stands for density independent pixel, will occupy the same amount of space independent of screen’s resolution.

*Tuesday, November 29th, 2016*

Continuing w/Android. Started Udacity Android course. Learned views (TextView, ButtonView, ImageView), XML basic syntax. A self-closing tag is used when a class doesn’t have any child classes.

*Friday, November 25th, 2016*

A synthetic class is generated by the compiler at runtime. Wow….

Encountered NullPointerException:

Thrown when an application attempts to use null in a case where an object is required. These include:
Calling the instance method of a null object.
Accessing or modifying the field of a null object.
Taking the length of null as if it were an array.
Accessing or modifying the slots of null as if it were an array.
Throwing null as if it were a Throwable value.

*Thursday, November 24th, 2016*

Ordered enough food to continue with writing Rock, Paper, Scissors. Procrastinate by reading Introduction to Algorithms.

“Contrary to what one might expect, incorrect algorithms can sometimes be useful, if their error rate can be controlled.”

*Wednesday, November 23rd, 2016*

Afternoon: polymorphism.

Evening: Continuing with Rock, Paper, Scissors game (Java homework). Learned that Java doesn’t work directly with svg images but there are many online converters from svg to png or jpg. Converting an svg image of paper to a png file produces a suprematist work of art:


Wish I knew why this happens but there is no time.

*Tuesday, November 22nd, 2016*

From The Anatomy of Interest: Women in Undergraduate Computer Science study:

QUOTE “[M]en tend to exaggerate their achievements more than women, and (...) are more likely to attribute their successes and failures in a self-affirming way than are women (Eccles 1992; Dweck 1986; Licht and Shapiro 1982)... “with the same grades in science and other courses, women in science were less confident of their abilities and more depressed about their academic performance than men" (Strenta et al. 1994, 543).” END QUOTE

QUOTE “[O]ur research identifies a "chicken and egg" problem that affects a female student as she thinks about her interest in computer science: is difficulty with course work due to lack of experience? or is lack of experience due to lack of interest? or is lack of interest due to lack of confidence? or is lack of confidence due to lack of interest? It is hard to disentangle one influence from the other, to know how they interact. Women’s interest (or lack of interest) may not be as "intrinsic" as it feels, for interest is continuously encouraged or extinguished, and defined, by cultural norms, external factors and internal responses. Far from being a static, immutable given, a combination of gender socialization, cultural artifacts of the field (a male-dominated history, culture, educational practices, peer interactions), and individual psychology all construct and/or undermine many women students’ sense of their own "intrinsic interest." END QUOTE 

*Monday, November 21st, 2016*

Java: inheritance. Multiple inheritance is not supported in Java. I thought multiple inheritance meant classes having grandchildren, but no - it means having more than one parent which is legit in some languages but not Java.

*Sunday, November 20th, 2016*

Difference between bin and src folders:

"Src" is the folder where the project's source files are located ( .java files). 

"Bin" folder is usually where the compiled files are copied to ( .class, .jar, etc. files which are compiled).

A Jar file is an Zip archive containing one or more java class files; JAR = Java ARchive.

*Saturday, November 19th, 2016*

Set up Android Studio and LibJDX.

*Friday, November 18th, 2016*

Homework 7: making simple GUIs in Java (dialog boxes, radio buttons, text fields, countdowns).

When the user chooses item1 and item3 with 2-day shipping my mystery store reports:

“You have ordered nullnullnull and will receive it in null!” 

Fixed it eventually.

*Thursday, November 17th, 2016*

Obsidian color scheme for Eclipse:
http://eclipse-color-theme.github.io/update/
Help - Install new software - Add - Paste the link
Then:
Window - Preferences - General - Appearance - Color Scheme - Obsidian

*Wednesday, November 16th, 2016*

Re. DRM: “Ubisoft broke with the tendency to use online DRM in late 2008, with the release of Prince of Persia as an experiment to "see how truthful people really are" regarding the claim that DRM was inciting people to use illegal copies. Although Ubisoft has not commented on the results of the "experiment", Tweakguides noted that two torrents on Mininova had over 23,000 people downloading the game within 24 hours of its release.”

“Croteam, the company that released Serious Sam 3: BFE in November 2011, implemented a different form of DRM wherein, instead of displaying error messages that stop the illicit version of the game from running, it causes a special invincible foe in the game to appear and constantly attack the player until he or she is killed.”

*Tuesday, November 15th, 2016*

DRM, DMCA and EULAs.

DRM = digital rights management. A piece of code is inserted to prevent copying or limits the number of devices that can use the software.

DMCA = Digital Millennium Copyright Act.

EULA = End User Licence Agreement, between software’s author or publisher and the end user.

*Wednesday, November 9th, 2016*

James Bach on software testing:

The picture is not a system! What does the system do? You must ask!
A professional tester = a professional sceptic
Tester’s job is to gather evidence and draw inferences = detective work.
Learn everything you can about the product!
Always seek the underlying complexity behind the apparent simplicity!
Software testing is rapid learning and solving a new problem each time. 

*Tuesday, November 8th, 2016*

Yesterday something named a controller was used in the app and I didn’t quite figure what it was. 

Turns out, a controller is a part of an MVC (model-view-controller) design pattern; it accepts input and converts it to commands for the model or view. Editing a document = updates model’s state; scrolling through a document = changes view’s presentation of a model.

*Monday, November 7th, 2016*

Watching MEAN Stack tutorial while riding my excercise bike. MEAN stack consists of MongoDB, Express.js, Angular.js and Node.js. 

MongoDB = more flexible; to create a schema one can start using it first (and it gets created).

Node.js = Javascript on the server. There is only 1 thread. NPM = Node package manager, a library, has Node modules. Express.js is one of them.

Node.js - start w/name and version.

Express = a web application for Node.js (“fast, unopinionated, minimalist”). Listens and responds to http requests.

In a the shell: npm install express --save

Angular.js - allows to build more dynamic web applications. Encourages the separation of concerns the model, the viewer and the controller. Embeddable = can use as little or as much as you want.

In html code
After
<!DOCTYPE html>
add:
<html ng-app>

Anytime someone requests js, we use a helper function

Made a change on the server => need to restart it.

*Friday, November 4th, 2016*

Our professor recommends using Graphics2D instead of the older Graphics class in Java despite the newer Graphics2D having more cumbersome syntax.

*Thursday, November 3rd, 2016*

JFrame and JPanel are containers, JLabel is a component.

*Wednesday, November 2nd, 2016*

Continuing with Java GUI: understand the hierarchy, layers, purpose of JFrame, JButton, etc. but the purpose of JLabel is still vague - is it more like a pane or a text field (or area)? 

*Monday, October 31st, 2016*

Java GUI.

*Saturday, October 29th, 2016*

Alt+Shift+S makes getters and setters instead of the typing!!

*Friday, October 28th, 2016*

Coders Club. Have to figure what machine learning algorithm has ranking prediction.

*Wednesday, October 26th, 2016*

First time pair programming with someone much more experienced than I am (Craig). Worked on Xiki and it was amazing! Craig said that he threw me into the middle of things and I figured out what’s what faster than others.

The Lyft driver David graduated from Dev Bootcamp two weeks ago. Asked him how many graduates find a developer job within the first 3 months after graduation. He said: the majority. I asked about the algorithms. He said they had one class on them - then use online tutorials. 

*Tuesday, October 25th, 2016*

Turns out one can install Linux on top of Windows! It’s been available for a few months. Installed it too. 

*Monday, October 24th, 2016*

More Java homework: constructor and method overloading, enums, this keyword, etc.

*Sunday, October 23rd, 2016*

Craig Muth on Ziki: 
QUOTE “Most apps (or at least their main structures) boil down to nested lists of choices.  There should be a (or perhaps many) very simple languages for defining the main navigation of an app (the nested lists of choices).  Xiki is on the path to being such a format.  As it is, you can type a few nested menu items (with 2-space indenting) and use it on the command line, in a text editor, in a web browser, and as a service.
It's crazy that in 2014 there isn't a dead-simple language that you can type a few lines of, and then deploy a simple but usable app to desktops, the web, and phones, and other devices.  It should be easy to create the main navigation for an app (just by making a text file), and drop it into any platform.  Then for the specifics of what some of the items in your navigation do, platform specific code may of course be necessary.” END QUOTE
https://www.kickstarter.com/projects/xiki/xiki-the-command-revolution

Wrote him a message.

*Saturday, October 22nd, 2016*

Advice from Quora on what makes a good GitHub project:
Well-documented
Use libraries instead of reinventing the wheel
Well-written README
Tests!

From Reddit:
“The best projects are the ones who would sound cool to people who have never taken a CS class at all.”

*Friday, October 21st, 2016*

Was making a list of things for Lake Tahoe. Tried adding a coat but didn’t know the name of it’s color (a mix of medium brown, orange and red, but muted). Found a nice little app that gives names to the colors the user chooses on the color wheel. Mine’s either “rust” or “burnt sienna.” What a great and useful project:
http://chir.ag/projects/name-that-color/

*Wednesday, October 19th, 2016*

The notorious Student+Course+Roster Java assignment - everything almost works except for the array with Student objects inside of a Course class. 
Found so many others struggling with this on CodeRanch and Stack Overflow. 

*Sunday, October 16th, 2016*

Learned that the QWERTY keyboard was created to slow down typists so as to avoid jamming up the old mechanical typewriters!

*Wednesday, October 12th, 2016*

Java Midterm. Got 96/100

*Sunday, October 2nd, 2016

From Linux Command Line:

QUOTE “What’s the difference between BRE and ERE? It’s a matter of metacharacters. With BRE, the following metacharacters are recognized: 
^ $ . [ ] * 
All other characters are considered literals. 
With ERE, the following metacharacters (and their associated functions) are added: 
( ) { } ? + | 
However (and this is the fun part), the “(”, “)”, “{”, and “}” characters are treated as metacharacters in BRE if they are escaped with a backslash, whereas with ERE, preceding any metacharacter with a backslash causes it to be treated as a literal.” END QUOTE

How evil is that?..

*Saturday, October 1st, 2016*

Missed a meeting w/Masha’s brother who was visiting for only a few days because of trying to figure out when to use arrays vs. lists vs. collections.

Am fascinated with the concept of multidimensional arrays. Don’t know yet why use them, assume for some crazy 3D graphics. 

*Thursday, September 29th, 2016*

Regular expressions start to seem less overwhelming, wrote first simple ones (with pipes) that worked.

*Wednesday, September 28th, 2016*

Missed Java class, missed Women Who Code panel talk - fell asleep and slept from 3pm to 8pm. Saw dreams/nightmares: Java code and riding on the train where my fake leather backpack was stolen by a blonde overweight girl.  I took it back from her which made her angry.

Struggling with Java project1 - creating a bank account. The driver program half-works only if in the same file as the class, otherwise throws “cannot be resolved to a type” error. Should have put both files in the same folder? 

1.5 past the midnight deadline: the code after line 128 is still a bloody mess.

*Sunday, September 18th, 2016*

Unix/Linux permissions: chmod absolute and symbolic; hard and symbolic links. Assignment 2 due tomorrow.

*Saturday, September 17th, 2016*

Linux textbook on symlinks: created some.

*Friday, September 16th, 2016*

From Linux Exercise FileUtils3: “Filenames and directory structure are an illusion. They don't really exist. Sorry.”

*Thursday, September 15th, 2016*

Linux: grep, find, etc.
CS101: compression, Newman algorithm for compression.

*Wednesday, September 14th, 2016*

Java classes: dog class.

*Sunday, September 11th*

From Java homework-2: “leave x alone if x is 0”

*Sunday, September 4th, 2016*

Java conditionals (read the textbook, chapter 5).

*Saturday, September 3rd, 2016*

Linux: Lab1, part 1
Exercises: Paths, part 1 (going up to parent directories, then down to display or list files and directories).

Ordered the SQL textbook, started.

*Thursday, September 1st, 2016*

Linux lab 3 - find and permissions. Was slower than some but not lost at all. CS101 - little test (easy). Memory: swapping, thrashing + parity bit.

Quora: why do front-end developers seem less self-confident? Answers: because there are so many variables on the front-end, while in the back-end something either works as intended or not; because front-end developers have control of their tools, while front-end devs can’t change their users’ browser, etc. + less subjective requirements in the front-end overall

*Wednesday, August 31st, 2016*

Java - control flow, loops. Haven’t read the book on it yet but didn’t feel completely lost - the syntax is not that different (from Python) and the idea is familiar. 

*Tuesday, August 30th, 2016*

Had to miss Writing Group because of Linux Assignment 1 deadline. Haven’t practiced Linux enough, did only a part of the assignment by the deadline; shh connection to hills was slow and logging me out every few minutes. Realized Learning Linux commands is a lot like learning to play a musical instrument: easy to understand, hard to use because one needs to practice A LOT.

*Sunday, August 28th, 2016*

Doing Java homework till 3 am in the morning. Can write simple programs!

*Thursday, August 25th, 2016*

CS101 turned out to be more interesting than expected: communication between Control Unit, ALU and RAM through set and enable wires, etc.

*Wednesday, August 24th, 2016*

Went to Coders Club meeting and joined them.

*Tuesday, August 23rd, 2016*

Dev Bootcamp’s founder: the hiring manager sees your trajectory (“I didn’t know any of that 9 weeks ago, see where I can be 2 months from now with a little guidance!”).

*Weekend: August Friday 19th - Sunday 21st, 2016*

Java Software Solutions - read 120 pages out of 159. Learned a lot!

*Thursday, August 18, 2016*

Started reading Linux Command Line, installed shh and sshed to hills - CCSF’s Linux server.

*Wednesday, August 17th, 2016*

Rented Starting Out with Java: From Control Structures to Objects and Java Software Solutions from Amazon and received free 2-day shipping for half a year as a student.

*Tuesday, August 16th, 2016*

First Unix/Linux class. Learned many commands but was wondering why it is all needed. 
Turns out, everything is based on Unix/Linux (Mac OS, Android). Windows is the only other OS (Professor Boyle despises it). Programmers from Quora: backend developers should know/use Unix/Linux. It’s very effective (for what? unclear yet). It is also an integral part of the culture.

*Monday, August 15th, 2016*

First Java class. Very fast-paced. Have to read the previous semester’s book.

*Sunday, August 14th, 2016*

TutorialsPoint Java tutorial: classes, identifiers, modifiers

*Friday, August 12th, 2016*

Installed Code Pretty plugin for Google Docs.

*Thursday, August 11th, 2016*

Installed Eclipse (Mars).
JPA = Java Persistence API.

Coders at Work: “Seibel: [T]hese days you’ve got to have a little capacity for saying, “I sort of understand how this works and I’m going to let it go at that until it becomes urgent that I understand it better.” 

*Wednesday, August 10th, 2016*

Installed Java (JDK - Java Developers Kip and JRE - Java Runtime Environment) 8.
Ov helped to make a path (advice w/semicolons from the tutorial didn’t work).
Made a list of Java-A topics from the course syllabus I have to become familiar with.

*Tuesday, August 9th, 2016*

Meetup re.CCSF. Should take Java B instead of A and an Android classes (also Java). Making phone apps is easier and faster than web apps.

*Sunday, August 7th, 2016*

Registered for CCSF CS classes: Java + Unix/Linux + 2 other ones.

*Saturday, August 6th, 2016*

Choosing between Java and C++. 
Differences:
C++ was created to be a better C, Java was supposed to be a better C++
C++ is an older language, some may say outdated
It’s faster
C++ is harder to learn
C++: Google Search, MySQL, Google Chrome
Java; most Android apps, OpenOffice, financial services apps (!), e-commerce, big data, scientific applications like native language processing 
Java is similar to C++ but doesn’t have the complicated features of it (pointers, operator overloading, etc.). Java has method overloading though
Java was initially created as an interpreter
Java is compiled to bytecode which then runs inside a virtual machine named JVM, while C++ compiles into Assembly; Java pays for its platform independence with a performance penalty
Java does not provide access to low-level system primitives and resources, where C++ does
Java: “write once, run anywhere,” while C++ has libraries to make it compatible w/diff. platforms
C++ is the language whose customers are programmers, while in case of Java it’s end users and “attempts to protect the end user from the programmer”
Java forces one to write OOP code, C++ is a multiparadigm language that allows one to do anything, including “bad” OOP ones like multiple inheritance
Java has a garbage collector (=automatic memory management); C++ has manual memory management by default
Java’s standard library is more extensive than C++’s
Hadoop is Java-based framework used for big data
Clojure and Scala also run on JVM

*Wednesday, August 3rd, 2016*

Applied to City College, CS.

*Tuesday, August 2nd, 2016*

App Lab’s (coding w/blocks) tutorial (simple app): Javascript embedded in HTML (if button (button id) is checked, go to page “yes”, else …)

Can switch between “show text” (normal code) vs. “show blocks” (flow).

JavaScript On Event (HTML events: the page has finished loading, the button was clicked, etc.):

<button onclick='document.getElementById("demo").innerHTML=Date()'>The time is?</button>

(JS is in quotes)

Node.js - V8 (interpreter) for the server side (allows using JavaScript on the server side). 
Npm - packages (modules) for JS to build from.

PS. JavaScript is asynchronous (single threaded), but the request has the thread for as long as it is actively doing something = a timeshare of the single thread between all requests.
Learned more about multithreading (block, barrel, simultaneous).

*Monday, August 1st, 2016*

Found Code.org and App Lab.

Quora (question on programming languages): JavaScript will become a thing of the past because users are switching from desktop to mobile > Python/Django or Ruby/Rails.

*Sunday, July 31st, 2016*

Zawinski: “You’ve got to say in the comment something that’s not there already. What’s it for? Either a higher-level or a lower-level description, depending on what’s most important. Sometimes the most important thing is, what is this for? Why would I use it? And sometimes the most important thing is, what’s the range of inputs that this expects?”

Started L8 - Assertions and Exceptions. 

*Saturday, July 30th, 2016*

Coders at Work. Jamie Zawinski: “[P]ut a window on the screen that has some buttons on it, and then dig down and start building the stuff that those buttons do (...) I find that getting something on the screen as soon as possible really helps focus the problem for me.” 

*Friday, July 29th, 2016*

Started reading Coders at Work.

*Tuesday, July 26th, 2016*

Debugging as binary search: add a print statement in the middle of the code. If the output is not what was expected, add another one in the middle of the first half of the code, etc.

*Monday, July 11th, 2016*

Added Postman extension to Chrome (cuts down the time for testing and developing APIs).

*Sunday, July 10th, 2016*

Explained the API request to Mika.

Everyone recommends The Gang of Four book (Design Patterns: Elements of Reusable Object-Oriented Software) = recurring solutions to common problems (!!), explains how different things are built!
Clean Code book - also recommended.
The Algorithm Design Manual - intermediate level, everyone recommends.
Coursera Algorithms course - check too.

What do self-taught programmers usually lack (Quora): vocabulary (read some introduction to programming book), algorithms, design & architecture, data structures (which ones to choose), understanding of the big picture (focus on end result instead), understanding of different programming paradigms (OO, functional, reactive), and humility. 

*Wednesday, July 6th, 2016*

Continued L7 debugging. Debugging as search: narrow down the space of errors, use the print statement throughout the code.

*Tuesday, July 5th, 2016*

L7: testing and debugging. Black-box: based on specification; glass-box: based on implementation (code). Recursion (recited from Think Like A Computer Scientist, Chapter 18): on nested lists.

*Monday, July 4th, 2016*

PSET3 - Radiation problem (find the area of a curved figure). Decreasing the step didn’t make my answers more accurate for some reason. Mine still were +-5% from the correct ones.

*Sunday, July 3rd, 2016*

Turing: decision problem. On Computable Numbers, with an Application to the Entscheidungsproblem, published in 1936. If a problem can be broken down into simple problems (=algorithm), it is decidable.

*Friday, July 1st, 2016*

GitHub flow: branch, commit, pull request. Awesome Python - collection of libraries and frameworks. Faker - package generating fake data. 

*Wednesday, June 29th, 2016*

Read Tutorials Point: Classes (instance, inheritance, etc.), modules (import, from, etc.)

*Tuesday, June 28th, 2016*

Ruby/Rails vs. Javascript/Node.js -> Javascript is more likely to dominate.

*Sunday, June 26th, 2016*

Read about 12 points Joel test for programming workplaces.

*Saturday, June 25th, 2016*

L6: problems 10 and 11. Dictionaries. Map built-in function: applies a list of functions to a list of arguments. dict.keys(), dict.items(), etc.

*Saturday, June 18th, 2016*

Structure and Implementation of Computer Programs: normal-order evaluation (fully expand, then reduce) vs. applicative-order evaluation (evaluate the arguments, then apply) - re. interpreters. (Lisp?) interpreter uses applicative-order evaluation. Usually, but not always, both types produce the same results.

Python: dictionaries (remind of SQL)

*Thursday, June 16th, 2016*

Eli the Computer Guy podcast: Portfolio!

Django connects an SQL database to Python, and more!

*Wednesday, June 15th, 2016*

is  operator - checks if things are the same objects and have the same place in the memory and the same id. 
== operator compares the values of the objects.

>>> x = 'a' 
>>> x += 'bc' 
>>> y = 'abc' 
>>> x == y 
True 
>>> x is y 
False
So, why aren't they the same string? Especially given this:
>>> z = 'abc' 
>>> w = 'abc' 
>>> z is w 
True
NB! In case of assignment, both variables point to the same object, is = True

Operations with lists: append, extend, insert (index, x), remove (x), pop (return and remove), clear (= del), list.sort() vs. sorted(list), reverse, copy

*Tuesday, June 14th, 2016*

The general form of a procedure definition (in Lisp) is 
(define (<name> <formal parameters> ) <body> ) 

*Sunday, June 12th, 2016*

From Structure and Interpretation of a Computer Program:

“[A] computer language is not just a way of getting a computer to perform operations but rather that it is a novel formal medium for expressing ideas about methodology. Thus, programs must be written for people to read, and only incidentally for machines to execute.”

“[O]ur conviction that ‘‘computer science’’ is not a science and that its significance has little to do with computers. The computer revolution is a revolution in the way we think and in the way we express what we think. The essence of this change is the emergence of what might best be called procedural epistemology -- the study of the structure of knowledge from an imperative point of view, as opposed to the more declarative point of view taken by classical mathematical subjects.”

*Saturday, June 11th, 2016*

SQL - pros and cons of splitting an SQL table into multiple tables. “Overly normalized tables” = not necessarily a good thing.

*June 1st, 2016*

Lists. Range.

*Friday, May 20th, 2016*

Degree vs. bootcamps: bootcamps teach practical knowledge, and their graduates are faster at understanding a problem, writing clean code, etc. But lack in algorithms, data structures and understanding of how computers work. YC startups prefer so called “Product Programmers” to “Technical Programmers” and dislike enterprise programmers (Java, C#).

*Thursday, May 19th, 2016*

L6 - lists. Amend, traversal, nested.

*Wednesday, May 11th, 2016*

L6 - lists, tuples

*Saturday, April 23rd, 2016*

Found how to update multiple records - had to disable “safe update.” 
The amount of different combinations of 176 items divided into 6 categories is over 34 billion. Need to add constraints to reduce this amount. Read about SQL’s IF function. Hasn’t been working yet.

*Friday, April 22nd, 2016*

Mika said: make a separate table with the rules in SQL. For the front end have to use Java or Ruby or something else. Mobile apps are harder to write that web apps.

*Thursday, April 21st, 2016*

Bought a domain, 1 year hosting for Shadows in a Red Cave.

*Monday, April 18th, 2016*

Junior developers: must have a “beginner mind” (humble, looking for learning opportunities everywhere). Have to do a lot of refactoring (rewriting ugly code) and little self-contained tasks. Integrate library code into the codebase. Be excited to be part of a team and enthusiastic about technology. Fix bugs. Work on internal tools. 

*Sunday, April 15th, 2016*

Started L6 (Objects) in Python.

*Saturday, April 14th, 2016*

Forgot the password from MySQL Workbench. 

*Thursday, April 14th, 2016*

Transition to Software Engineering meetup. 

HackBright Academy = like a convent school, girls only. Easy interview process, less tech, “just explain them why you like programming.” The challenge can be done in any language. People work on their personal projects for the last half of the term. Each student is assigned a mentor.

Dev Bootcamp. The oldest. Easier to enroll.

App Academy (Sophy). Pay later. Very tech interview. Ruby. Challenges are googlable.

Hack Reactor. JavaScript. Harder to enroll. Teach some CS fundamentals.

Makers Square is affiliated w/Hack Reactor but has simpler facilities, is cheaper.

Resume: highlight projects, not the bootcamp. Employers don’t care about the bootcamp. Don’t talk about it at the interview. All bootcamps prepare for job interviews.

Looking for a job. Apply for positions with experience “2 years and under.” Some people even got senior positions after the bootcamp. Cold applications: 5 a day is OK. If applied to more than 10 and no response = something’s wrong with the resume. The girl from Dev Bootcamp found a job at Adobe through networking. Bought a paid LinkedIn account, asked people to have coffee with her and “what it is like to work at this place?” Said: “They won’t remember anything I said, the point is to make them like me and remember me.”

Mentors. Sophy used a mentor to teach her how to transition from being an engineer to VP.

*Saturday, April 9th, 2016*

Rows: 157.
Can make simple queries (like, %, etc.). AND NOT works!

*Monday, April 4th, 2016*

Added 2 new columns to article_category. Renamed Category_ID and Category_Name to SubCategory_ID and SubCategory_Name. Have 21 subcategories and 6 categories.

Refreshed queries: order by, limit

*Saturday, April 2nd, 2016*

Row 42 in articles_list is considered a duplicate. Had to delete. Now have row 41 and 43.
Total number of rows today: 57.

*Friday, April 1st, 2016*

Made more tables (Article_Category). Added foreign keys. CASCADE means delete values in the parent table. There is also SET NULL value. Chose CASCADE for now. 

Replaced TINYINT in Pattern with VARCHAR.

*Thursday, March 31st, 2016*

Created first rows of outfit_robot. Edited column names. Found that boolean type in MySQL is TYNYINT(1) - 0 for False, 1 for True.

*Wednesday, March 30th, 2016*

Installed MySQL Workbench (editor). Started making the first database!!
The recommended maximum amount of foreign keys is 253.

*Tuesday, March 29th, 2016*

Data Engineering and Hiring meetup.

Apache Spark is a very hot thing now - “who could have known half a year ago?” Similar to Hadoop. Both are big data frameworks. Hadoop does distributed storage and indexing of data; Spark does data processing. Spark was designed for Hadoop and is faster than MapReduce (Hadoop’s data processing tool). Essential for processing of streaming data.

RE. interviews. Valuable: passion for the industry and passion for learning. Many people are hired for their potential rather than experience. While solving a problem, communicate!

Important: asking questions during the interview. 
Good questions: 
How do you evaluate people?
What are the rituals in the team?
What kind of person is a successful member of the team?
What is the next step the company is considering?
Best:
Suggestions for the app, improvements, etc.

From Upwork. Python = $55/h, Scala+Spark = $95/h

Installed mySQL. 

*Thursday, March 24th, 2016*

Problem 8: find if a character is in a string using recursion and bisection search. Very hard. Spent more than 2 hours before looking for an answer.
Stack Overflow: found how to sort a string in alphabetical order. Found it wasn’t required in the assignment.

Found an easier course called The Hard Way to Learn Python. Decided to take it when tired, and the MIT one when have high energy.

Ov persuaded to enroll in HTML & CSS & JavaScript course.

*Wednesday, March 23rd, 2016*

Rehearsed the SQL workshop.
L5 problem 6 and 7: iterative and recursive function to determine the length of a string, as if the built in one didn’t exist.

*Tuesday, March 22nd, 2016*

Intro to JavaScript meetup at Galvanize. JavaScript also has functions and many more similarities to Python. People with no programming background were lost. Realized it was a great idea to take a course on introduction to programming, rather than just learn a language.

Made mistakes: one was because i misspelled “length,” another one - missed a < in “script.

*Sunday, March 20th, 2016*

Intro to SQL workshop. Learned how to query databases, didn’t learn how to create new ones.
Operators: select (columns), from (table_name), where (condition), group by (column), having (condition), order by (column), limit (number).

Operators: =, !=, % (like), ilike (case insensitive), ~ (matches regular expressions), in (included in a list).

Join.

Monday, March 14th, 2016

Quora: a senior programmer can work with an ill formed task.
L5: Fibonacci numbers - code (and his rabbit breeding background); palindrome. Both are solved recursively.

*Thursday, March 10th, 2016*

Talked with Tigran. Asked why there were so few junior developer jobs. He said the listings that are “not senior” and don’t ask for many years of experience could be junior roles. Junior developers are not expected to have experience - only education (and maybe internships).Said his company once had a problem having too many inexperienced junior developers at once; they wrote poor code. His lead developer spends hours with junior devs discussing different ways to solve a problem, etc.

*Tuesday, March 8th, 2016*

L5, Problem 5 - recursive function to find the greatest common divisor using Euclid’s formula. 
The Towers of Hanoi recursive algorithm. So beautiful - made me cry.

*Monday, March 7th, 2016*

Enrolled in SQL workshop on March 20th.

*Sunday, March 6th, 2016*

From Quora: Programmers don’t write code for 8 hours a day, but rather 1-3 hours. The rest of the time is spent thinking, meeting, designing, solving, debugging. 

Another advice from Quora (how do self-taught programmers actually get jobs?): find a mentor. Highly focused (= immersive) education is effective. Other options: start with freelancing (charge the same as the lowest bidders; then $30/h, then there will be a long-term client). Apprenticeships. Find a technical recruiter. Find a small company to start with to get more personal interviews (startup meetups). Portfolio. An open source project (may start by writing documentation, then bug hunting/fixing, then maintaining). A long term personal project. A website or API with custom coding (accessing a remote API - this API could be github, flickr, Facebook, etc.-  or using custom database queries; it has to look good). For mid-level: at least 6 months of commercial experience + unit testing (RSpec for Ruby) + UI testing (Selenium) + Agile + code design + concurrency.

“Not having a CS degree is only a problem in the first few years of career.”

Small personal website: what you have learned so far, links to projects, what problems were encountered and how you solved them. 

Readable code! Clarity of structure and naming!

Make it a habit to go on GitHub and explore projects every day!

*Thursday, March 3rd, 2016*

The weird function works because of mathematical induction.
Difference between iteration and recursion.
Solved Problem 2, 3. Was solving # 4 for over an hour, but forgot about the min function. Went to see the solution in comments.

*Monday, February 29th, 2016*

L5. Solved problem 1. Recursion step and base case. Weird function referencing itself that works for some reason.

*Sunday, February 28th, 2016*

Cyclomatic complexity and control flow graph.
Pset 1, problem 1: counting vowels in a user generated string - solved. 

Was surprised how many ways to solve a problem that are not working I already know!

*Thursday, February 25th, 2016*

Quora: experienced programmers use less “if” statements.
Cargo cult programming - when inexperienced programmers use things they do not completely understand.

*Tuesday, February 23rd, 2016*

Solved L4 problems 8-11. 
Was looking for an in operator in documentation. Encountered a piece of code for creating Fibonacci numbers. Couldn’t understand why it does what it does for 40 minutes. Finally got it.

Problem L12 - string methods: index, find, capitalize, lower, islower, etc. The difference between index and find methods. 

*Saturday, February 20th, 2016*

Functions within functions: order of execution, stack frames. Understood but when they kept over-explaining, un-understood. 

Watched Recitation # 2 - covered for loop, while loop, range, tuples (were not covered in lectures).

*Friday, February 19th, 2016*

Stack Exchange has a sub-site for code review. 

Advice for a programming blog from somewhere: list 1 thing you learned a day.

Did exercises for L4 (functions). Got confused with times when values from global environments are used vs. local environment (both can happen at once in an irrational manner). Went to YouTube to watch the same lecture done by the old professor. His presentation was better. 

*Thursday, February 18th, 2016*

Met with Jury and went to a VR event at Google. Jury said it is best to learn from more experienced programmers (rather than courses, etc.). Asked him why they might be interested to work with me/teach me. He said 1. because you will do simpler, repetitive boring things for them 2. older programmers have parental instinct and like to pass on their knowledge.

*Wednesday, February 17th, 2016*

Continued L4 about functions - environment, etc.
Watched a tech interview with a problem of airplanes’ queue (was solved in Python).

*Tuesday, February 16th, 2016*

Realized I didn’t know the English names of many most basic math things (knew them only in Russian), like polynomials. While reading learned about imaginary numbers (i).
 i2 = −1
Other types of numbers: real numbers, natural (prime and composite) numbers, irrational numbers (# 2,), etc.
Refreshed denominators and differentiation. If for x2 f’(x) = 2x; for a constant f’(x) = 0 (a number; the function on the graph is parallel to y axis, so it makes sense).
At the end of L3 there was a Newton-Raphson algorithm for finding better guesses for square roots.
L4 - functions.
def name (property1, property 2, etc.): 
‘’’
comment
‘’’
code
---
(to recall) 
variable = name (x, y, z, etc.)
recall

If there is no recall, it will run through all the expressions.

*Friday, February 12th, 2016*

“Secret number” excercise (MIT, edX, Python). Couldn’t make it work - the program was supposed to ask each question once, but mine was asking the same question numerous times. After 2-3 hours looked at the solution. It was similar to mine, but had a few lines I didn’t understand. 

guessed = False

while not guessed:
…
 if user_ans == 'c':
guessed = True

Replaced “while not guessed” with “while guessed = True” - didn’t work. 

*Thursday, February 11th, 2016*

Went to JVS’ Starting a Career in Tech lecture/workshop. Sameer from Digital Strategies was presenting. 

Sameer: everything that uses technology is considered to be “tech industry,” like content management, etc. Problem solving mindset is needed. Being able to solve a problem is more important (and desirable) than knowing a particular technologie/tool, etc. Important to have at least a basic understanding of “Turtles All the Way Down”/”Coasting.”

Sameer: In smaller companies tech roles are defined based on systems the company has. The bigger the company, the more specific they get in their job roles/descriptions. Big companies have “glass ceiling”: the management decides certain employees are good in their roles and don’t want them to ever move up. Not the case with smaller companies that never have enough people. Must understand the business, how different departments interact and how you can bring value.

Tools change fast because consumer expectations change.

80% of the things you will learn from your peers (people who are there learning the same thing). There are meetups for every thing imaginable. Subreddits.

Important for interviews. 
Career narrative. “Every time I had to prove that my previous job doesn’t disqualify me from this one.”
Communication skills. Being able to explain things, explain your role in the company, challenges you faced. Community service = good.
Approach to Learning. Good: iterative approach, willingness to hustle, to persevere, willingness to collaborate.
Resume + Online Presence. Use keywords from the job description. If it is your dream job, say so in the cover letter! Resume is only useful in passing the keyword filter. Upload it to Dice, CareerBuilder, Stack Overflow Careers, etc. LinkedIn is a must. LinkedIn recommendations. Developers should also have Github and a website. Website shows you are current and has needed keywords (just like the resume).
Tools, Processes. Kiss Metrics and Tableau are replacing SQL. 
Educational Background. Huge number of programmers are self-taught. Familiarity with the business is more important than knowing particular tools. HTML & CSS, SQL, API, Unix, security - must know for almost everyone. Bootcamps are expensive, they will find you a job, but you must know first that this industry is what you want.

*Sunday, February 7th, 2016*

Girl Develop It 2-day HTML & CSS workshop. 

Day 1. 

HTML provides structure and semantics.
Works regardless of indentation! 2 spaces is a good practice.
<!DOCTYPE html> must be on top of every page.
The head contains metadata about the page, the body - actual content.
HTML validator, HTML Formatter (indents nicely) and W3Schools (has a validator and lots of info)are good tools.
Lists, formatted text (em, strong), images, links, embedding (iframe), tables, debugging, HTTP request, buttons, labels, checkboxes, radio buttons, exercises. 7h.
Sublime Editor looks pretty.
Not having a 5-minute break for hours is murder.

*Saturday, February 6th, 2016*

Workshop, day 2.

CSS - Cascading Style Sheets.

Consist of style rules. Rules consist of “selectors” and “declarations.”
Goes into head. <style> bla bla </style>
Types of selectors: 1. element 2. ID 3. class 4. position in document
Color systems: HEX, RGB
p { .. } element, finds all p elements
#ID 
.class
_ (space) position in document (example ul em { ….} finds a em descendant of ul)
a: active { .. } Pseudo class selectors style elements depending on their state (example: pressed link changes its color, etc.)
/* …*/ comments
color (font color), background-color, font-family, font-size (em, %, px, xx-small, smaller, etc.), font-weight.
Elements, types: inline and block.
<div> creates a block element
The Box Model (all elements are treated as boxes by the browser): margin, border, padding, z-index
Page layouts - use FluxBox and/or Bootstrap.

*Friday, February 5th, 2016*

Read an article saying there are people that cannot be taught how to program, no matter the approach. The concepts that are the most hard to grasp are:
assignment and sequence
recursion / iteration
concurrency

Cache, URL, RESTful applications - scratched the surface.

*Wednesday, February 3rd, 2016*

Apple - $460,772 in profits per employee
21st Century Fox - $277,344
Google - $270,123
Facebook at $236,705
Facebook has about 8,500 developers

*Tuesday, February 2nd, 2016*

Went to whiteboard interview practice meetup at Chartboost. Talked with Ryan, head of talent. He said:

"Networking is very important; those who have connections in the company will be considered first.
For changing careers from screenwriting / copywriting to programming it makes sense to apply to media / film / etc. companies.
Re.resume. Don’t have to remove all non-related experience completely. May let it occupy bottom 25-30% of the resume
They hired 3 people out of bootcamps in the last few years
consider internships; they are not only for students and are well-paid. Each such position had 300 people applying over the course of 2 months.
Should have a portfolio: open source projects, etc.
The first programming job will be the most hard, then things will get much easier."

Another guy, Prawaal, said:
"If you already have a BA or MA, then a bootcamp or a QA position may be a good start
Big companies (he worked for Oracle and Symantec) don’t hire from bootcamps but rather from colleges, esp. in Southern CA
Question often asked at QA interviews: how would you test this (most common - a vending machine)?
Even a senior engineer starts providing value only after about 3 months on the job."

2 eggs, 100 floors. Suggested going at a certain step, like 3 or 4. Prawaal said bisection search only. But his version will take more steps!

Veronica: was teaching herself Java for almost a year but is not familiar with neither pseudo code nor decision trees.

*Monday, February 1st, 2016*

Stack, linked list, skip list.

*Sunday, January 31st, 2016*

More exercises - while True creating an infinite loop, for loop inside of the while loop, etc. Got most of them wrong.
Zipfian Academy teaches data science (12 week course), but previous knowledge of mathematics/statistics is needed. Apprentice program for intermediate developers at thoughtbot.

*Saturday, January 30th, 2016*

Karrigell - Python web framework. Another way is to insert Python code into HTML using <% %>
Enrolled in Saturday/Sunday HTML/CSS workshop.

*Friday, January 29th, 2016*

Watched a TED on data visualization (context is important, # US military budget: absolute values vs. soldiers per capita or spending compared to GDP, etc.). Python’s keywords and built-in functions. Continued lecture 3’s homework: for loops, ranges, check and guess algorithm.

*Thursday, January 28th, 2016*

Heard of trading algorithms for the first time (Stealth analogy). Heap sort algorithm.

*Monday, January 25th, 2016*

Found Python syntax cheat sheets and Big O cheat sheets.
Finished lecture 2 + homework. Wrote many simple branching programs + FizzBuzz.

*Sunday, January 24th, 2016*

6.00.1x course: half lecture 2 + homework, functions (half lect.4) + homework. Started with lecture 4 because of the assignment deadline (watched lect 1-3 in the past). Couldn’t do the assignment, went back to the previous lectures. Homework for lecture 2 was easy.

*Saturday, January 23rd, 2016*

Bus (in comp. architecture). Transatlantic cable. Parser.
String operations in Python.
Watched (pausing to think/Google) lecture 1 of MIT-edX 6.00.1x course.

*Thursday, January 21st, 2016*

Grant advised to create simple programs (the one that backs up all the files once a week, for instance). Said he creates a calculator and/or a spirograph in any new language he learns. Google and search for a solution till one is found.

*Wednesday, January 20th, 2016*

Canopy’s documentation, used for the first time.
Data validation - finally understood what it means.

Read about developer job experiences on Quora. Small companies (stress, speed, more demands, more learning) vs. big companies (can afford code reviews, organized databases, testing infrastructure, etc.); companies that have clients (stress, diversity of products) vs. build their own product. At a job interview ask many questions about their practices (how do you use source control, what are your coding standards, how are the deadlines managed).

Another advice: keeping work journal. Will better understand how long things take.
code reviews Do save time in the end but they are upfront costs.

Comments to code should address the “why” (it is necessary, this approach is taken, etc.) rather than “what” (it is doing) + provide assumptions + a business context + comment the unexpected + workarounds for bugs.

*Monday, January 18th, 2016*

Started MIT 6.01 course via edX. Installed Canopy (Python 2.7, editor, libraries).

If an infinite loop occurres, press Ctrl + or restart the Kernel or restart Canopy.

*Saturday, January 16th, 2016*

Asked Dima about the amount of skills that’s good enough to apply for a job. He said understanding of data modeling was very important + to google interview questions for a particular language.

Data modeling: conceptual, logical, physical.
4 data modeling types (Barker is the most popular).
Data mod. steps (entities, relationships, attributes, normalize, denormalize, etc.)

*Friday, January 15th, 2016*

Joined more programming meetups. 
RSVP'd for data science on Jan 29 and mock whiteboard interviews on Feb 2nd. 

*Thursday, January 14th, 2016*

Learned that internships are usually for college students.
Indeed job postings: Python = big data + SQL/Cassandra/MongoDB
SQL vs noSQL: differences. 
SQL: blobs.
Read about lambda function and how multiple languages coexist in one program.
Created an Outfit App zdoc with a few excerpts of what is needed.

*Wednesday, January 13th, 2016*

Different approaches to teaching/learning programming. 
An article about confidence vs. competence. Intro courses help students build simple apps, students get excited. But can’t build their own apps; debug but don’t understand what is happening.

From http://doubletheprogrammers.tumblr.com/
Instead of teaching syntax and building a predetermined app, start with a real problem, introduce concepts as needed.

Advice: focus on learning each thing “just enough” to achieve your goals.

*Tuesday, January 12th, 2016*

Translators (compilers, decompilers, assemblers, etc.)
Source code, bytecode, virtual machine (i.e. interpreter?)
Charles Babbage, Ada Lovelace, Analytical Engine (Babbage created, Ada wrote the first algorithm).

*Monday, January 11th, 2016*

Gained superficial understanding of UNIX vs. Linux vs. POSIX vs. BSD 
Updated the Table of Skills.
Made a profile on Git (BreadCircuses).
Updated the list of questions to ask programmers next time I meet some of them (hash, hardware, assignment statement, operating system, portfolio questions).
Started reading about Rails and why it is used.

*Sunday, January 10th, 2016*

Functional programming article (main difference - there is no assignment)
Mutable objects, kernel, destructive assignment, copying, etc.

*Friday, January 8th, 2016*

RubyMonk: Arrays (delete, iterate, etc.) + documentation.

*Tuesday, December 29, 2015*

First steps in learning to program: consuming Wikipedia articles on different languages, paradigms, farameworks, etc., like a vacuum cleaner. Start understanding more than 3% of what they talk about.

*1991-1995*

The Soviet Union collapses. 

Kate’s main problem: wants to play chess better than Dad.

*1987-1990*

Dad is writing a PhD. 

Kate dismembers dolls and plays with used punch cards trying to find patterns in missing numbers. Created a theory: numbers “2” and “3” have irreconcilable differences and are at war with one another, but their power is almost equal and neither can win. When numbers like “23,323” and “32,223” fight, things get even more complicated. Broke more dolls.

*1983*

Mom and Dad write algorithms to predict the trajectories of flying objects in space. They are assigned programmers who write actual code for them in Fortran. Dad learns Fortran too so he can better understand what is happening. Mom doesn’t like her job because it is  too theoretical - “you never see the actual fruits of your labor.”

A daughter is born. Mom could not decide on a name for a month but then went with Katia (Kate), a popular Russian name at the time.






