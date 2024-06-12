---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

{%- assign python = site.languages | where: "title", "Python" | first -%}

## Welcome!
Thanks for taking the time to visit! This site is intended for 
prospective employers to learn a little more about me and my 
professional experiences. 

Most pages include links to related items. Want 
to know about what Python projects I have worked on? Go to [languages]({% link languages.md %}) and 
select [python]({% link {{python.path}} %}). The related projects are listed 
at the top of the page.

### [About]({% link about.md %})
Learn more about my recent 
professional journey.

### [Languages]({% link languages.md %}) 
Lists the coding languages I 
have used and described my experiences with them.

### [Projects]({% link projects.md %}) 
Provides a short description of some 
of the technical projects I have worked on.

### [Roles]({% link roles.md %}) 
A breakdown of some of the recent roles I have had.

### [Skills]({% link skills.md %}) 
Non-technical skills I have developed in my different roles.

### [Tools]({% link tools.md %}) 
A list of tools that I have used or been trained in.
