---
layout: product-work
project: Preventing User Error
permalink: /work/vineya/preventing-user-error
technologies: Research, Pen & Paper, Sketch, InVision
---

<h3 class="first-h3">The Problem</h3>

During job creation, a user can create a job that spans across two days, but only for jobs that go overnight (i.e. 11:00 pm - 1:00 am) or within 24 hours of the start time. Multi-day jobs must be created in two separate jobs. Based on how the back end developers set up their data, only one day as a data point was being stored, thus requiring us to solve this circumstance with a start date entry only. 

As a suggestion from a front end developer, we added a “Ends Next Day” checkbox below the start date, start time and end time inputs in the job creation form, a seemingly quick solution to the problem. 

<p>
    <img alt="Original Date/Time Picker" src="/images/work/vineya/preventing-user-error/original_date_time_picker.png">
</p>

In practice however, this was quite the opposite of a quick solution. Our quality assurance team discovered an issue, or bug, when a user would select an end time either the same or earlier than the start time, this “Ends Next Day” checkbox would automatically check without providing any error or feedback (how would the form know that’s not what the user wanted), thus causing job creators to create jobs of a incorrect or much longer duration than desired.

<h3 class="second-h3">The Solution</h3>

Given that the date and time entry of a job are two of the most important details for a scheduling platform, I realized we needed an effective and straightforward solution. I took some time to better understand date and time inputs. I explored various solutions that are out there already, Outlook Calendar, Google Calendar, various airline flight pickers, Dribbble, Pinterest, wherever I could think to search.

It turned out that Google Calendar and Southwest Airlines, despite having two entries for dates, had some great solutions to these inputs that essentially don’t even give a user a chance to input an incorrect time. I got my inspiration for an input solution mostly from these two examples.

Here's a quick walk through of the key improvements designed to prevent this particular issue, and improve upon a few other areas as well.


##### Step 1: Select Date
Here a user can either type in the date in the "MM/DD/YY" format, or select a date from the drop down calendar.

<p>
    <img class="pue-images" alt="Step 1: Select Date" src="/images/work/vineya/preventing-user-error/01_select_date.png">
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

<p class="italic small-note">Have any thoughts, ideas, feedback? I love to discuss my work, so <a href="mailto:casiemattrisch@gmail.com">let me know</a>!</p>
