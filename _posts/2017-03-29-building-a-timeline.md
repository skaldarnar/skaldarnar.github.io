---
layout: post
title: Building a Solid Timeline for Your Project
categories:
- blog
tags:
- gsoc
---

This is another post in the series on Google Summer of Code. I'm trying to give you an impression of the 
 [mentor's perspective][mentors perspective] and what we are looking for during that time. By now, you 
 should be writing your [convincing proposal], and this post should help you to build a solid timeline
 for your summer project.
 
---

We are right in the application period of Google Summer of Code now, so if you are eager to get a spot on
the summer project you should have started on a draft proposal already. An essential part of your proposal is
the **timeline**. First of all, it describes in detail what you are going to do. Second, it shows how familiar
you already are with the code base. Third, it is an estimation and self-assessment. The following notes might
help you with building a solid timeline for your project.

In general, we expect a precise notion of _what you are going to deliver_ and _what is a nice-to-have_. This groups your
goals into **main goals** and **stretch-goals**. This may sound familiar to KickStarter campaigns where often additional
stretch goals are enabled once a specific amount (on top of the original target) is reached.

Dividing your work period into subtasks allows you to identify bottlenecks, critical paths, and dependencies between
them. We usually find a scope of **one week* per task reasonable. You have started with a high-level overview, e.g.,
first phase, second phase, and third phase. Try to break it down to one-week tasks (maybe even 2-3 days), and avoid 
generic, unspecified sub tasks. If you cannot clearly describe and explain the outcome of a task try to work on it 
with mentors.

In the end, this gives you flexibility in defining your overall project scope by shifting tasks from main to stretch and
vice versa. If it feels your (main) task is too short, add more stretch goals. If it feels your (main) task is too long, 
move subtask(s) to the stretch goals. Keep an eye out on dependencies here - don't block yourself!

The estimations are no hard deadlines, but rather a guideline. Organizations will hand out project _ideas_ which means
that sometimes they can be too complex (or too easy) to be done by a single person. Your timeline should identify such
problems so that you can define a better scope together with mentors.
Estimate what it takes *you* to complete the tasks, and include time for learning, research, etc. If you are not sure 
about some detail, ask a (potential) mentor for guidance. 

Finally, let's have a quick look at two different formats. We don't tell you to use a specific format, but I want to 
give two examples and point out why those met our expectations last year.

### Detailed Timeline

Rostyslav Zatserkovnyi, one of our students from last year, decided on using a _detailed timeline_. A timeline entry 
describes a sub task which is estimated to approximately one week of work. Sometimes it can be more depending on how
easily a task can be broken up or whether it forms a logical unit that has to be implemented together.

The entry caption gives an overview of what is going to happen that week. In other formats, this corresponds
to the bullet point or note describing a task. In the body of the entry Rostyslav gives more detailed information
on what is required for the implementation to be considered done. Adding images and diagrams can help clarifiy the 
desired results.

Finally, he gives an estimation of the task's work.
You can find his proposal [here][rzats].

> ##### JSON to tree view adapter
>
> A custom deserializer designed to work with the UITreeView component developed in the previous phase of the project 
> will be developed. This utility class will generate a TreeView based on a JSON file, with value types represented as 
> leaf nodes and arrays/objects as separate branches tracking and visually representing the number of their child items. 
> A similar serializer method will reconstruct the JSON file based on a TreeView by iterating through the root TreeItem.
>
> Since a JSON deserializer can be used for other purposes within Terasology (e.g. Shape or Prefab editors), this 
> adapter will also become a core NUI utility class.
>
>  ![Adapter Usage Example]({{ site.baseurl }}{% link assets/2017-03-29-building-a-timeline/image_1.png %})
>  Figure 2: Adapter usage example (data source: Wikipedia)
>  
>  To save horizontal space, the first value of an array member object is displayed as the branch name and one-item 
> arrays are represented as objects (i.e. do not expand into a separate tree branch containing one object).
>  
> _Approximate implementation time: 1 week (June 6th - June 11th)._

### Tabular Timeline

We were presented with a _tabular timeline_ by Taha Doğan Güneş. He outlined his goals and continued with the timeline,
following a plan to achieve the goals. The work period was strictly divided in one-week sub tasks, and for each task
a short description in form of a bullet point list was given. 
In contrast to Rostyslav's detailed timeline, all technical details and ideas on the implementation were given in a 
separate section.

You can find Taha's proposal [here][tdgunes].

---

These two timeline formats are just examples of how different this piece of your proposal might look like. I wanted
to convey a general idea of a timeline's level of detail, both to help you understand the project and estimate
the effort, and to enable us to give better feedback and help you fix the hard edges of your document.

[tdgunes]: http://forum.terasology.org/attachments/tdgunesgsoc2016-pdf.2326/
[rzats]: https://github.com/saketkc/fos-proposals/blob/master/GSoC-2016/Accepted/MovingBlocks-rzats-Visual-NUI-Editor/MovingBlocks-rzats-Visual-NUI-Editor.md
[convincing proposal]: {{ site.baseurl }}{% link _posts/2017-03-23-convincing-proposal.md %}
[mentors perspective]: {{ site.baseurl }}{% link _posts/2017-03-10-mentors-perspective-on-gsoc.md %}