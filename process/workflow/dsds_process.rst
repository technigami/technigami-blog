====================================
Process MS Access / Excel Projects
====================================

Treating MS Access / Excel projects as prototypes for larger systems,
the general workflow

Phase 1: Planning, and into a scalable, more versatile database system
=======================================================================

1.1: Collecting business requirements
--------------------------------------

Here, we establish the specific business goals associated with this transition.  This will guide us in making an informed decision that best fits your organization's needs.

If you have business processes you are running in excel, you can gain some benefit from moving to MS Access -
and you can see more incremental benefit by moving that into a web application using a more scalable database.

.. graphviz::

   digraph database_process {
      "Excel" -> "Access" -> "MS Sql Database";
      "Access" -> "Mongo DB";
      "Access" -> "MySQL";
      "Access" -> "Postgresql";
   }

1.2: Strategy for making the transition
----------------------------------------

If your organization relies heavily on MS Access or Excel, depending on your specific requirements, you may benefit most by sticking with those systems and leveraging our services to build web based views into those data - or, if we go through the needs of your organization, it may make more sense to build a seamless experience for interacting with your data through a web based interface.


Phase 2: Organizing Data, Iteration 
====================================


2.1: First iterative product
----------------------------

Based on the business goals we collected in phase 1, and your specific immediate needs,
provide a web product which satisfies one of those needs.  This should be a project that we can allocate less than 2 weeks of effort to.
Here we make a product in whatever language / framework is appropriate for a quick first pass on a product - with a full vertical cross-section, from database design through web app implementation.


.. graphviz::

   digraph iterative_process {
      "Choose or Update Database" -> "Choose Business Goal" -> "Outline requrements" -> "Identify success criteria" -> "Implement limited scope web app";
      "Implement limited scope web app" -> "Choose Business Goal";
      "Identify success criteria" -> "Prototype in Excel / Access"  -> "Choose or Update Database"; 
   }
   

2.2: Ongoing work
------------------

We like to think of ourselves as your outsourced "web / dev department down the hall".  A software product is never finished - there are always more things you can add, always more features that could benefit your company, and always maintenance.  We highly recommend keeping a team around on retainer to keep the system running smoothly and providing the most, tangible benefit to your business.  Based on how our first iterative product went, we can build a schedule and pricing model that fits your business needs, and promises some direct measurable benefit to how you do business.

