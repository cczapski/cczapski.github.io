---
layout: product-work
case-study: Designing for Unintentional Errors
description: Removing unintentional system errors and improving user interactions with contextual feedback
permalink: /uxui/designing-for-unintentional-errors
---

<h3 class="first-h3">The Problem</h3>

In an effort to allow users to create appointments without adding in a new "End Date" field (of which was deemed too complex of a back end solution at the time), a Front End developer chose to quickly solve the need by allowing the user to select an "Ends Next Day" checkbox below the Start Date, Start Time and End Time inputs to indicate and confirm that an appointment would span two days.

<p>
    <img alt="Original Date/Time Picker" src="/images/work/vineya/preventing-user-error/original_date_time_picker.png">
</p>

A fair quick fix in theory was proving to cause many issues in practice: when a user would select an end time the same or earlier than the start time, the "Ends Next Day" checkbox would automatically check. Users were unintentionally creating appointments 24+ hours in duration.

The volume of reported user instances, the lack of a user's ability to edit the inputs themselves, and the critical appointment details impacted with this issue quickly moved this problem to the top of my improvement priority list. 

<h3 class="second-h3">The Details</h3>

<h5>The Application</h5>
Vineya for Agencies and Vineya for Businesses web applications

<a href="/work/vineya/what-is-vineya" target="blank">What is Vineya?</a>

<h5>The Users & Audience</h5>
Appointment creators, approximately 80% of all Vineya for Agencies and Businesses users, and the primary business target market for revenue generation

<h5>The Team & Role</h5>
After identification of the problem from the Customer Service team and evaluations with the Quality Assurance team to uncover the root issue, I was responsible to design an improvement that would prevent the unintended errors when entering date and time details for an appointment and allow users to purposefully and successfully create appointments spanning two days  as desired.

<h5>The Tools & Methods</h5>
Pen & Paper, Sketch, Invision, Jira, Direct User Feedback, Usability Research, Sketching & High Fidelity Comps

<h3 class="third-h3">The Approach</h3>

##### 1. Evaluate direct user feedback

For a stronger understanding of the challenges faced with the user's interactions, I completed thorough evaluations of our direct user feedback received by our Customer Service team. 

##### 2. Self test
Only slightly familiar with the FE developer's implemented solution, I tested the appointment creation form several times for a better grasp on the design limitations that led to the frequent error. It was easy to identify how a user could make this error: contextual feedback about the automatic system selection of "Ends Next Day" based on the user's input was completely non-existent. Unless you had double checked your entries, start times, end times, and AM/PM selections, and visibly noticed the small checkbox selected underneath entries, it was quite easy to overlook the system's automated selection.

##### 3. Outline the solution goals
To ensure a proposed solution meets the proper needs of the issue, I find it critical and helpful to outline solution goals:

<ol type="a">
  <li>Allow a user to intentionally and intuitively create an appointment that spans two days</li>
  <li>Prevent a user from creating an appointment with an unintended duration</li>
  <li>Provide contextual feedback and direction in response to pre-form submission entries</li>
  <li>Develop a solution with one date entry per BE development constraints</li>
</ol>

##### 4. Explore similar applications and ideate various solutions
I frequently look to existing and similar applications for inspiration on how certain challenges have been solved before. In this instance, I evaluated several websites and applications with a focused date/time input: Outlook Calendar, Google Calendar, and various airline websites. 
    
I found that Google Calendar and Southwest.com had particularly interesting solutions with applicable pieces to build off of. With the unique challenge of having only a Start Date input, I iterated through sketches of various options and user flows with inspiration from these existing solutions.

##### 5. Generate high fidelity user flows
With our consistent visual styling already established for each application, I find it helpful and quick to produce high fidelity user flows to test against. Importing application specific Sketch style guides and symbols truly increases efficiency in accomplishing this process. 

##### 6. Validate potential solution
Once added to InVision, I presented the user flows to our QA team for testing against the solution goals and overall improvement from the baseline solution. As is often the case, QA helped identify some "what if" scenarios of user inputs, taking me back to steps four and five to update and include important potential user entries in the solution. 

##### 7. Finalize solution
After a couple of cyclical iterations and testing of steps four, five, and six, we were able to successfully identify and finalize an enhanced solution that touched on a handful of smaller improvements as well. 

<h3 class="first-h3">The Solution</h3>

##### Step 1: Select Date
Here a user can either type in the date in the "MM/DD/YY" format, or select a date from the drop down calendar.

<p>
    <img class="pue-images" alt="Step 1: Select Date" src="/images/work/vineya/preventing-user-error/01_select_start_date.png">
</p>

##### Step 2: Select Start Time, Default Drop Down
As a user tabs or clicks over to the start time, the time drop down defaults to 7:00 am, the standard hours start time for jobs. Users can either type in or scroll to enter the start time.

<p class="italic small-note">Date Display Improvement: Note the date display shows the day of the week, month, date of the week and year rather than the MM/DD/YY format. This display helps users to confirm the date they select matches the day of the week. A requestor could easily mistake Friday, June 25th for Friday, June 24th when requesting a job, and now a job creator can visually confirm and correct as needed.</p>

<p>
    <img class="pue-images" alt="Step 2: Select Start Time Default" src="/images/work/vineya/preventing-user-error/02_select_start_default.png">
</p>

##### Step 3: Select Start Time, AM Limit
The start time AM limit prevents users from selecting a start time on the previous day.

<p>
    <img class="pue-images" alt="Step 3: Select Start Time, AM Limit" src="/images/work/vineya/preventing-user-error/03_select_start_am_limit.png">
</p>

##### Step 4: Select Start Time, PM Limit
The start time PM limit prevents users from selecting a start time for the following day.

<p>
    <img class="pue-images" alt="Step 4: Select Start Time, PM Limit" src="/images/work/vineya/preventing-user-error/04_select_start_pm_limit.png">
</p>

##### Step 5: Select End Time, Default
By default, the end time entry will start in 15 minutes increments (the required billing increments for job times), 15 minutes after the selected start time of the job. This default will prevent users from selecting an end time before a start time.

<p class="italic small-note">Job Duration Display: Note the addition of the job duration next to the end times. A lot of job requestors ask for a start time and a duration rather than specifying an end time. This duration display allows job creators to reference the duraction as needed.</p>

<p>
    <img class="pue-images" alt="Step 5: Select End Time Default" src="/images/work/vineya/preventing-user-error/05_select_end_default.png">
</p>

##### Step 6: Select End Time, PM Limit
Lastly, we consider our 24 hour job time limit and make the last time entry 10:30 pm. 

<p>
    <img class="pue-images" alt="Step 6: Select End, PM Limit" src="/images/work/vineya/preventing-user-error/06_select_end_pm_limit.png">
</p>

##### Step 7: Final Entry Display
We end with a much more clear entry display when jobs occur overnight, with a few additional improvements along the way.

<p>
    <img class="pue-images" alt="Step 7: Final Input Entry" src="/images/work/vineya/preventing-user-error/07_final_entry.png">
</p>

This particular issue allowed me to recognize the need to consider more closely what could go wrong with user input, and to anticipate user errors as much as possible for users.

With a product like Vineya that contains so many different elements, I will be continually discovering problems with original and even improved upon designs, and searching for the best improvements for my users.

<h3 class="second-h3">The Learnings</h3>

##### Evaluate all solutions, no matter how quick of a fix they may seem to be
Although quick, untested improvements are often necessary evils in a fast-paced, agile world, they can lead to critical and unintended errors. Seeing the issues occur from this instance has led me to think twice before signing off on a quick solution, especially if the updates are being made to critical aspects of a user's flow, no matter how trivial they may seem at the time. 

##### Take time to design and develop contextual feedback, especially in critical forms
Even with the use of an "Ends Next Day" checkbox as a solution to our problem, the addition of feedback could have prevented many of the errors that users encountered from the quick fix. It's critical to inform any user key information about their interactions to ensure they're achieving their ultimate goals while using a product. 

##### Identify their strengths and collaborate with team members to improve the process and the solution
Through the design process, I discovered how useful QA engineers could be while validating a solution. As a designer, I consider myself to be fairly attuned to user behavior, but often forget about those unexpected "what if" interactions from atypical user paths. Collaborating with our QA team, who focus daily on anticipating all the things a user could try to do to create some sort of bug in the system,  allowed me to develop a more well-rounded, straight-forward solution. I continue to involve their expertise in my process to this day.

<p class="italic small-note">Have any thoughts, ideas, feedback? I love to discuss my work, so <a href="mailto:casiemattrisch@gmail.com">let me know</a>!</p>

<button class="back">
    <a href="/uxui/">Back to UX/UI Work</a>
</button>
