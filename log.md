# 100 Days Of Code - Log

My format for the challenge is committing at least 15 minutes for 100 days to working through Knothecode.io. 100 days will be out on January 9th - or on February 18th if I count the weekends.


### Day 32: November 2, 2019
 
**Today's Progress**: 

KTC: PHP String Building and Processing Basics: Replacing Substrings;

Docx: -

**Thoughts:** 


**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-string-building-processing-basics/episode-8)



### Day 31: November 1, 2019
 
**Today's Progress**: 

KTC: PHP String Building and Processing Basics: Has Substring;

Docx: -

Read about Nginx and Apache for work, read about SEO and 301 redirects. My local setup is running on Nginx, so I've decided to make a list of the redirects I will need and add them all when I'm back on Apache.

**Thoughts:** 
Got stuck for a hwile because of a coincidence in line numbers and me being not attentive enough. I thought the problem was in the code I was adding on line 24, and it turned out it was in the comments.php file on line 24. No idea how that got corrupted, maybe the dog walked on the keyboard. Seeing the number 24 I was really assuming it was in my new code because that was the line I was expecting problems from. Read error messages carefully.

**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-string-building-processing-basics/episode-8)



### Day 30: October 31, 2019
 
**Today's Progress**: 

KTC: PHP String Building and Processing Basics: Embedding Variables in a String; Embedding Complex Variables; Concatenating Strings with a Dot; Concatenating and Assigning Shorthand; Formatting a String using Placeholders; Specifying Which Argument in a Formatted String;

Docx: -

Also spent some time migrating a bit more of the D website to the new theme and reading up on 301 redirects. I now also know that Nginx does not use an .htacess file. It never occured to me before to look into the differences between Nginx and Apache.  


**Thoughts:** I got a long and very detailed response from Tonya. It was an incredible feeling, like I truly have a mentor who cares. And the answer cleared up all my questions too.
It turned out I was not only adding my code through add_action, but also calling the function from within the plugin. And while the add_action way would have worked perfectly (because the loops_start hook is called later than wp_get_current_user function is loaded), when I was calling it from within my plugin, it was way too early. And there was no need to be calling it at the moment the plugin was running.
While it felt like a really stupid mistake to be making, on the bright side, I think my understanding of how add_action works is finally solid. And I'm so grateful that Tonya took the time to help me understand.

**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-string-building-processing-basics/episode-8)



### Day 29: October 30, 2019
 
**Today's Progress**: 

KTC: PHP String Building and Processing Basics: Embedding Variables in a String

Docx: add_action - In Action, Namespacing, 

Spent a lot of time looking for a good way to add a 3d perspective carousel slider to the D website portfolio page (I'd never use one for my own stuff but they really want one). Still thinking whether I'll be using a ready solution (the best match I've been able to find so far is [this](https://codecanyon.net/item/ultimate-3d-carousel-wordpress-plugin/18948914) on Codecanyon) vs adapting the opensource [Cloud 9 Carousel](https://github.com/specious/cloud9carousel). 

The ultimate decision partly depends on how I want this thing to behave on mobile. With cloud 9 I would also have to invest time into making it swipable on touch devices. While it would be an interesting thing to get my hands into and I've found a pretty good guide, I am currently focusing on my php skills, so maybe it makes sense to just go with a ready-made solution for now.


**Thoughts:** 
Got stuch on Embedding Variables in a String yesterday and only managed to figure stuff out today. I got the main content, no problem with that, but Tonya was using wp_get_current_user which went ok for her, and kept causing a fatal error for me. 
I ended up figuring out why it wasn't working for me: wp_get_current_user is a pluggable function which means it is only loaded after the plugins. So if I want it to work in my plugin code I have to hook into init or plugins_loaded. (Took me forever to make that work, because I didn't realize that a namespaced add_action requires the full path, including the namespace to run. 
Glad I've figured it all out now, but still confused why wp_get_current_user works without the hooks for Tonya, our set ups are supposed to be the same. Wrote her a letter (kind of proud of myself that I did, reaching out is totally scary).


**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-string-building-processing-basics/episode-2)



### Day 28: October 29, 2019
 
**Today's Progress**: 

KTC: PHP String Building and Processing Basics: 

Docx: Operator Precedence; do_action The What, Real-Life Example, 


**Thoughts:** 
Feeling a bit overwhelmed by the amount of things I have to grasp before I'm any good. Maybe that's just PMS speaking.

**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-string-building-processing-basics/episode-2)



### Day 27: October 28, 2019
 
**Today's Progress**: 

KTC: PHP conditional expressions: Operator Truth Tables; Logical Operator Experiment; Operator Precedence Experiment;

KTC: PHP String Building and Processing Basics: Lab Introduction;

Docx: Operator Precedence - The What; 


**Thoughts:** 
Feeling a bit overwhelmed by the amount of things I have to grasp before I'm any good. Maybe that's just PMS speaking.

**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-string-building-processing-basics/episode-2)



### Day 26: October 27, 2019
 
**Today's Progress**: 

KTC: PHP conditional expressions: Anatomy of a Conditional Expression; Falsey Conditional Expression; Functions in the Conditional Expression; Assignment in the Conditional Expression; 

Untrusted: Levels 1-5;

Docx: -


**Thoughts:** 

**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-variables-bootcamp/episode-14)



### Day 25: October 26, 2019
 
**Today's Progress**: 

KTC: PHP Variables Bootcamp: Static Variables; Static Variables – PHP Internals; Passing Variables By Reference; Passing Variables By Reference – PHP Internals; Namespacing; Variable Scope When Including Files; Type Juggling;

Docx: -


**Thoughts:** 
Learning about static variables and passing by reference was especially cool.



**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-variables-bootcamp/episode-14)



### Day 24: October 25, 2019
 
**Today's Progress**: 

KTC: PHP Variables Bootcamp: Global Variables – PHP Internals;

Docx: -


**Thoughts:** 



**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-variables-bootcamp/episode-6)



### Day 23: October 24, 2019
 
**Today's Progress**: 

KTC: Let’s Build a PHP (Non-WordPress) Sandbox: Lab Introduction; Spin Up the Web Server; Folder Structure; Setup Composer in Your Plugin; Introduction to Whoops; Introduction to Kint;

KTC: PHP Variables Bootcamp: 

Docx: -


**Thoughts:** 
Got stuck because composer kept creating my vendor folder in the wrong location. Good thing I had already done composer setup in the plugin lab, ended up comparing the files line for line. Turned out my config somehow ended up inside the autoload brackets. Glad I figured that out.

Finished setting up my non-wordpress sandbox.


**Link to work:** [Current KTC video](https://knowthecode.io/labs/developers-guide-customizing-genesis-overview/episode-12)



### Day 22: October 23, 2019
 
**Today's Progress**: 
KTC: Overview of the Genesis Framework – Developer’s Guide to Customizing Genesis: File Architecture; Codebase Architecture; Event Naming Convention; Initializing Genesis; Setting Up Genesis; Wrap it Up;

KTC: PHP Variables Bootcamp: PHP Variables Introduction;

Docx: -


**Thoughts:** 
I've finished the beginner's track!!!


**Link to work:** [Current KTC video](https://knowthecode.io/labs/developers-guide-customizing-genesis-overview/episode-12)



### Day 21: October 22, 2019
 
**Today's Progress**: 
KTC: Overview of the Genesis Framework – Developer’s Guide to Customizing Genesis: Visual Hook Guide and the HTML – Content; Visual Hook Guide and the HTML – Sidebar; Visual Hook Guide and the HTML – Footer; Initialize & Setup Overview;

Docx: -


**Thoughts:** 
I think after I get through this lab I should spend some extra time just going through the theme code and the markup on the actual pages, so I become more confident in my understanding of what happens where. The way everything is broke up is also making me wonder what the best strategy for work is if you have a photoshop template that you are translating to genesis. First creating the layout in html/css, then breaking it up into all the blocks?
I have my presentation at D. tomorrow, and I've been unwell all day, barely managed to even watch those three videos. I think I will now get some rest (1-2 hours) and then just work on my presentation till morning. I need to focus not on making it perfect, but on simply getting it done.


**Link to work:** [Current KTC video](https://knowthecode.io/labs/developers-guide-customizing-genesis-overview/episode-12)



### Day 20: October 21, 2019
 
**Today's Progress**: 
KTC: Overview of the Genesis Framework – Developer’s Guide to Customizing Genesis: Web Page Sequence – in the Code; The Intent of HTML and its Markup; The Intent of the Theme; WordPress Event (Plugin API) Refresher; Visual Hook Guide and the HTML – Header;

Docx: WordPress add_action, the What & Syntax; WordPress remove_action, the What & Syntax; WordPress add_filter, the What & Syntax; WordPress remove_filter, the What & Syntax; WordPress do_action, the What & Syntax; WordPress apply_filters, the What & Syntax;


**Thoughts:** 
I am diving into understanding how Genesis works. I am glad that Tonya is dedicating so much attention to architecture and sound coding practices.
Depending on how I'm feeling, I sometimes start worrying a lot that my progress is too slow, and that I should know everything while I know next to nothing. That makes me panic and almost want to give up.
So this whole thing with being part of the challenge helps. It allows to feel that I've made some progress: showed up for another one of the hundred days and did my thing.


**Link to work:** [Current KTC video](https://knowthecode.io/labs/developers-guide-customizing-genesis-overview/episode-8)




### Day 19: October 20, 2019
 
**Today's Progress**: 
Had trouble with starter plugin. Turns out if I use a kint d() in the plugin file and go to the admin area, that causes the site to crash, though the same d() on a regular page is fine. Took me a while to figure out, but at least I now know what's wrong and can continue.
Didn't have time for any actual studying, because I was traveling from Petro to St. Pete and then catching my breath.

**Thoughts:** 


**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-101-gentle-introduction-wordpress-programming/episode-13)




### Day 18: October 19, 2019
 
**Today's Progress**: 
KTC: Let’s Build a WordPress Starter Sandbox Plugin: Let's test it out; 

KTC: Overview of the Genesis Framework – Developer’s Guide to Customizing Genesis: Lab Introduction; The Why of the Genesis Framework; Web Page Sequence;  

**Thoughts:** 


**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-101-gentle-introduction-wordpress-programming/episode-13)



### Day 17: October 18, 2019
 
**Today's Progress**: 
KTC: PHP 101: What's the deal with scope?; Naming Stuff; Putting it All Together; Where do I go from here?;

KTC: Let’s Build a WordPress Starter Sandbox Plugin: Lab Introduction; Plugin File and Folder Structure; Plugin Header DocBlock; What is a DocBlock?; Setup Composer in Your Plugin; Introduction to Kint; Introduction to Whoops;

**Thoughts:** (written on day 18) I was almost done with the plugin, but then I was suddenly exhausted (I don't know whether it was organically or I somehow took my pills wrong) and had to emergency crash. Can't get my Whoops to autoload for some reason. Hope to fix that today.


**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-101-gentle-introduction-wordpress-programming/episode-13)



### Day 16: October 17, 2019
 
**Today's Progress**: 
KTC: PHP 101: To Run or Not to Run – Making Decisions; Sequencing – Yup, code runs in order; Repeating code using Loops; Building Strings with Dots and Variables;

**Thoughts:** 


**Link to work:** [Current KTC video](https://knowthecode.io/labs/lets-build-wordpress-starter-plugin/episode-8  )



### Day 15: October 16, 2019
 
**Today's Progress**: 
KTC: PHP 101: Gentle Introduction to WordPress Programming: What’s the deal with Variables?; Break Up Code into Logical Parts; Subroutines – Behold the function; Loading Files to Run;

**Thoughts:** (written on day 16) Too tired for thoughts.


**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-101-gentle-introduction-wordpress-programming/episode-5)



### Day 14: October 15, 2019
 
**Today's Progress**: 
KTC: PHP 101: Gentle Introduction to WordPress Programming: Lab Introduction; What is PHP? Why use it?; Why and how does WordPress use PHP?; Syntax Basics;

**Thoughts:** 
It's things I'm already using, but I wanted to see them explained and laid out in detail before I dive into anything more complicated, and Tonya does recommend to  complete the beginner track before diving into the theme development track.
I might be doing a project together with my brother, and it would be cool to use that as a place to try out my Genesis customization track finds.

**Link to work:** [Current KTC video](https://knowthecode.io/labs/php-101-gentle-introduction-wordpress-programming/episode-5)



### Day 13: October 14, 2019
 
**Today's Progress**: 
Round 12 of Flexbox Zombies (final round). Spent some time searching for projects to further practice Flexbox on, considering  Wes Bos's code-alongs. Watched Crossbrowser flexbox support and autoprefixer.

**Thoughts:** 
Finished Flexbox Zombies today! The last round was easier than I thought. I expected the final challenges to be more difficult. The game really helped me make sense of flexbox. I think I really have the basic properties down now, although I'm still not sure how to really make it an integral part of my daily practice. I will be looking into sample projects to build, I guess.
There is also Dave's CCS grid game, but I will be doing that a bit later, I want to space these out (and also earn some money first, so that I can afford it).

**Link to work:** [Flexbox Zombies](https://flexboxzombies.com/p/flexbox-zombies), [Current KTC video](https://knowthecode.io/labs/git-contributing/contributors-workflow-big-picture)



### Day 12: October 13, 2019
 
**Today's Progress**: 
Round 11 of Flexbox Zombies (shorthand). 
Know the Code: Simply Git: Store & Document a Snapshot; Git Status – View State of Working & Staging; Git Log - View History; Unstage Changes; Rollback Changes in Working Directory; Fix the Last Commit Message; Add More Changes to Last Commit; Uncommit Last Commit;

**Thoughts:** 
Git is starting to make more sense. Practicing more tomorrow. Flexbox is feeling better too, but I feel like when I'm done with the Zomibe game, I need to find either some assignments to practice Flexbox, or come up with a project. A way to put it into real-life practice, but in a way that allows to practice bit by bit.

**Link to work:** [Flexbox Zombies](https://flexboxzombies.com/p/flexbox-zombies), [Current KTC video](https://knowthecode.io/labs/git-contributing/contributors-workflow-big-picture)



### Day 11: October 12, 2019
 
**Today's Progress**: 
Round 10 of Flexbox Zombies (shorthand). 
Know the Code: Simply Git: Git Add – Stage Small Changes;

**Thoughts:** 
(Written on day 10): managed to struggle through about half an hour of Flexbox Zombies. I was extremely tired, so when I felt I was no longer being productive in the least I gave up and went to sleep. Better today though, got a full night's rest.

**Link to work:** [Flexbox Zombies](https://flexboxzombies.com/p/flexbox-zombies)



### Day 10: October 11, 2019
 
**Today's Progress**: 
Round 9 of Flexbox Zombies (flex-wrap). 
Know the Code: Simply Git: Git Add – Stage Small Changes;

**Thoughts:** 

**Link to work:** [Flexbox Zombies](https://flexboxzombies.com/p/flexbox-zombies), [Current KTC video](https://knowthecode.io/labs/simply-git/big-picture)



### Day 9: October 10, 2019
 
**Today's Progress**: 
Round 8 of Flexbox Zombies (order). 
Know the Code: Simply Git: Git Init – Put New Project into Version Control; Original Theme Snapshot – Your First Commit;

**Thoughts:** 
Was tired after D. meeting and transporting my sculptures, so went right to sleep. (written on day 9)

**Link to work:** [Flexbox Zombies](https://flexboxzombies.com/p/flexbox-zombies), [Current KTC video](https://knowthecode.io/labs/simply-git/big-picture)



### Day 8: October 9, 2019
 
**Today's Progress**: 
Round 8 of Flexbox Zombies (order). 
Know the Code: Tune PhpStorm for WordPress DevelopWhy You Need PhpStorm; Setup the Sandbox Site; Tune the Look; Be Faster with Keymappings; Split-Screen Coding Windows; Enable WordPress & Jump to Hook; Jump to Function; WordPress Coding Standard; Configuring to Other Coding Standards; Autocompletions. Inline and Online Documentation.; Function DocBlock Template; Selecting Multiple Instances (Multi-Cursor); Shortcuts & Snippets (Live Templates); Refactoring Tools;

**Thoughts:** 
I was so tired I fell right asleep and didn't even tweet my progress or write up my thoughts. (written on day 8)

**Link to work:** [Flexbox Zombies](https://flexboxzombies.com/p/flexbox-zombies), [Current KTC video](https://knowthecode.io/labs/simply-git/big-picture)



### Day 7: October 8, 2019
 
**Today's Progress**: 
Rounds 6-7 of Flexbox Zombies (flex-shrink and flex-basis). 
Lambda school Precourse: Introduction to CSS.
Know the Code: Simply Git: Lab introduction, The Big Picture, 3 Locals - Working, Staging & Storage.

**Thoughts:** 
It's a bit hard to eyeball the ratios for the shrinking/growing zombies, so with this round a lot of the time I have to try over and over again to get it right. I get the principle, but keep estimating the values wrong.

I rewrote my lost templates today, and I was much faster and better this time, and I think my code was cleaner too.  Went over what I need to write up my online store proposal for D. Writing that in the morning. 

Watched the free part (first three videos) of the Simply Git lab on KTC, hoping to start using version control within a week. At least in a very basic way.

It's impressive how much the zombie game is helping me with the Flexbox logic, it really made putting together the new template a lot easier.

I am writing here both about study and work, because the two end up being intertwined. Also managed to finish another square pic today.


**Link to work:** [Flexbox Zombies](https://flexboxzombies.com/p/flexbox-zombies)
                  [Lambda School](https://apply.lambdaschool.com/)
                  [Current KTC video](https://knowthecode.io/labs/simply-git/big-picture)



### Day 6: October 7, 2019
 
**Today's Progress**: 
Rounds 4-5 of Flexbox Zombies (align-self, flex-grow). 
Lambda school Precourse: Introduction to web development fundamentals.
Lambda school Precourse: Introduction to HTML.

**Thoughts:** 
I found out that Lambda school ISA is unavailable in Russia halfway through the application process. That makes perfect sense, really, why would it be, but I was really upset. For a moment I felt like maybe I didn't have to go through this alone. The structure and the mentoring and the support were such an appealing prospect. But obviously there's no world in which I can afford the $20k payment without the ISA. 
I decided to go through the Precourse either way. It has all the things I need to refresh for Know the Code, so it's as good a place as any.

Made some progress on the websites for artists program with K. Finished the report for work but didn't find it in me to redo the lost template, mostly because I was unwell from the erratic sleep (and lack thereof). Planning to get up in an hour or so and get that done.

Got some drawing done (even with the studies and work and the sleep|non sleep thing).


**Link to work:** [Flexbox Zombies](https://flexboxzombies.com/p/flexbox-zombies)
                  [Lambda School](https://apply.lambdaschool.com/)



### Day 5: October 6, 2019
 
**Today's Progress**: 
Got through three rounds of Flexbox Zombies. 

**Thoughts:** 
The Beginner track says to brush up on html, css and basic javascript before going further, and flexbox is one of those things that I can't get to comfortably using without looking stuff up in the manual constantly. And since I'll be building a few Flexbox-based layouts on the deviz website this week and the coming one, I thought it made sense to get Flexbox to an automatic level, so I don't have to think about it or look it up constantly.
Other than that writing up my monthly report for deviz, need that thing done by morning. As I was writing it, I discovered that I'd lost the half the work I'd done on the job opening page templates. I still have the css, but my php templates are gone (my bad, lost them while reinstalling Local). I am hoping to get comfortable using Git within the coming couple of weeks so something like that never happens again.

Also wrote up the basics of the program for the Websites for Artists project K. and I will be doing. That's not part of my studies, but it's part of me both as an artist, and a developer, so it's important.


**Link to work:** [Flexbox Zombies](https://flexboxzombies.com/p/flexbox-zombies)



### Day 4: October 5, 2019
 
**Today's Progress**: 
Zoomed through the 24 levels of Flexbox Froggy to refresh Flexbox. 

**Thoughts:** 
Needed Flexbox for my work project (the employee profiles and contact information are displayed on cards that it makes sense to use Flexbox with). Then spent most of the night fixing the AAA plugin for bark. But in truth saying J. did most of the work is an understatement. Though my basic idea was true, I could never have figured out the kink that was in the way without him. But I learned a lot watching him work, problem solve and troubleshoot.

**Link to work:** [Flexbox Froggy](https://flexboxfroggy.com/)



### Day 3: October 4, 2019
 
**Today's Progress**: 
Watched:
   - Building blocks of programming: Basics of Iteration, Order of Execution, Abstraction, Scoping – Who Can Communicate With Whom; => finished step 6.

**Thoughts:** 
So I've finished the steps of the beginner's track where I mostly listen and now need to decide whether I'm going to go through steps 7 and 8 on Codecademy, as recommended, or brush up on that stuff elsewhere. The courses there were initially recommended as free ones, but that is no longer the case for half of them. There is a one week trial period, so maybe if I try hard enough, I can manage to get through on time. I'm not worried about the html and css, but the JavaScript might put a spike or two in my wheels.
Also, I need to stop procrastinating my work project, so I'm pausing my studies for today. Two things I need to do: a brief outline of my websites for artists idea for the talk with N, and write up the function that will display employees and their details on the deviz contact pages.


**Link to work:** [Current NKC video](
https://knowthecode.io/labs/building-blocks-of-programming/episode-10)



### Day 2: October 3, 2019
 
**Today's Progress**: 
Watched:
  - Computational thinking: Pseudocode; => finished Step 4
  - Types of data: Lab introduction, Primitive Data Type, Composite Data Type, Special Data Type, Abstract Data Type; => finished Step 5
  - Building blocks of programming: Lab Introduction, User-Friendly Expression of Information, Fundamentals of Syntax, Decision branching - if/then/else, Decision branching - switch/case

**Thoughts:** 
It's a bit hard to focus today, I'm in a jittery state because my sleep cycle is very off, and the videos today don't require any actions, just focusing on the info. But I've managed to finish steps five anad six, and should be done with seven soon, and after that it gets more hands-on.

**Link to work:** [Current NKC video](
https://knowthecode.io/labs/building-blocks-of-programming/episode-6)



### Day 1: October 2, 2019

**Today's Progress**: Watched Computational thinking and Computational visualization on KTC. (that's for the challenge part, probably about half an hour total). Other than that spent the whole day preparing the new deviz site for tomorrow's meeting which I then cancelled at the last moment, because I can't go two nights without sleep.
J ended up doing most of the work for the function to rewrite the People CPT title using ACF fields. I was tired and scared and frozen minded.

**Thoughts:** Seems like just the kind of foundation I've been struggling with finding. I don't know how code and web dev will relate to my art, but I hope at some point those two lines will merge.

**Link to work:** [Current NKC video](
http://knowthecode.io/labs/problem-solving-expression/episode-4)



### Day 0: October 1, 2019

**Today's Progress**: Finished Step 1 – A Gentle Introduction, Step 3 Introduction to Computation and Programming – Overview, Started Step 4 - Problem Solving Expression (did Step 2 - Setup Your Development Machine yesterday).

**Thoughts:** Seems like just the kind of foundation I've been struggling with finding. I don't know how code and web dev will relate to my art, but I hope at some point those two lines will merge.

**Link to work:** [Current NKC video](https://knowthecode.io/labs/problem-solving-expression/episode-2)
