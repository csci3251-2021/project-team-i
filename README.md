# Introduction
Gonna set up a repo. Things left:
* Task 5: Keep checking...
* Task 6: Write C code
* Task 7: Get a status badge
* Task 8: Promote your repo

# Code
//please write the code here
# Contributors
{% for staff_member in site.stu %}
  <p><img class="media-object" src="{{ staff_member.image }}" width="50px" height="50px">
     {{ staff_member.name }}
    <a href="https://github.com/{{ staff_member.user }}">
      @{{ staff_member.user }}
    </a>
  </p>
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}
