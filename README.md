# Introduction
In our project we have demonstrated the following
* Manage issues and pull requests, as well as keeping track of issues using the Project board
* Set up a readme file with
* Show team members and their avatars using markdown
* Show some C code that we have written with syntax highlighting
* Apply a status badge to our code
* Lastly, we were able to promote our repository

# Code
``` c
#include <stdio.h>
int main(){
  printf("hello world");
  return 0;
}
```
![Generic Badge](https://github.com/ikim0106/dummy_repo/blob/main/badge.svg)

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

---
Last updated: {{ site.time }}
