---
layout: essay
type: essay
title: "A Developers Guide to Design Patterns"
# All dates must be YYYY-MM-DD format!
date: 2025-12-03
published: true
labels:
  - Software Engineering
  - Design Patterns
---

<img width="200px" class="rounded float-start pe-4" src="../img/designpatterns.jpg">


## Seeing Code as a System, Not Just Lines

One of the biggest shifts in my thinking this semester came from learning to see code as something more structural than individual functions or components. Building the WODs in React and Next.js, and especially working on RoomMatch UHM, made me realize that healthy codebases have internal logic, rhythms, and repeated structures. Certain solutions kept appearing such as similar shapes or similar flows and they brought order to what could have otherwise become unpredictable and messy.
Later, with a little more research, I learned these recognizable structures are called design patterns. Although I went through most of the semester not being able to name them, I realized I was already using them. They emerged because they simply made the code cleaner, easier to reason about, and resilient to change. In that sense, design patterns are less about memorizing technical labels and more about learning to architect code intentionally.
Patterns That Emerged in the WODs

Working through the React practice WODs, I noticed that the way components “listen” to changes in state always follows the same structure. A piece of state updates in one place, and the rest of the UI adjusts automatically. I did not know the official terminology at the time, but I understood that this pattern prevented me from manually passing information around to every component. It created a natural, predictable chain of communication.
I also encountered another recurring structure when dealing with database connections. In RoomMatch UHM, Prisma kept creating multiple connections whenever Next.js was reloaded. The recommended fix, to make sure the connection was created only once and reused everywhere, was not presented as a theoretical pattern, but it solved the problem efficiently. Later I realized this approach aligns with a well-known design structure used across countless frameworks and applications.
Even small WODs taught recurring ideas. When we separated data, UI, and behavior in exercises like Bowfolios or Digits, the organization felt familiar across projects. I did not think of it as a “pattern,” just a way to make the application understandable. But in reality, I was following a pattern that many developers rely on to keep logic, rendering, and data concerns from collapsing into one file.
These experiences helped me see that patterns are not invented, but discovered through practice. They are the natural by-product of trying to build code that behaves consistently across different features and assignments.

## RoomMatch UHM: Where Patterns Became Practical

RoomMatch UHM was where these structural ideas became more essential rather than optional. The moment multiple components, database operations, and UI interactions started overlapping, the project required careful organization. I noticed that reusing certain structures was not just convenient, but necessary to keep the application readable.
For example, using a centralized form-handling function instead of writing the same validation logic in three different components was a structural choice that followed the same design solutions I had used in earlier WODs. So did organizing code into “models,” “pages,” and “components,” which naturally separated responsibilities. These techniques made the project feel manageable, even as it grew.
Through RoomMatch, I recognized that design patterns are what allow a project to scale without collapsing under its own weight. They make your code behave like a well-run system instead of a series of disconnected tasks.

## Why Interviewers Ask This Question

I believe when interviewers ask, “What are design patterns?” they are not really checking whether you can recite a textbook definition. What they want to know is whether you design systems intentionally or whether you simply write code that works once and hope it holds up later.
After this class, I imagine a developer familiar with patterns can anticipate how code will behave in the future, build features that integrate smoothly with the rest of the system, and solve problems efficiently without having to reinvent a new solution.
My own experience in ICS 314 reflects this. I did not begin the semester thinking about architecture, but I ended up designing code in a way that mirrored well-established patterns because the scale of the projects made them necessary. Learning to recognize these structures gives me confidence that I can speak about them in interviews, not as memorized theory, but as lived experience.

## Conclusion

Design patterns have helped me understand that good code is never an accident. Whether in practice WODs, React exercises, or RoomMatch UHM, the most reliable solutions emerge from structures that many developers before me had already discovered. Even before I had the vocabulary for them, I was learning to use patterns that made my code logical, maintainable, and adaptable. Therefore, design patterns are not about memorizing names, but about learning to see the architecture beneath the surface of the code. 
