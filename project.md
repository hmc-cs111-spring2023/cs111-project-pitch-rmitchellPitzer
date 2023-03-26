# Project proposal

## The user and a language

This section describes who the project would serve and why a language might be a
good way to meet their needs.

### What's the need?

_What need is met by your idea? Who are you helping? What is that person's
experience like now? What would their experience be like if you could help
them?_


The need met involves creating a schedule or calendar. Google Calendar for instance provides many options for creating a schedule. However, I do not need so many features like out of office, time insights, guests, google meet, and sometimes creating or editing an event can be frustrating due to how events times sometimes change after you edit them. This process for creating or editing events requires multiple clicks through different menus and different options, which takes time and can frustrate the user and ultimately I think users would appreciate it if an option to quickly type out a file that would then be used to make a schedule that’d fit their needs best existed. By creating a way to quickly make schedules using a DSL I would be helping people like me who don’t depend on different calendars’ many options, and instead just want a simple calendar to view their events and schedules.


### Why a language?

_Why is a DSL appropriate for your user(s)? How does it address the need?_



While other DSL’s such as Icalendar exist, it can be difficult to edit or make them by just using text files. The default way to edit these is to use a calendar app or website, which can be slower and more difficult to use. By creating a DSL, many of the unnecessary features and bloat can be removed, limiting the complexity. This should result in a simple to use, easy to understand language that can be used by anyone to quickly create schedules that can then be previewed or exported to other formats. I also hope that by giving the user the option to use syntax inspired by natural language or by using syntax that creates a schedule as quick as possible, the language will be useful by both people with limited experience in DSL’s and power users who have experience in Computer Science and DSL’s.


### Why you?

_What excites you about this idea? How did you come up with it?_


I originally came up with the idea out of frustration for Google Calendar. I have terrible organization/time management, so a schedule is very important to me. However, I don’t want an overly complicated schedule that’s very detailed because then it will be difficult for me to pay attention to it or make changes. In a sense, I would be putting more effort into maintaining the calendar than I would be in attending the events on the calendar. However, the options given by Google Calendar can sometimes slow down the user and interacting with the calendar can be very slow. I wanted an option to just quickly type out an event name, start/end time, days it occurs on, and a description if it’s needed. 
	This led me to the idea of making a DSL by limiting the features a lot of calendar apps have, and by doing so creating a robust DSL that could quickly create new schedules and events. I’m ultimately excited about this idea because I personally would use it. I think it would help me be more organized and manage my time better, and if there are people who feel similarly with their calendar app, it would be amazing if this could help them make schedules as well.


### Domain

_Describe the project's domain in five words._

Making schedules easier and faster


### Interface (syntax)

_How might the user interact with the language? What does programming look
like? Why is this the right way to interact with the problem domain?_

While I haven’t finalized the syntax yet, I hope the user will interact with the language by writing out a text file. This could be done in any text editor, or in a command line terminal, or in some type of preview option. The user would write out a line for a single event, specify some arguments like start/end time, start/end day, title, description, and what days it repeats on. I also hope to incorporate natural language, so a user could for instance type out “set ‘CS111’ describing ‘Domain Specific Languages in Shanahan 2465’ on Monday Wednesday from 1:15pm to 2:30pm”. But I also hope to give the option for the user to not need natural language, typing for that same event “‘CS111’ ‘Domain Specific Languages in Shanahan 2465’ M W 1:15pm 2:30pm”. I think this is the right way to interact with the problem domain because this will create an event much quicker than interacting with a calendar app. I also think it’s much more intuitive than Icalendar.


### Operation (semantics)

_What might happen when a program runs? How does a program interact with the
user? What kinds of errors might occur, and how might they be communicated to
the user?_

While I haven’t finalized the syntax/semantics of the DSL yet, I would like to use an external DSL using parser combinators to read in the user input. The program the user writes would then be read, and then this could either result in an Icalendar ICS file, or it could be passed to a second DSL which will visualize it in a HTML/Excel file. 
	Some errors that might occur could be type errors, such as inputting “29:72pm” for the start time, or syntax errors such as not giving a title for the event. I think this could be avoided by simply catching and returning errors for these. These could then be communicated to the user via error messages. I know there are probably more errors that are possible, but I can not think of any because it is 3:15 am and I am very tired. 


### Expressiveness

_What should be easy to do in this language? What should be possible, but
difficult? What should be impossible or very difficult?_

I want it to be very very easy to create simple events. This should take less than 20 seconds max. I also want these events to be output as a file which could then be imported to another calendar app. This should be easy by limiting the number of arguments to pass to the DSL.
	I think it should be possible, but difficult to write very long, descriptive events. I think with this DSL I want to prioritize speed/ease of use, and if a user is trying to write a very long title or description I think writing that in a text file or terminal might be difficult, but still possible.
	It should be impossible to take advantage of much of the features offered by calendar apps. This would include google meet links, different types of events like tasks or focus time or out of office, and calendar event ownership. The user could import the ICS file output into a calendar app and then add these new features, but I think I would want to at least limit this in the DSL. 


### Related work

_Are there any other DSLs in this domain? If not, describe how you know there
aren't and conjecture why not. If so, describe them and provide links. How well
do they address the need? Are there any particularly admirable qualities of the
language? Are there parts of the language you think could be improved?_

There are many DSL’s for creating calendars and schedules, but I will only describe two in this pitch: ICalendar and Coursicle. 
	ICalendar is a standard created in 1998 to describe calendaring and scheduling information. More information can be found here: 
	https://www.ietf.org/rfc/rfc2445.txt
	ICalendar is very capable, and the text document linked above has over a 100 pages describing the standard. It’s also supported by many calendar apps, which is fantastic! I think ICalendar covers nearly everything anyone would want in a calendar app, and to that extent it addresses the need for a calendar standard very well. That said, I think editing ICalendar files leaves much to be desired. For instance, opening my calendar into a plain text editor or an excel sheet shows 3044 lines, each referring to some property of the calendar or an event. Editing this in text is nearly impossible, so one would use a calendar app to do this, but many of the calendar options can be slow or frustrating to use. I admire the support of ICalendar from other software and the insane amount of features it has, but I think using it with excel or text editors can be improved.
	On the other hand, there are online schedule makers such as Coursicle, as seen here:
www.coursicle.com 
These are lightweight weekly schedule makers with limited options, so events can quickly be created and then exported to a number of different file types, such as .ics, images, or printing it. This is closer to my project’s idea than to the ICalendar standard. I think it’s admirable that a lightweight, easy to visualize and use website can quickly make schedules which could then be exported and used in many calendar apps. I also like some features it has such as having options for “MWF”, “TuTh”, and “MW” available for repeating events. However, I feel like this can be improved upon and still would most likely not be as fast as editing a text file. Ultimately, I would want a way to limit the capabilities of the DSL to having similar options that Coursicle has, while also allowing for editing using a text editor to speed up the process.


## The Project

This section examines whether the idea makes for a good CS 111 project.

### Suitability

_If someone were to work on this project, what percentage of their time would be
spent directly engaging in the **language** aspects of this project (e.g.,
making language design decisions), as opposed to "systems" aspects of the
project (e.g., implementing a complicated semantics that doesn't require a lot
of language design)?_

I think this project would skew more towards systems. If I had to say, probably 70% systems and 30% language design. There are opportunities to work on the language aspect of it however. I would like to implement parser combinators such that users could either use natural language when describing an event or type only required syntax so as to make making a course calendar very quick. However, the DSL’s being made for this project largely focus on compatibility and exporting to ICS, and then also being able to parse and display them in a preview. I think most of the time spent will be on implementing ICS export/parsing ICS for the second DSL, which should mostly be systems focused.


### Scope

_How big an idea is this? How ambitious is this project?_


I think the project isn’t too big of an idea. I think others have worked on similar ideas and there already is an ICS standard. Therefore there should be libraries I can utilize and I can use much of the knowledge from previous HW assignments in this project. However, I think working on two DSL’s might prove to be difficult and might be time consuming. I think the project should not be too ambitious because there is already much documentation on ICS and different calendar standards, but it might be difficult to fit everything I want to do into 5 weeks should I run into any roadblocks.


### Benefits and drawbacks

_Why might this be a good idea for a project? Why might this not be a good idea
project?_

I think this is a fantastic idea for a project because it’s something I’m personally interested in. I also think it’s a good idea because it could help others stay organized, and it could help myself stay organized. It’s also something that could be used to explore different tradeoffs for host languages and DSL design techniques.
I think it might not be a good idea because it will largely be focused on systems instead of language design. This might give me a limited understanding of DSL’s, and might instead leave me with a better understanding of the .ICS file type. However, professor Weidermann has mentioned it’s a great idea and that it’s viable, so that shouldn’t be too big of a problem.
