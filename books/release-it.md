# Release it!
> Design and deploy production ready software

*by Michael T. Nygard*

## Chapter 1: Living in Production
---
Does “feature complete” mean “production ready”? 

Software spends more time in production than in development.
  
## Aiming for the Right Target
Most software is designed for the development lab or the testers in the QA department.
  
When our system passes QA, can we say with confidence that it’s ready for production?
  
**Design For Production:** Design softwre to operate at low cost and high quality.

## The Scope of the Challenge

Building software fast that’s cheap to build, good for users, and cheap to operate demands continually improving architecture and design techniques.
  
## A Million Dollars Here, a Million Dollars There
Beware of systems which exhibit low availability, direct losses in missed revenue, and indirect losses through damage to the brand.
  
Make decisions that optimize development cost at the expense of operational cost only makes sense in the context of the team aiming for a **fixed budget and delivery date** (consultory?).
  
Design and architecture decisions are also financial decisions (implementation cost as well as their downstream costs).
  
 ## Use the Force
The earliest decisions you make can be the hardest ones to reverse later. The beginning is when your team is most ignorant of the eventual structure of the software, yet that’s when some of the most irrevocable decisions must be made

**Early delivery and incremental improvements** means software gets into production quickly.

## Pragmatic Architecture
Architect shall not just rub shoulders with the coders but be one.

Question all. “How can we do a deployment without rebooting the world?” “What metrics do we need to collect, and how will we analyze them?” “What part of the system needs improvement the most?”

---
### Part 1: Create Stability
---

## Case Study: 
## The Exception That Grounded an Airline

Have you ever noticed that the incidents that blow up into the biggest issues start with something very small? A tiny programming error starts the snowball rolling downhill.

## The Change Window

Planned downtime to perform critical operations on the system. Team was trained and applied this change several times before this one. When concluded, change looked succesful.

## The Outage
Suddenly the system broke. 

Restoring service takes precedence over investigation. When the fur flies, improvisation is not your friend

The trick to restoring service is figuring out what to target. You can always “reboot the world” by restarting every single server, layer by layer. That’s almost always effective, but it takes a long time. 

## Consequences
You know it’s going to be a bad day when you see the CEO stalking around the operations center to find out who cost him his vacation home in St. Thomas.

## Postmortem
"You touched it last” turns out to be a good starting point most of the time.

- Did the last action cause the outage? If not, what did?
- Was the system configured correctly?
- Did the team conduct the actions correctly?
- How could the failure have been detected before it became an outage?
- Most importantly, how do we make sure this never, ever happens again?
  
Managing perception after a major incident can be as important as managing the incident itself

## Hunting for Clues
Stack-traces can be very helpful.

## The Smoking Gun
Relations can get strained due to the fear of blame. 

## An Ounce of Prevention?
Ultimately, it’s just fantasy to expect every single bug to be driven out. Bugs will happen. They cannot be eliminated, so they must be survived instead.

The worst problem here is that the bug in one system could propagate to all the other affected systems. **“How do we prevent bugs in one system from affecting everything else?”**
