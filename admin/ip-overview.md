{% from "common/admin.njk" import show_admin_page with context %}

{% call show_admin_page("ip-overview") %}
<div id="main">

<div id="title">

</div>
<div id="body">

<div tags="m--cs2103 m--cs2113">

**The objectives of the individual project (iP)** are to learn or refresh the basics of:
* Java
* OOP
* IDEs
* Git and GitHub
* Project automation tools
* Code quality

</div>
<div tags="m--cs2103 m--cs2113">

**All the skills you learn in the iP will be useful in the team project (tP)**. Some of the iP code can even be adapted for the tP.<br>
{{ icon_tip }} The more you do in the iP, and the farther you go beyond the minimal expectations, the easier the tP will be.

**The iP is based on the generic project called [_Project Duke_](../se-book-adapted/projectDuke/index.html)**. Its overview is given below.

<include src="dukeFragment.md" boilerplate var-header="**Overview**" var-fragment="text.md#intro" />
<br>

**You will do the iP over the first half of the semester**.

</div>

</div>
</div>

{% endcall %}
