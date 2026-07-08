{% from "common/macros.njk" import embed_topic, show_as_tab with context %}
{% from "common/admin.njk" import show_admin_page with context %}

{% call show_admin_page("textbooks") %}
<div id="main">

**This course is supported by a customized online textbook** [**_Software Engineering for Self-Directed Learners_** ({{ course }} edition)]({{ baseUrl }}/se-book-adapted/index.html), integrated into this course website.

**Topics relevant for a week appear on the weekly schedule page** (see the <span class="text-primary">{{ show_as_tab('Topics', icon_tab_topics) }}</span> tab). Some of those topics come with pre-recorded videos. ==Watching those videos is encouraged but optional==: while they do not cover any theory beyond the textbook, they can offer complementary explanations, more examples, and visualizations.
</div>

<div id="tip-about-lecture-videos" class="indented">

<box type="tip" seamless>

##### Tips for watching pre-recorded videos

* ==We recommend watching the provided <span class="badge rounded-pill bg-danger">++{{ icon_video }} Videos++</span> at faster speeds== (`x1.25` or even `x1.5`) _if_ the current pace of the video feels "too slow" for you.{% if cs2113 %}
* The pre-recorded videos and lecture webcasts are distributed via Canvas.{% else %}
* You'll need to use your NUSNET login to access them.{% endif %}
</box>
</div>

==**A PDF version of the full textbook will be provided**== at the start of the semester, via Canvas. In addition, you can [use this technique](https://se-education.org/guides/tutorials/savingPdf.html) to save the main text of a specific page or chapter as a PDF file.

</div>

{% endcall %}
