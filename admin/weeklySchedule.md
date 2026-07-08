{% from "common/macros.njk" import embed_topic with context %}
{% from "common/admin.njk" import show_admin_page with context %}

{% call show_admin_page("weeklySchedule") %}
<div id="main">

<div tags="m--cs2103" id="week-definition">

### Timing of the {{ lecture_name }}

As our lecture slot (which we use for the weekly briefing) is at the end of the week, ==the briefing in the Week~n~ lecture slot covers a recap of Week~n~ and a preview of Week~n+1~== %%e.g., The briefing on week 3 {{ day_lecture }} covers a recap of week 3 and a preview of week 4%%.

</div>
<p/>
<div id="deadline-definition">

### Deadline for weekly tasks

<span class="text-danger">**The deadline** for weekly tasks is {{ day_lecture }} {{ time_lecture_start}}</span>, i.e., the lecture slot start time. Work done after that time %%(e.g., code committed after {{ day_lecture }} {{ time_lecture_start}})%% will be credited for the following week.

{% if not cs2113 %}**It's OK to miss a few weekly project deadlines occasionally**; i.e., we'll not penalize you for occasionally missing those deadlines, **provided you catch up soon** (i.e., catch up within a few days after the deadline). This flexibility does not apply if a task description states a specific deadline.<br>
{% endif %}

**It's OK to make occasional mistakes in weekly tasks**. Making mistakes is a natural part of learning new things, after all. If a weekly task was not accepted as 'done' due to a mistake you made, go ahead and rectify the mistake as soon as you can -- in most cases, our grading scripts will not penalize such mistakes if they are corrected soon after.

**We won't wait forever, though.** Note that for most interim deliverables, we stop checking about one week after the deadline has passed. So, work/corrections done more than one week after the deadline might not get noticed at all by our grading scripts, even as late submissions.
</div>

### Timing recommendations

* **Start Week~n+1~ tasks on Week~n~ Friday**. As the Week~n+1~ briefing is held on Week~n~ Friday (i.e., ~2 days before the week actually starts), we recommend that you start Week~n+1~ tasks on that same Friday. That way, you have more time to finish them by the Week~n+1~ deadline (i.e., Week~n+1~ {{ day_lecture }} {{ time_lecture_start}}).{{ bullet_checkbox_selected_green }}
* <span id="before-attempting-tasks">**Before attempting weekly project tasks, go through the weekly topics**{% if not cs2103 %} (and do the weekly programming exercises/activities, if any){% endif %} because the knowledge from those topics may be needed to complete the project tasks.</span>
* **Try to finish most weekly tasks before attending the tutorial of that week**, because some tutorial tasks are most useful _after_ you have completed the weekly tasks.

</div>
{% endcall %}
