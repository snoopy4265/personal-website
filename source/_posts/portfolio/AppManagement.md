---
title: Redesign Sauce Labs App Management
date: 2023-06-20 08:26:28
password: michellewu2023
categories: portfolio
tags:
  - portfolio
cover_image: /images/AppManagementCover.png
---
<h5 class="mb-0 text-center">During my time working in Sauce, I am involved in revamping the entire app management experience to solve customer problems and enable future scalability through integration of various functionalities across our product offerings.</h5>
<p class="text-muted text-center">Redesign Sauce Labs App Management | Year: 2023</p>

</br>

### Problems
There are several reasons for the redesign of app management. The primary reason is driven by customer feedback. We heard from customers that they were having **difficulties organising and managing their app builds** mainly because of our limited app management structure. With current app management, all the app builds that customers uploaded for testing are placed in one central location with only flat file structure. **<mark>This causes trouble for users managing apps for different environments and different testing purposes.</mark>**

</br>
<img src="https://www.dropbox.com/s/g1l1qq6rashe7ld/AppManagementProblem.png?raw=1" width="100%" height="auto"/>
</br>

Other reasons for the redesign include **considerations for future scalability** and **alignment with the long-term product vision** of creating a unified and user-friendly central app dashboard that integrates various functionalities from our product offerings. 
All in all, redesigning app management will serve as an important initial step in accommodating these developments.

</br>

### Goal & Focus
> Design a user-friendly and scalable app management system that aligns with the user's mental model, facilitating effortless organisation of their applications and quick retrieval for testing.
<div class="row mb-3">
  <div class="col-6 col-md-6">
    <strong><i class="fas fa-user-friends"></i> The Team</strong>
    1x Product Designer (Me)
    1x Senior Product Designer
    1x Product Manager
  </div>
  <div class="col-6 col-md-3">
    <strong><i class="fas fa-tasks"></i> Key Contribution</strong>
    User Research
    Journey Mapping
    Insights Synthesis
  </div>
  <div class="col-6 col-md-3">
    <strong> </strong>
    Concept Testing
    Mockups Design
    Prototype Testing
  </div>
  <div class="col-12 col-md-12">
    <strong><i class="fas fa-project-diagram"></i> Design Process</strong>
    <img src="https://www.dropbox.com/s/buu4dmiip6hqfbr/DesignProcess.png?raw=1" width="100%" height="auto"/>
  </div>
</div>

</br>
</br>

### Inspiration - Research & Synthesise

Research is king, especially as a newcomer to the workforce and touching on a new field, research becomes even more important. Fortunately, before I even started working here, many other product designers had designed, researched, and envisioned early concept of app management. There were also personas targeting different user groups of Sauce Labs as well as their journeys for me to look through. 

So I mainly started from collecting information from our existing knowlege base. Try to understand who are our users, what are their needs and pain points, what have been done so far and what do we envision.


<div class="row justify-content-center align-items-center mb-5">
  <div class="col-12 col-md-12">
    <strong>Inspiration</strong>
    <h3 class="text-left mb-0"><mark>User Persona</mark></h3>
    While we recognize that Sauce Labs serves many types of users, by cross-referencing Weekly Active User(WAU) of app management with user personas, it makes sense to focus primarily on these 2 personas:
    1. **Uploader/Maintainer**: Someone who is responsible to upload/maintain apps to Sauce Labs, mainly are mobile developers. 
    2. **Internal Tester**: Someone who is responsible for testing, could be QAs or developers.
    We also found out that users work in big corporations tend to report problems to us. Because they have a need of organising numerous apps and retrieve the right version to do quality check.
  </div>
</div>

<div class="row justify-content-center align-items-center">
  <div class="col-12 col-md-6">
    <strong>Inspiration</strong>
    <h3 class="text-left mb-0"><mark>User Journey Mapping</mark></h3>
    After identifying the target users for the project, I worked with PM to map out the user journey. During this process, the PM, who has a background in app developing, explained to me the mobile development cycle and how our product intersects with various stages. 
    **This really helped me to understand the needs and pain points of users when interacting with our product.**
  </div>
  <div class="col-12 col-md-6 pt-md-5">
    <img src="https://www.dropbox.com/s/k0yp1w5j8rmlfhw/AppManagementJourneyPhoto.jpg?raw=1" width="100%" height="auto"/>
    <img src="https://www.dropbox.com/s/n8m41cib0zjgjmk/AppManagementJourneyMap.jpg?raw=1" width="100%" height="auto"/>
  </div>
</div>
From here, I learned that users need to:
- Have a **grouping mechanism** to organise their app builds in a way that others can more easily to retrieve.
- Find the **latest** build through an **unique value**. That value could be file name, version/build, or JiRA number..etc, up to users' own preferences.


<div class="row justify-content-center align-items-center mb-5">
  <div class="col-12 col-md-12">
    <strong>Inspiration</strong>
    <h3 class="text-left mb-0"><mark>Competitor Analysis</mark></h3>
    To gain more inspiration, I also conducted a round of competitor analysis in an attempt to understand how app management is currently handled by us (Sauce Core and Test Fairy) and the competitors (Google's Firebase and Microsoft's App Center). Evaluate the strength and weakness of different ways of handling. Pinpoint the outlier and close the knowledge gap. 
    <img src="https://www.dropbox.com/s/l6da275km8ppshk/AppManagementDeskResearch.jpg?raw=1" class="my-5" width="100%" height="auto"/>
    This series of preliminary investigations gave us insights to initial questions such as:
    **1. How do users organize their apps on these platforms? What kind of grouping mechanism they use?**
    **2. Why do users need to organize their apps?**
    **3. How many levels have users created to manage their apps?**
  </div>
</div>

</br>
<hr/>
</br>

### Ideation - Ideate & Prototype

Based on the information collected from inspiration phase, I started to have some ideas for possible information architectures. So I shifted gears to focus my energy on ideating all of the possible solutions for new app management.

<div class="row justify-content-center align-items-center mb-5">
  <div class="col-12 col-md-12">
    <strong>Ideation</strong>
    <h3 class="text-left mb-0"><mark>Data Model/Concept Ideation</mark></h3>
    I created **4 different concepts** and wrote down each of the limitations and benefits. I also projected what the interface would look like with future features to ensure that the concept would scale to our product vision. 
    <img src="https://www.dropbox.com/s/vmbswft1dt9impb/AppManagementDiagram.png?raw=1" class="my-5" width="100%" height="auto"/>
    <img src="https://www.dropbox.com/s/5cdrbqzm3hcfavs/AppManagementConcept.png?raw=1" class="mb-5" width="100%" height="auto"/>
    After multiple rounds of iterations and discussion with PM, other designers and stakeholders, we landed on a final concept with these features: 
    **1. Introduce a new hierarchy model incoporating an extra layer called "project" on top of apps to provide a flexible grouping mechanism.**
    **2. Enable users to tag on app builds to provide extra unique values to identify.**
    **3. Show "recently tested" section to assist user workflow.**
  </div>
</div>

<div class="row justify-content-center align-items-center mb-5">
  <div class="col-12 col-md-12">
    <strong>Ideation</strong>
    <h3 class="text-left mb-0"><mark>Concept Testing</mark></h3>
    To validate this concept, we conducted internal concept testing by interviewing **5 key customer-facing employees** within our organization, such as technical account managers, customer support engineers, and solution engineers. As individuals who regularly interact with customers, they possess a deep understanding of user complaints and pain points. We presented them with the new concept design prototype and gathered their feedback. 
    <img src="https://www.dropbox.com/s/hncvnhqfg6nbahh/AppManagementConceptTesting.png?raw=1" class="my-5" width="100%" height="auto"/>
    At first, we were slightly worried that users can't understand the new hierarchy. But from the testing, **we got relatively positive feedback about the new structure.** <mark>It was a relief for us because we ensured that we are heading in the right direction and that people can understand the new hierarchy model we proposed, which is our original goal: introduce an app management system that aligns with the user’s mental model.</mark>
    Other than that, our internal testers also suggested a number of improvements to the new design, which were carefully collated and prioritized for design modification.
  </div>
</div>

</br>
<hr/>
</br>

### Implementation - Build & Measure

You will never know precisely until you build it and put your idea out there to the world for your users to use and continuously measure and learn. Especially, we are building a platform serving multiple user types with numerous different behaviours and preferences. 

At this stage of the design process, we aim to build the high fidelity design and push it to a subset of external users to gather insights on usability and to uncover any hidden issues in the workflow before handing over to the development.

<div class="row justify-content-center align-items-center mb-5">
  <div class="col-12 col-md-12">
    <strong>Implementation</strong>
    <h3 class="text-left mb-0"><mark>Hi-fi Design Prototype</mark></h3>
    After finalizing the design direction and information architecture, I proceeded to flesh out interfaces and user flows. At this stage, I designed more high fidelity prototypes, incorporating our company's design system while also utilizing data that closely resembles real-world scenarios. This included simulating actual app data, version numbers, and possible categorization methods within the interface. The itention was to facilitate easier comprehension and foster discussions among team members, enabling them to identify any potential logical gaps or flaws within the design.
    <img src="https://www.dropbox.com/s/mzj7a0eod4z8hgg/AppManagementDesign.png?raw=1" class="my-5" width="100%" height="auto"/>
  </div>
</div>

<div class="row justify-content-center align-items-center mb-5">
  <div class="col-12 col-md-6">
    <strong>Implementation</strong>
    <h3 class="text-left mb-0"><mark>Task Analysis</mark></h3>
    To test our design out there, we decided to run an **unmoderated clickable prototype testing** by using **[Maze](https://maze.co/)** as a testing tool and **[Pendo](https://go.pendo.io/demo-pendo-products-hv-z.html?cq_plac=&cq_net=g&cq_pos=&cq_med=&cq_plt=gp&cq_cmp=9965755808&gad=1)** as a recruitment method.
    We asked users to go through a clickable prototype with 4 tasks and report if they believe they completed each task, how hard they would rate them, and their thoughts around the way. 
    We wanted to mainly validate:
    **1. If the users can easily navigate to the specific version of the specific app.**
    **2. If the workflow for uploading the apps into project was clear and intuitive to our users**
  </div>
  <div class="col-12 col-md-6 pt-md-5">
    <img src="https://www.dropbox.com/s/3wcqg2exhl4u6oq/AppManagementRecruit.png?raw=1" class="my-5" width="100%" height="auto"/>
  </div>
</div>

In the end, we were able to gather 21 responses + 6 responses from the internal pilot run, which gave us 27 data points to analyse. 

<img src="https://www.dropbox.com/s/kbz9i3dl6i2h8oz/AppManagementPrototypeTesting.png?raw=1" width="100%" height="auto"/>

This fine-grained method of testing enabled us to pinpoint areas of the design that were successful and areas that needed further iteration. We then took those learnings and made even more improvements to the final design.

</br>
<hr/>
</br>

### Conclusion - Retrospective & Key Learnings

It is not easy to redesign a software service that already has many users. When users have already developed a habitual mental model for your product, it takes a lot of effort to introduce a new mental model and make it easy for users to learn without rebounding. Extensive research and discovery at the beginning is important, but I think what also important is through a continuous process of think, build and learn to see what is working with users, what isn’t, and what improvements can be done to the solution over time.

I am grateful for the trust from the team to let me who just onboarded for no more than a month, take on the responsibility of designing this project and give me timely help during the process. According to our product vision, we will add app distribution and error reporting functions to this project in the future. There are still lots of potential and improvement for this and the impacts are expected to be significant as well.

</br>

