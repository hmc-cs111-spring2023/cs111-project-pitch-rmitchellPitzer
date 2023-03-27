# Contract

## Goals

_At a high level, what do you most want to get out of this project, and why?_

I would hope to get an understanding of the different ways Domain Specific Languages are made and what techniques can be used to make them. While we’ve been reading about Domain Specific Language design and have even made a DSL in the form of our Piconot language, I do think getting to explore different design principles and getting to run into pitfalls of DSL design naturally will help me learn about DSL design, which I can then use in later projects. I’d also love to put into practice what we’ve been learning about in DSL’s, like investigating the benefits and drawbacks of internal/external DSL’s, ease of use, natural language influence, and which programming languages are best suited to particular needs.
	I also hope to have a project at the end that I will be proud of. Naturally I’m very interested in this topic (calendar/schedule making) as it always seems needlessly complicated to create a schedule in Google Calendar. I would want something that not only would I be proud to have made and show off, but also one I would want to use to fix that problem of needlessly complicated schedule creation. To elaborate on this, it feels like I need to click through too many options in Google Calendar to make a new event and time/dates may change when I go to edit them so I need to edit the time two or three times for any given event. I hope that by making a DSL that would easily allow for the creation of events by writing to a text file I can have something that would be useful not only to myself but to others as well.
	Something else I’d want to get out of the project is a frontend user interface. While I’ve already discussed this with professor Weidermann, and it is at best a stretch goal if time allows for it, I would hope to be able to create a preview window similar to how context free implements a preview window. I do have some experience with creating desktop apps using Javascript frameworks, so while I would love to do something like that, I do acknowledge that it’s not required and will only be investigated if time allows for it.


## Concepts / skills

_What concepts and / or skills from class would you like to work on, as part of your
project? Are there any concepts / skills that we haven't covered in class that you would
like to work on, as part of your project (for example, other things related to DSLs that
you have come across, or topics from other classes)? Why are you interested in working on
these things?_

I think one of the things I’m most interested in is transferring the knowledge I have in Scala and DSL design to other host languages. I think that if I can get an idea of how to write, for instance, parser combinators in other languages, or more broadly, how to write external DSL’s in other languages, I should be able to transfer that knowledge to other languages in the future and could almost lessen the tradeoffs when deciding on a host language in the future. 
	I also want to further grow my experience in Scala. While I do feel comfortable working in Scala, I do think my Piconot assignment was compromised and sacrificed much of what I wanted in it due to not knowing the language or libraries well enough. I think that working on those skills will be beneficial to this project and to other projects in the future. 
	I mentioned earlier that I’d want to work on a frontend user interface for this project to preview changes, but it is completely unnecessary and I would only work on it should time allow for it. As for concepts and skills not covered in class, I think investigating other host languages would be useful. While I would like to work on this project using Scala, if I investigate other host languages and find others that are more suitable for this project I would like to use those instead, which I don’t think has been covered in class. 
	I’m most interested in working on these things because I either want to grow my experience in DSL design and Scala, as well as learn new ideas and techniques that will be useful in future projects. Transferring skills to other host languages, learning more about Scala, learning more about external DSL design, growing my experience in UX design are all things that are important to me and would definitely be beneficial going forward.


## Time management plan

_How do you plan to set aside time outside of class, to work on the project? Are there
intermediate milestones that you can create, to help you make consistent progress?_

  While much of this project is still unknown to me, I do have some ideas as to how I can manage my time, but I don’t expect this timeline to stay the same throughout the project, and would not be surprised if I adjust it to better fit the project. I hope to work ~4-8 hours a week outside of class on this project. Currently that is around the time I spend on the HW assignments for this class, and given that most of the classes going forward will be studio classes, I don’t think time will be a concern on this project. I will log hours spent on this project to further adjust timelines/expectations.
The milestones are broken down week by week. Seeing that there are 5 weeks to work on this, I hope to spend my time accordingly:
Week 1: Investigate benefits and tradeoffs between host languages, and determine whether an external/internal implementation will work best. Finalize the syntax/language design knowing this. Decide on a general architecture/structure of the DSL (I know that professor Wiedermann already discussed making two distinct DSL’s: One for letting the user create events using the DSL syntax, which can then could compile toiCalendar, and another for taking in that iCalendar input and showing a preview in either Excel or HTML/CSS. While this is very broad/vague, I hope by the end of week 1 to have this finalized). This should also require research on different calendar DSL’s such as iCalendar and understanding how an iCalendar file could be output using a language, whether through writing to a file manually or by using libraries in the host language.
Week 2: Make progress in implementing the first DSL: Parsing user input. This will be my primary focus, implementing parsing combinators and reading input from a file/text stream. I hope by the end of this week I will have fully implemented the syntax for the user.
Week 3: Finish the first DSL. I hope by the end of this week the DSL will be able to output to iCalendar or a specific filetype that could then be read into the second DSL. This will require some foresight to understand how the second DSL should read in input. Hopefully most of the design language and implementation of parsing user input will be done already. I am worried about exporting to iCalendar, as I do not know whether using a library (or if it exists!) or writing my own solution would be best. I hope to determine that in week 3 and to have a solution.
Week 4: Work on the second DSL. Make progress in outputting to a HTML/CSS file. I believe that my work in the previous weeks should make this easier as much of the exploratory work should be done. Therefore, I hope that by the end of this week I will have the preview options and the second DSL nearly complete.
Week 5: Finish the second DSL, finish the previews, link everything together. I am unsure how much time this will take, so I am leaving this a bit vague for the moment. I might barely have enough time to get this submitted, or I might have more than enough time. In that case, I hope to develop the preview/output to HTML+CSS/Excel further to incorporate a user interface/preview option.

## Teamwork plan

_If you plan to work with someone else on the project, what is your plan for
collaborating? What part(s) do you think you might do together? What part(s) are you
considering doing separately? How will you hold one another accountable to make regular
progress?_

I do not plan to work in a team.

## Critique plan

_What will you do to make sure that you can give consistent and actionable feedback to
other people in the class?_

  I would hope that my experience in working on this project will give me some idea of how to critique others’ projects. However, that’s not really going to ensure I give consistent and helpful feedback to others. To ensure this, I will (if professor Wiedermann allows it!) read the project’s contract and proposal, understand the timeline the student is working with, understand the project’s premise, and know what goals need to be met by the next milestone. By doing this I can give constructive feedback on how best to approach the next milestone.
	To ensure I give actionable feedback I hope to review the feedback I’ve given and received for past projects, and to look back at my Fowler reading notes in assignment 1. This should help me better understand DSL design ideas before I critique another student’s DSL, and I also hope that my experience in making this project will give me some insight into DSL design which could be used in critiquing other students. 


## Success

_At the end of the semester, what would you be proud to show or tell someone about your
project?_

While I really love the idea of a user interface, with a preview option, and a fully polished and working DSL language that others could use, I think I would be happy knowing I put in lots of effort and learned a lot through this project. In that sense, I would just be proud to tell or show others the project knowing I put an honest effort into it.
	That being said, I think if I could make it usable for others and easy to get started for people with no experience in Computer Science I would be very happy showing others how to use it and how to install it. The project would be something I’d personally want to use, and if others could use it I would be very proud of it. 



## Assessment

_Looking over your responses to the previous questions, what would you consider to be an
"A-" for your project? What would you consider to be an "A"?_


I think an A- would be a project that would be well packaged for beginners to use, bug free, polished enough such that users could easily use and understand it, and generally nice to use. All milestones and critiques are met, and the previews in HTML/CSS aren’t ugly and are presentable. I also think it’d be nice to have documentation on Github, showing how to use the DSL and how to get started with it.
	I think an A would be a project that meets all the requirements of an A-, with the added frontend user interface component. While I know this isn’t required, and while I know putting it at A means it would be impossible to get an A if I don’t have time to implement it, I really like the idea of making a preview similar to context free, and in a weird way I think the idea that should I get my work done ahead of schedule I would be able to implement a user interface would motivate me to work on this. Hence, A if I can get everything possible done :) 


