# DDD North 2017 Married to the Mob (Programming)

## Intro

Thank you for being here, I realise I am standing between you and lunch.

Who I am - principal dev, sage, run local meetup groups .net and agile. Also lead Makers and Creators at Campus North

I am happy to take questions at any time.

I would like to share what I have learned about the technique of Mob programming in the last 18 months or so. What is mob programming, how to do it, is Woody Zuill an evil genius? Also embedded in the middle of that is a overlooked technique which I think has some massive benefits and I will explore that later.

Warning - there will be humblebrags or name dropping during this talk. Sorry.


## Agile

Who here considers they are working in an agile way? 
  - Scrum?
  - Standups?
  - Sprints?
  - Retrospectives?
  - Code Reviews?
  - Pairing?


## Tradition

Lone developer working in cube/silo and having a comparatively long feedback loop between writing code and having it used.
Mitigations for that are code review, quality gates, various QA strategies - mainly manual testing, demonstration and sign offs at the end of the project. All kinds of Kubuki because of big batch size. 


- XP & Pairing
  - Two devs sitting at a keyboard, swapping between them
  - Driver has an idea of how to proceed and types code
  - Navigator is thinking about the road ahead
  - Swap when person stalls and other person has an idea
  - One person typing their ideas, one person nodding along
  - Not talking often
  - How many people consider themselves XP?
  - How many do some level of pairing?
  - What do you find difficult about it?
  - Who has tried it and didn't like it?
  - Why didn't you like it?
  
  
- Anti-Patterns
  - Dev typing (not explaining verbally)
  - Other Dev reading what is typed and making sense of it.
  - Strong personalities
  - Often see one person typing and another is the nodding dog.
  - Dreyfuss Model of Skill Acquisition
  - Pairing with Beginners
  - Pairing Experts
  - Pairing Expert and Senior



## XP 
XP came along to try and resolve some of those issues and shorten the feedback loop - code review gets done all the time with pairing, continuous integration gives feedback on build issues, automated tests, smoke tests give quick feedback on overall quality (although not a guarantee). Smaller batches.

https://www.youtube.com/watch?v=unDxq76JcvE XP Turns 20


## My Journey

Least original person - Come up with all kinds of good ideas. Invented ReST after it had been invented. Invented something like No Estimates - twitter told me I hadn't invented it. Refactoring techniques - Woody - Ah yes we do that...

As part of my role as a principal dev, I run lunchtime coding dojos for some of the less experienced devs or those looking to move up to a dev role. This is a deliberate discovery setup where the goal is to learn something, not to complete a program. I started off setting a small programming problem each week and trying TDD in pairs and threes. This worked quite well until a chance conversation with Emily Bache turned me on to Randori style programming. What I found was the beginners got stuck very easily trying to write code as an inexperienced pair and would get bogged down in the wrong thing. Randori meant that we collapsed the pairs into a single group with the person who thought they could progress at the keyboard and the rest of the group would watch. That person would get stuck but someone else would be inspired by that idea and would take the keyboard and be able to add something else. And little by little we solved some problems, and devs progressed. 3 Test engineers are now developers thanks to that process. 

Meanwhile, Woody Zuill was hired at Hunter Industries to help a development team to improve their quality and deliver some projects. The team identified the shortcomings in their knowledge and so they took an action to meet for an hour each morning to do a dojo like activity to practice techniques like refactoring, they had a lunchtime study session for dev books. After each session the devs would return to their desks/silos and begin the real work of the day. What they found was they missed working as a group and discussed trying an experiment....

Meanwhile...

All through this gradual evolution of the dojo process I was using the socratic method to question what the group was thinking about - using questions to direct their thoughts to one thing or another. Also I encouraged the person typing to describe what it was that they were doing. But! I noticed that some people were reluctant to volunteer to type and were embarrassed to speak up, unsure of syntax etc. when all eyes were on them.

So we decided to turn the randori style inside out and have the person at the keyboard be the person to just concentrate on typing with the person with the actual idea would dictate what to do. This meant that the person at the keyboard got to type in the language and got the syntax explained to them as they went along, the person with the idea got to struggle with expressing themselves clearly, and the rest of the group got to hear what they were thinking and contribute.

This worked really well and has stayed as the model for our coding dojos. I was so proud of this that tweeted about this new invention and would came back with a "well actually?" Woody. Evil Genius Woody.

And he told me all about what had been happening at Hunter. How the team had started working together as a group on their tasks almost full time and were getting great results! Curses another invention foiled.


## XP++

So what is Mob Programming? (that's a lovely bit of code you got there, it would be a pity if anything were to happen to it)
Where > 3 people collaborate on a single computer to solve a problem or series of problems.

Woody's quote says it best:

"All the brilliant people working on the same thing, at the same time, in the same space..."

"...and on the same computer"

It's an extension of pair programming with the next highest collective noun being a "mob".
Turn up the good echoing XP

## Things you will need

There are rules and guidelines to follow.

Mobbing components 
Rules
keyboard
navigator
mob
keyboard
big screen
local laptop?


## Rules

  - Kindness (sprinkle)
  - Consideration
  - Respect
  - Use strong style pairing (important)

## Roles

From the XP roles, we have a driver, and the rest of the mob. If the mob is particularly big you might need to direct efforts through single nominated navigator who changes when the driver changes. If it's bigger still you may need a facilitator too.
Everyone in the team has a role and the roles swap amongst members of the team every few minutes.

## Guidelines

  - Driver or Typist
  Driver is the least interesting piece of this whole arrangement. You are the person 
    - Listen to what mob is asking
    - Translate that to code
    - Work with incomplete understanding at short intervals
    - Patience!
    - Don't premature challenge - leads endless discussions
    - Write the code, talk about the code, change - arguments fall away
  
  - Rest of Mob
    - Discover what the next logical step is
    - Work collaboratively
    - What is the next step and park everything else
    - Talk at right level of abstraction for typist
      - Inexperienced
      - Synatax level
      - Extract method
      - Move to line, select lines, right click...
      - Communication is difficult
      - Challenge is hard to 
      
         - Responsible to help understanding
    - If you don't understand - have courage to ask
 
      Driver
At the keyboard
Trust the navigator
Computer of the SS enterprise

Navigator
Verbal instructions
Talk at highest level of abstraction


Facilitator?

Timer is the last member of the team
Timer - switch to new keyboard every 5 minutes, 10 minutes

  - Optional Navigator

## Environment components
  
  - Shyness
  - Everyone must be able to see the screen
  - Big screens
  - Wireless keyboard and mouse
  - Local laptop if like me you have a harder time looking with head at unnatural angle.




## Features

Amplified learning, easy for everyone to keep up to speed with problem being solved. 
Amplified problems, slowness is amplified in tests, n x time for everyone. 
 - Shared understanding.
    - Seeing code artefact
    - Short periods of time
    - Effective - typist duration is very small.
    New mob nobody is in sync.

## What it is not

Not solo programming with an audience
Rockstar pirate ninja


For me the most interesting part of mob programming is the way it turns pairing inside out. Here's an example mob



## Strong Style Pairing

Llewellyn Falco - strong style pairing - this is the technique I believe is the big difference and the one thing that you can use to make immediate improvements. 

"For an idea to go from your head into the computer it MUST go through someone else's hands"

http://llewellynfalco.blogspot.co.uk/2014/06/llewellyns-strong-style-pairing.html

http://visible-quality.blogspot.co.uk/2015/08/being-navigator-in-strong-style-pairing.html
http://blog.xebia.com/practical-styles-of-pair-programming/


## Rubber Ducks

Like rubber ducking, find faults by vocalising what you are thinking. Much better than thinking in own head.

## Tiredness Kills

 - Some teams hate typing - switching is easy
 - Some with high trust - it's a finish the thought kind of thing
 - Others need a physical timer to force a change
   
   
## Other Approaches

Mob Testing - talk to Mike L about this.

Mob RPG

## Implemented by...

  - LateRooms.com
  - Hunter Industries
  - Alaska Airlines
  - Unruly Media
  - Industrial Logic
  - Menlo Innovations
  - Blue Fruit  
  
  
## Takeaways
  - Not here to tell you that you have to do or this is the only way to do it
  - But - It is possible and teams all over the world are doing it and having success.
  - Woody has hundreds of cases - travels the world advising teams
  - Pair
  - Do strong style pairing !!!
  - Mob when you can - hard to do culture change to do full mobbing
  - Mob ad-hoc seems to be good second best
  - Hopfully it will catch on

  
## Research 

Research backs it up, a study published in the Journal of Personality and Social Psychology looked at the effects of group size on problem solving. Researchers compared the problem-solving performance of small groups to that of individuals working alone. 
The results of the study indicate that groups of three solve problems better than even the best individuals working alone. What are the implications of these results? The findings may be useful in academics, where problem solving groups might serve as an effective learning tool. Groups and teams in science, health care, and business may also find these techniques useful as well.
    

## Resources

### Books and Papers

  - Bray, R. M., Kerr, N. L., & Atkin, R. S. (1978). "Effects of group size, problem difficulty, and sex on group performance and member reactions." Journal of Personality and Social Psychology, 36, 1224-1240.
  - Rooksby, Hunt Wang, "Theory and Practice of randori coding dojos", 2014 http://johnrooksby.org/papers/XP2014_rooksby_dojo.pdf
  - Wilson A, "Mob programming what works and what doesn't", Helsinki 2015 (Unruly Media)
  - Hohman, M Slocum, A , "Mob Programming and the Transitiion to XP" (2001), http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.18.2967&rep=rep1&type=pdf

- Maaret and LLewellyn - mob programming guidebook - https://leanpub.com/mobprogrammingguidebook

### Timers

  - Mobster timer https://github.com/dillonkearns/mobster
  https://github.com/MobProgramming/MobTimer.python
  
### Links

  http://mobprogramming.org/
  https://agilegamesnewengland.com/index.php/mob-programming-conference
  - Mobster timer https://github.com/dillonkearns/mobster
  
### Mob RPG Game
  - Good guide to the roles and behaviours
  - Need to run it on a code kata maybe?
  - Willem Larsen https://github.com/willemlarsen/mobprogrammingrpg

  
## Closer
  - Thank you for being here
  - Hope it was useful
  - Woody is back in UK in July 2018 
  - Questions
  - Feedback forms
  
  
- Need To Work on:
  - Story around (Need to work in my unimaginative steps)
  - How to fit strong style pairing
  - Isn't it just massively inefficient Pair programming?
  - How is it different from Swarming? 
  - Rubber Ducking 
      Eliza bot 
      https://rubberduckdebugging.com/cyberduck/
      
  - Jigsaw?




keyboard is not hard work, navigators have harder work.

No standup!
resilience
Truck number
Getting things done and delivered.

Worktime flexibility
Looks weird
Management buyin

reflection !!! -> Learning

Loudest voice
Navigator


Its fun


TDD is easier
Red
Green Refactor

Simple Design
Passes All Tests
Clearn Expressive Consistent
No Duplication
Minimal

Resolving conflict - experiment groups pairs

Strong accomplished teams, start to finish on a feature
Everyone has a part of the solution. Shared pain - something is taking too long - someone can build a tool.

Protocol if you aren't learning or contributing, you can go and do somethign else

Half baked ideas aren't wasted time - beware of a single dev in a room on their own.




Just for programmers?
Testers
Increase levels of understanding



Woody father of mob. 

fundamental attribution error
- I broke the build because of reasons, you broke the build because you're a terrible person.


Llewellyn (inception of mob) - useful way to do it even if not using mob

Consideration
- Listen and put your self in their place.
- Understand where they are coming from

 
 
Visible - good for discussion and insights
Whiteboard - identify important things to park on whiteboard


Can be very tiring but also the most productive, very enjoyable

Rules
Kindness
Consideration 
Respect

Prevents name calling and derogatory remarks
Norm Kerth's retrospective prime directive - every one is doing their best for theam 
and have their own point of view.

http://www.retrospectives.com/pages/retroPrimeDirective.html

"Regardless of what we discover, we understand and truly believe that everyone did the best job they could, given what they knew at the time, their skills and abilities, the resources available, and the situation at hand." 	



Guidelines
* Have a timer
* Strong Styling
* Roles
Driver
Navigator from XP
Other Mob 
 - Overwhelming having all navigators
 - Depends on size of team
* Research
* AUtomation
Slow is obvious
Use automation to get rid of slowness in process

Regular retrospectives
How did the day go, week go




Continuous code review
Longer ability to focus
attention to detail
catching errors

Mob is not crippled by bathroom breaks or meetings or holidays


Focus

Organically there are a lot of things to think about
Code, standard, deployment, use cases, testing buisness impact, security etc.
Mob takes up different aspects of all these 
Doesn't work
One person is an expert - don't give them a keyboard - not allowed to have the keyboards
Get understanding from them

Truck number

Help everyone else get up to speed

Nobody knows what's going on
Legacy, person gone

Timebox refactoring to improve code. At the end of the 20 mins. Talk about, throw away changes 

New technology
 No body knows, needs research Timebox separation  - everyone has a different learning style
 What do we need to know to solve
   - Share what we have learned. 
   - Put puzzle parts together.
   
   
   
Cost effective?
Sage accountancy software
Cost x 4
Single person's job
Is it cost effective
Productivity and effectiveness
Can you not just type faster

Deve productivity
Knowledge work
Lines of code?
Number of hours?
BUSYNESS
Time to market
Financial Return - systems thinking
Dev
Sales
Marketing
Really hard to measure 

What impacts developer productivity? Ask audience
Meetings?
Phone calls
Project Managers?
Interruptions?
Slow decision makers
Not available
Solving the wrong problem
Too many hours
Code quality goes down
Bugs
Productivity of everyone - devs and testers
Incomplete understanding - see defects
Cruft - quality of code. Falco - on our own we get best and worst of us - graph
- retro fit practices to compensate - code review
Mob - Filters worst and get best all the time, 
Technical Debt
Investigating potential defects (not really a defect)

Mutlitasking
switch 15 minutes+ cost
Multiple switches - lose hours per day
Context switches are expensive
Mob solves 

Reduce WIP


Grunt work



Solo is faster
Major cost in production is defects and maintenance
Time spent overall is less due to improved quality

Very expensive pair programming


Ideal team size is 4 ish for complex problems
2s is level of cleverest person
3-5 can solve more complex problems than the clevest 
American Psychological society study


Pair programming
 Strong personalities vim or emacs
 Anti-pattern - heated and confrontational
 - Introverts
 - Person typing
 
 Increased flow.
 Work stops, meeting, come back, type
 Work flows because it's averaged.
 Work on the most important thing
   park other things
   
 
 Group majority
 Go where the majority wants to go
 
 
 Waiting for information
 If you are waiting there is someone missing from the mob
 


 Physical setup to get it right
 
 lareg screens
 Open space to work
 Keyboard
 Hunter pix 12 teams
 
Emodies some of the approaches used in cutting-edge education practices - training from the back of the room.


- Session will answer
- What it is
- How to use it
- Why Woody Zuill is an evil genius
- Least original person you will meet

- Pair Programming
- When I started
- What it is
- XP
- Problems
- Watching someone else
- Keyboard hogging
- Minimal Collaboration
- Skill levels
- Informal Pairing

- Dojo
- Working with junior devs
- One person at keyboard who can make progress, everyone watching.
- Deliberate Practice
- Pairs
- Randori
- Learning styles
- Most productive

- Strict Style Pairing
- Llewellyn Falco
- Turns it around
- To go into the computer, your idea has to go through someone else's fingers
- Better turn around

- Mob Programming
- Hunter Industries
- Turn up the good
- Woody Zuill

- Benefits
- Constant Code review
- Learning
- Code Styles and Standards
- Correctness
- Readability
- Dry, SOLID etc.
- Super short feedback loop
- Truck number
- Help
- Task completion
- Reduced handoffs
- Whole team ownership
- No standup


- Rules

on demand collaboration

- How to 
Pairs at pairing stations

Mob
One navigator, many drivers
Navigator dumb typist
Drivers are



Falco - Hunter Industries and Woody Zuill




http://mobprogramming.org/

Woody - Comes up with these ideas

All the brilliant people working on the same problem, at the same time, in the same space, on the same computer

Turn up the good echoing XP


Strong Style Pairing
For an idea to go from your head into the computer, it must go through someone elses hands

- Roles
- Driver
- At the keyboard
- Trust the navigator
- Make it so

- Navigator
- Verbal instructions
- No keyboard
- Talk at highest level of abstraction
 - intent
 - 
 - syntax
- Mobber

- Researcher

- Sponsor

- Learner ?


- Timing is everything
- Switch every 5 minutes, 10 minutes
- How often
- How relaxed
- Strict timer




"Nothing is more dangerous than an idea, when you have only one idea"
- Emile-Auguste Chartier
Beware of a single programmer, alone in a room

The most dangerous

Pragmatic Programmers

Timer - switch to new keyboard every 5 minutes, 10 minutes

keyboard is not hard work, navigators have harder work.

No standup!
resilience
Truck number
Getting things done and delivered.

Worktime flexibility
Looks weird
Management buyin

reflection !!! -> Learning

Loudest voice
Navigator
Mob the RPG

Mob Timer - Start Mobbing Driver, Mobber, Mobber, Navigator

Roles

Driver


Navigator


Mobber

Not solo programming with an audience
Its fun


Resourced

mob programming conference
RPG
Mobster timer github/dillonkearns/mobster

timer github.com/MobProgramming/MobTImer.python
lewellyn falco strong style pairing

TDD is easier
Red
Green Refactor

Simple Design
Passes All Tests
Clearn Expressive Consistent
No Duplication
Minimal

Resolving conflict - experiment groups pairs

Strong accomplished teams, start to finish on a feature
Everyone has a part of the solution. Shared pain - something is taking too long - someone can build a tool.

Protocol if you aren't learning or contributing, you can go and do somethign else

Half baked ideas aren't wasted time - beware of a single dev in a room on their own.


- Jigsaw

- Conclusion
- Thank you
- Resources
- ebook 
- github.com/MobProgramming/MobTImer.python
- Questions
- Feedback Forms

Changes:

Prep:



----

# alt


- What is it
- Woody Zuiil
- Hunter Industries discovered it
- All the ...

- Strong Style Pairing
- llewellyn Falco
- Driver
- Navigator

- Mob
- Extension - turned up the good
- Productivity
- Cancels dips in productivity
- Short feedback loops
- Tester
- Business Req
- Focussed
- Learning by Osmosis

- Mob Testing
- Maaret


- Agile NE
- Woody 2016

- Roles
- Driver at laptop
- Big screens
- Everyone contributes
- Navigator tells driver what to type
- Facilitator - needed ? 

- Rules
- Be Nice
- Kindness, Consideration, Respect
- For everyone
- Scary talking in front of people
- Scary coding in front of people
- Not so bad - see gurus who hunt and peck,
- can't remember API calls
- Timer
- Driver 
- Navigator -> Driver
- retrospective
- something is painful - make a tool to help!
- pain becomes obvious
- timer strictness

Small batchers (badgers)
Handoffs
Waterfall 


- Dojos

- Findings
- Hard to facilitate
- Mob not too big
- Drive with mouth shut
- Don't type your ideas (strong)
- Navigator - mediates
- Non coders
- Other approaches



- Swap every n minutes
- Break every n minutes (comfort)





Working together, not working individually and getting together to scrum

Pairing
Swarming
Mobbing


- Woody

- At hunter
- Turn up the good on working together
- What we noticed - good and wanted to try more of working together

- Rotate Roles

- Analysts
- Testers
- Devs
- Product Experts - why are we making it - part of the team at least partially

- Whole workflow, people knwo part, overlapping knowledge but not complete- handoffs


- Green field projects


- Driver
- One person typing
- Translates thoughts team is having into code that a computer can use
- Programming is code and learning and thinking about what we are doing
- Whole team thinking, learning and translating through


- Exhausting in meetings
- Mobs are not meetings
- Pay attention but not intent
- Super laser focus wears you out

- Get up, go work on something else, where can you contribute in the right way at the right time.
- Respond to current situation

- Efficient?
- Effectiveness !!!
- Not typing pool
- What destroys productivity
- Blocking Questions - queue
- Waiting for answers
 - Sitting together
 - Better to clarify rather than email or waiting for a meeting
- Working together was better for them.
- Noticed that was better.

- Waiting for Lead developer
- Context switching
- Working on serveral tasks to fill in when blocked
- Long running tasks , nothing gets finished or long running.

- Purpose Mastery Autonomy


## Teams

Design Studio method
Orchestras
Writing Music
Writers room
Sports teams

Better results working together - didnt' start out - noticed it.

Team in name only
Same manager but all working on different things
Jackson and Mei


Simple principles
- Strong pairing
- Articulate idea before part of code

Pairing some styles
 Typing person has idea. and is typing into the keyboard, not description
 Other person is reading back from screen
 Not good tranlation
  
  
## Driver

 At keyboard for a few minutes at a time
 
## Isn't this just a collosally expensive pairing

 QUality of thought is more important than quality of typing.


## De Mobbing

Break out for research
 
 
 ## Push back
 
 Management skepticism
 - At sage, if it works then continue to do it.
 

## Team Size

3, 4 or more. Larger sizes may get more chaotic, may need to delegate all information through a nominated navigator, as team size grows (like a dev meetup) then we may also need a facilitator for riot control. Opinions differ with team culture. Some find that 8 is the right size (full scrum team) and talk about 3-4 as a mini-mob. Research says 5 is a good number for problem solving.

## Fail

Fails on tedious tasks or long running tests, admin tasks. Amplification makes long tasks seem longer. Opportunity for someone to create a tool or to address it in some other way. 

## Reasons to mob

Spreading knowledge
Experimenting
Lowert knowledge
Different approaches in testing

 Learn from each other
IDE coding tips - like my alt mouse select to select a block of text horizontally and vertically

Discussion is good - don't want groupthink
Team decision
Idiomatic, wisdom of the group
Not follows a persons personality
Features takes a shorter amount of time
Diligence in creating tests, refactoring, naming

Knowledge sharing for new members. Harde to understnad object model
 Easy to pick up idioms, teach history of app
 
  SQL, C#, Javascript, Html
 Shared cognitive burden
 Work on bigger problems. 
 
 
## Productivity Blockers

Reasons for frustration
Information silos
Too many meetings
Testing or reviewing too late
Inconsistent coding
accruing technical debt
context switching
Waiting for questions to be answered


## Benefits

Continuous Code Review
Knowledge sharing
Emergent design
Debate
Consistency
Learning
Inclusivity
Truck numbers



## Equipment

  - Whiteboard or pen and paper. Issues will arise and you need to be able to park them so you can come back (David Allen - you brain is for having ideas not for storing them).
  

## Directing the Driver

Talk at the highest level of abstraction the person can understand. Concepts, programming constructs, down to syntax and punctuation if needed. Usually beginners in a language won't stay that way for long once they have seen enough people type and have practiced themselves. Talk about line numbers


# dojo

Emily Bache Randori style dojoing


## Remoting

We do some remote work with telepresence or google hangouts which just sometimes means the person remote is only ever a navigator and never a typist because of lag in the network but I have done some mobbing where we are working with Github and using the web interface to check in code directly in browser then using online build and test tools like Travis CI.


## Fail

Not everything is suitable for a mob. Repetitive tasks where you wnat to just put on headphones and crunch through it. Admin tasks. Lengthy testing tasks, is it possible to automate and have it be faster next time?  


## Watch out for

### tiredness kills
  Don't let or make one person drive too long

Avoid rabbit holes use the group to stay on track


## Going Forward

Not mandatory - it might work for you, consider it
This is how I prefer to work at work and how I run all of our coding dojos.
