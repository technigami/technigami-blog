=============================
A process for agile planning
=============================
There are many ways of planning a large software development project, and many ways of planning agile software development.
Outlining one formula for agile development is almost a misnomer - since the principle of agile development is that its flexible and every project / every group / organization will have different needs and different styles of communication.  This is one approach of many, and there is no one "correct" approach.

In this process, there are a few preliminary steps involving research before we get into the core cycle:

1. Research: Gather all of the resources you can on the subject, interview stakeholders to identify topics of research - but keep the research relatively short.  You don't want to go too far without checking in with the stakeholders, you want to stay grounded to some common agreed on reality.

2. Identify Business Objectives: Interview stakeholders and identify why the website exists, what business purposes it serves

3. Identify Audience: Use a combination of interviews, review of analytics, google trends, other analytics, including quantcast analytics, and some general insight into the type of business to outline who the the main users of the site or software product will be.

4. Prioritize Audience: Go through the list of audience, look at your business objectives, and talk about what business objectives are best served by each segment of audience.  Once you have prioritized your business objectives, you can prioritize your audience.  This task might be simplified for larger audience lists to filter the list into "High", "Medium", and "Low" priority groups.

5. Prioritize business objectives

6. Come up with a rough list of calls to action, and *measurable* success criteria.

And then we enter into the cycle of refining the user objectives,
and continue to clarify the product features and acceptance criteria.

Agile development techniques often refer to the idea of a "user story".  This is what is known in sociology as a "boundary object" - it is a powerful concept which helps bridge language gaps between people of different backgrounds, languages, or disciplines.  There isn't really much of a standard formal definition of a user story - it should be from the perspective of a user of the system, and should be short enough to fit on an index card.  They will be the subject of discussion / revision.

"Boundary objects are said to allow coordination without consensus as they can allow an actor's local understanding to be reframed in the context of a some wider collective activity" [1]_.


.. graphviz::

   digraph user_stories {
      "Interview / Survey" -> "Identify Business Objectives";
      "Identify Business Objectives" -> "Identify User Objectives" ->"Generate user stories";
      "Generate user stories" -> "Simplify user stories" -> "Build Use Cases"-> "Identify acceptance criteria";
      "Generate user stories" -> "Identify acceptance criteria";
      "Identify acceptance criteria" -> "Interview / Survey";
      "Generate user stories" -> "Build Context Diagram";
      "Build Context Diagram" -> "Identify acceptance criteria";

   }

Discussion around user stories is key to making them useful.  Its easy for the process to get out of hand.  One tool that is useful in organizing the discussion is the context diagram [4]_.  Its important if the developers are involved in building the user stories that the user stories not include development details.  Stories need to really reflect how users are using the system.

The output of the discussion on user stories can be formalized into Use Cases, to go further into a functional specification of software you can write a Use Case.  The output of the discussion can also go directly into building some wireframes, depending on the scale / scope of the project.  Use cases are useful in much larger projects, and can be useful for partial coverage of the more important features of a smaller project.  

There are some standard semantics for writing use cases - and they are used across the board in the discipline of Business Process Management [3]_ (as far as I can tell).  Depending on the requirements for the project and / or time constraints, you can often take Use Case documents and directly turn them into tests, and developer the software product using the Behavior Driven Development (BDD) technique.  There are a number of BDD frameworks out there.  PHP has Behat, Ruby has Cucumber, Python has Lettuce, and javascript has a few.  Jasmine is one I have worked with some.  BDD offers some great benefits, but there is a learning curve, and it can be hard to move a team not already used to using BDD techniques in the direction of either Test Driven, or Behavior Driven development.  There is certainly an argument for software built without tests, using regression testing - build it pretty well, and test what breaks when it breaks to make sure that it doesn't happen again. 

One process for moving forward from a list of user stories

1. Refine and map / group user stories 
2. Extract high level features
3. Build use cases.
4. Identify acceptance criteria
5. Revisit calls to action
6. Interview

.. graphviz::

  digraph wireframes {
    "Prioritize Calls to Action" -> "Refine Use Cases" -> "Build General Layout";
    "Build General Layout" -> "Build Storyboard";
    "Build Storyboard" -> "Build mockups of required design elements" -> "Interview / Feedback" -> "Prioritize Calls to Action";
    "Build Storyboard" -> "Generate User Stories" -> "Refine User Stories" -> "Refine Use Cases";
  }

Once we have refined a set of user stories and their acceptance criteria,
and gain a more complete understanding of how users will use the system,
we enter the design cycle involving iterating on user stories to form wireframe documents.
These wireframes can be thought of as similar to storyboards.  They serve to act as functional prototypes of how users will interact with the system, based on their user stories.  


A case for agile methods
-------------------------
Communication poses one of the largest challenges in most software projects, and can often indirectly or directly contribute to a project being late or over budget.  Agile methods are built to make sure that when you're working on the software, its the thing that was asked for, and to make sure that as a product owner or consumer, you can have software that is flexible / can adapt to a rapidly changing landscape of technology, requirements, and business needs. 


   
References
----------
.. [1] Bechky, B. A (2003). "Sharing meaning across occupational communities: The transformation of understanding on a production floor.". Organization Science 14 (3): 312–330..
.. [2] http://www.mountaingoatsoftware.com/topics/user-stories
.. [3] http://en.wikipedia.org/wiki/Business_process_management
.. [4] http://www.industriallogic.com/blog/as-a-developer-is-not-a-user-story/
.. [5] http://www.agilemodeling.com/artifacts/userStory.htm
.. [6] http://blog.extremeplanner.com/2006/01/writing-good-user-stories.html
.. [7] http://www.allaboutagile.com/writing-good-user-stories/
.. [8] http://dannorth.net/whats-in-a-story/
.. [9] http://www.scrumalliance.org/articles/169-new-to-user-stories
 
 

