---
layout: product-work
case-study: Simplifying the Complex
description: Making sense of complex system interactions to implement improvements critical to user needs
permalink: /pm/simplifying-the-complex
---

<h3 class="first-h3">The Problem</h3>
Without user research and more thorough user need assessments prior to any product development, the product was developed with what we learned to be quite restrictive abilities around appointment scheduling. Editing all fields on an appointment, or job, form regardless of the point within the job's lifecycle was not possible with the release of the product and quickly became a highly desired improvement from our full agency user base. 

For example, if an agency scheduler created an appointment for 10:30 am on Tuesday the 11th, but later learned that the time needed to be moved to 10 am, the only option was to cancel the original appointment and create a new one.

An understandably common occurrence in practice held heavy system implications, however, because of the original architecture of the product catered towards less flexible needs. In our example, if an interpreter had already been assigned to work the job and the time changed, we would first need to ensure the new time didn't conflict with any existing appointments on the interpreter's schedule before determining that they were available with the updated appointment details. 

<span class="emphasis">With the feature to edit all appointment fields at any point during it's lifecycle in queue for development on our product roadmap, I had to determine just how we could make this possible and account for the more complex scenarios and implications to editing any 30+ fields in any one of the 8 possible appointment statuses.</span>

<h3 class="second-h3">The Details</h3>

<h5>The Application</h5>
<a href="/work/what-is-vineya" target="blank">Vineya</a> for Agencies, Vineya for Businesses, and Vineya for Interpreters 

<h5>The Users & Audience</h5>
A direct impact to the appointment creators, approximately 90% of all Vineya for Agencies and Businesses users, and an in indirect impact to ASL interpreters

<h5>The Team & Role</h5>
As the Technical Product Manager, it was my responsibility to outline the specific feature requirements, functionality, and user flows in a clear, concise, and digestible format for sales, design, and development roles to reference and direct their responsibilities around the feature.

<h5>The Tools & Methods</h5>
Jira, Whiteboard, Excel, Sketch, Information Architecture, Complex System Evaluations

<h3 class="third-h3">The Approach</h3>
##### Step 1: Understanding the Starting Point
My first goal was to get a full picture of where we currently stood versus where we wanted to go. To do so, I outlined all of the fields on an appointment against all of the appointment statuses and indicated whether it was:
1. Currently editable in each status
2. Desired to be editable in each status

<p>
    <img class="img-shadow" alt="Edit Jobs - Current vs. Desired" src="/images/work/pm/simplify_complex/edit_job_current_desired.png">
</p>

##### Step 2: Defining the Possibilities
I then needed to ensure I clearly outlined all of the possibilities for both job fields and job statuses. 

For job fields, I sorted each into one of four categories:
1. <span class="bold">Never Edit</span> - any field that could not be edited (i.e. job ids, system control job statuses, etc.)
2. <span class="bold">No Impact</span> - any field that could be edited in any job status without impacting other fields through the job life cycle (i.e. reference code)
3. <span class="bold">Small Impact</span> - any field that did have a small impact on another field or system process when edited in the job life cycle (i.e. consumer email impacting consumer email notifications)
4. <span class="bold">Complex Impact</span> - any job field that did have a complex impact on another field or system process when edited in the job life cycle (i.e. editing the date could impact interpreter's and their availability to attend the meeting) 

<p>
    <img class="img-shadow" alt="Edit Jobs Field Impacts" src="/images/work/pm/simplify_complex/edit_jobs_fields_impact.png">
</p>

For job statuses, I outlined first the "happy path" for a job's life cycle, and then added the additional process possibilities based on various user actions and selections.

<p>
    <img class="img-shadow" alt="Job Status Transitions" src="/images/work/pm/simplify_complex/job_status_transitions.png">
</p>

After defining the possibilities, it became much more clear where the majority of the challenges would lie: any field that had a complex impact if edited could directly impact interpreter selections and appointment cost estimations. 

##### Step 3: Brainstorming the Challenges
Focusing my evaluations on the complex fields, I drilled further down into outlining what could occur if a field was edited in each different status in a past and/or future timeframe.

Taking interpreter selections, or interpreter scheduling, as an example, below you can see some initial brainstorming around how I started to process the impacts. I identified two key questions that needed to be asked for each complex field and each status in both past and future timeframes:

1. What happens to existing interpreter selections (or already invited or scheduled interpreters)?
2. Is there a status change? 

<p>
    <img class="img-shadow-dark" alt="Brainstorming Complex Fields" src="/images/work/pm/simplify_complex/brainstorm_complex_fields.jpg">
</p>

##### Step 4: Simplifying the Complexities
Finally, I started to identify patterns and themes that guided me in outlining answers to my two key questions. Below you can see how I visually represented the results of those patterns and themes to help guide others also trying to understand the complex impacts of potential user edits.

<p>
    <img class="img-shadow" alt="Complex Fields Evaluations while Selecting Inteprreters" src="/images/work/pm/simplify_complex/interpreter_selections_complex_fields.png">
</p>


<h3 class="first-h3">The Solution</h3>
Breaking down the overwhelming task into key pieces truly helped me better process and identify the true challenges.

Once I had identified the zero impact and simple fields and edits, I was able to focus on the then much smaller picture of the more challenging field edits.

Through the use of the documentation and visuals that I created while processing the problem, I was more efficiently able to outline and define the system requirements for the feature and provide visual alternatives to anyone else processing the complex needs.

That's not to say this was then a piece of cake to subsequently design and develop, but it did ease the process for all parties involved. 

<h3 class="second-h3">The Learnings</h3>
##### Break down the problem into digestible pieces
What at first seemed almost too daunting to achieve quickly became an understandable  challenge by breaking down the current system fields and processes into smaller groups. Then, approaching the problem by the smaller groups allowed me to effectively evaluate the various needs and impact of the initially overwhelming goal. 
    
##### Pinpoint similarities, differences, and themes
Identifying the links and disconnects between possible scenarios enabled me to establish logical groupings and more adequately and concisely outline the required system functions in response to user actions, an applicable learning to many other areas of product work, including design and user research.

##### No challenge is too complex
A touch of a clichéd motivational learning, yes, but nevertheless still true. When I approach a complex problem, I typically have equal parts of fear and excitement. Knowing that there is always a valid and possible solution to achieve through hard work and collaboration, the excitement drives me through the fear and makes the formidable problems my favorite ones to handle. 

<p class="italic small-note">Have any thoughts, ideas, feedback? I love to discuss my work, so <a href="mailto:casiemattrisch@gmail.com">let me know</a>!</p>

<div class="resume">
  <button class="back">
      <a href="/pm/">Back to PM Work</a>
  </button>
</div>