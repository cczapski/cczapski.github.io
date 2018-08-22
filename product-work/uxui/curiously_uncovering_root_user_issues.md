---
layout: product-work
case-study: Curiously Uncovering Root User Issues
description: Understanding the root user challenges instead of leading with proposed sales and user solutions
permalink: /uxui/curiously-uncovering-root-user-issues
---

<h3 class="first-h3">The Problem</h3>
A fairly frequent occurrence, our sales team alerted us of an urgent need driven by our largest customer: integrate our system with any, and every, financial software, with priority towards QuickBooks. 

When we asked the sales team for more details around  the suddenly essential need, we were informed that the customer simply expressed that they must have this ability to effectively operate, with zero additional details. Knowing that integrating our full system into QuickBooks alone (not even considering any and every financial software) was no small task, our team knew we had to more fully evaluate the customer's needs to determine what was possible. 

I personally had the great, burning question: why? What had prompted this customer of a year to all of a sudden express such high urgency towards this new feature request? 

Luckily, given the countless unknowns around this pressing need, I was able to convince the sales team to allow me to join a customer meeting to interview our users and better understand the request. It's important to note that this was no small task given the sales team's resistance towards allowing any Software Development team member to interact with customers. 

Thus the problem was identified: <span class="emphasis">how to determine the root user issues of such as immediate feature request to ensure a realistic and effective solution could be determined.</span>


<h3 class="second-h3">The Details</h3>

<h5>The Application</h5>
<a href="/work/what-is-vineya" target="blank">Vineya</a> for Agencies web application

<h5>The Users & Audience</h5>
Agency administrators, particularly those with a financial focus on their business, representing approximately 40% of Vineya for Agencies users

<h5>The Team & Role</h5>
I was first responsible for researching the user needs in collaboration with our sales team, and then responsible for designing an effective user experience for the determined solution with development guidance from a Front End Developer and our Data Specialist. 

<h5>The Tools & Methods</h5>
GoToMeeting, Pen & Paper, Sketch, InVision, Remote User Interviews, Sketching & High Fidelity Comps

<h3 class="third-h3">The Approach</h3>
##### 1) Preparing for remote user interviews 
Excited for some face to face time with our users, I prepared focus questions to gain a deeper understanding of the user's current challenges and goals:
* Can you explain what activities you'd like to achieve through integrating Vineya with QuickBooks? 
* What is the process that you have taken to achieve these activities since using Vineya over the past year? 
* How frequently do you have to perform these activities? 
* What specific Vineya data is most important to integrate into QuickBooks? 
* Have you used an interpreter scheduling and management system in the past that allowed you to achieve your main goals? And if yes, what did you like and dislike about their process? 
    
##### 2) Identifying the real problem
During the interviews, I started to get a more clear picture of what had been so time consuming for the users. In an effort to merge Vineya data into their QuickBooks software, a daily activity, users would first download various Vineya canned reports that included any and every data piece related to that report. They would then delete unnecessary columns and rearrange the data to their needs before manually entering data into QuickBooks.
    
I could understand why the solution requested was to integrate Vineya into QuickBooks; however, knowing the development complexity of that solution, I wanted to see if there were other options that could perhaps be achieved quicker and could also benefit the unique financial and data processes of other Agency users. 
    
##### 3) Establishing solution goals
1. Decrease the amount of time users take to manipulate canned Vineya reports to fit their needs
2. Allow customization of Vineya reports
3. Ensure the solution is applicable and beneficial to our full agency user base
4. Determine if a less time consuming and complex development solution exists
    
##### 4) Ideating more realistic solutions
Given the discussion in the interview was heavily focused around QuickBooks and the customer's ability to more easily manipulate QuickBooks reports through custom web reporting options, we started to wonder about us focusing on a custom web report solution in Vineya. If we allowed users to customize our existing reports and organize the data to fit their needs, the customer could then easily import tailored reports using the QuickBooks data import feature. 
    
##### 5) Determining the development possibilities
With a fresh idea, we discussed the realistic implications from a development perspective. Yes, we could integrate our system with QuickBooks, but the process was estimated to take both FE and BE bandwidth over a series of months. Focusing on custom reporting tools to existing reports would only need the work of one FE developer and our Data Specialist over a month or two.
    
##### 6) Designing the solution
Balancing the pros and cons of each solution, and knowing that each option would meet the users needs of more easily integrating Vineya data into their financial software, we decided to proceed with the less complex option that we could implement into production much quicker.
    
At that point, I took inspiration from QuickBooks' customized reporting and some of the common themes from the user interview and proceeded from initial sketches to high fidelity comps for the final solution.

<h3 class="first-h3">The Solution</h3>
First, a user has the option to create a custom report from one of the many existing canned reports. 

<p>
    <img class="img-shadow-dark" alt="Create Custom Report" src="/images/work/uxui/root-user-issues/01_create_custom_report.png">
</p>

From there, the user has various options on the report page to aid in flexibility around use cases:
* Change the predefined report period or custom date range
* Further customize the report to edit the title, pre-set reporting timeframes, and included columns
* Save any changes to an existing report or as a new report
* Download a .CSV file of the report
* Sort the report columns and remember the selections on saved reports
* Move the columns into any preferred order within the browser view

<p>
    <img class="img-shadow" alt="View Custom Report" src="/images/work/uxui/root-user-issues/02_view_custom_report.png">
</p>

<p>
    <img class="img-shadow-dark" alt="Edit Custom Report" src="/images/work/uxui/root-user-issues/03_edit_custom_report.png">
</p>

In cases where users start to navigate away from a report with unsaved changes, they are first asked to confirm that they would like to leave without saving their changes. 

<p>
    <img class="img-shadow-dark" alt="Save Before Leaving" src="/images/work/uxui/root-user-issues/04_save_before_leaving.png">
</p>

And finally, users can manage existing reports by running, copying, or deleting any custom reports. r

<p>
    <img class="img-shadow" alt="Manage Custom Reports" src="/images/work/uxui/root-user-issues/05_manage_custom_reports.png">
</p>

<h3 class="second-h3">The Learnings</h3>
##### Focus on the problem, not the proposed solution
Our sales team has always liked to present us with desired feature requests. Based on our processes at the time for establishing priorities, the Software Development team would simply take their feature requests and implement them. Fortunately this feature request was large and vague enough that we had the opportunity to more fully evaluate and ask the "Why" behind the request to uncover the true issues and implement the better solution.
    
##### Despite organizational resistance to direct user interactions, be persistent! 
Since day one with the organization, I have always requested direct user interaction through research and haven't always been successful in achieving buy in to incorporate that key piece into our process. Through this experience and now a handful of others, I've learned that creative persistence is always worth pursuing when it leads to a better solution for my end users.

<p class="italic small-note">Have any thoughts, ideas, feedback? I love to discuss my work, so <a href="mailto:casiemattrisch@gmail.com">let me know</a>!</p>

<div class="resume">
  <button class="back">
      <a href="/ux-ui/">Back to UX/UI Work</a>
  </button>
</div>