---
layout: home
---

<div align="center" markdown="1">

# Hey there! I'm Diego Fernando Rojas 👋.

### A software developer and diver from Colombia 🇨🇴
### currently living between Barcelona 🇪🇸 and Berlin 🇩🇪
<br>

</div>

<div class="home-paragraph"  markdown="1">

And I live my life at the intersection of technology, underwater exploration, and the pulsating rhythms of techno music. Here, I publish occasionally about:

1. 👨‍💻 **Software:** I enjoy experimenting with software tools. My main focus is profiling, performance, and observability. However, occasionally, I could write about other topics like containers, architecture, tricks, compilers, distributed systems, programming languages, and everything in between.

2. 🐋 **Diving and ocean conservation:** Since I started diving in 2006, I have become a direct witness to how our consumption practices are killing the sea. I'm fully involved in Ocean conservation efforts through storytelling, audiovisual content, and educational content. In this section, I document this journey.

3. 💡 **Misc:** Here, I write my thoughts, notes, quotes, or whatever about software and humanity. These are just random opinions. I'm a native Spanish speaker, so the content in this section will be mainly in Spanish.

4. 🎶 **Techno Music:** A curated list of tracks that I like. Feel the groove!

<div align="center" markdown="1">
<br>
<hr>
<br>

# Latest Post

</div>

{% assign latest_posts = site.posts | where_exp: "post", "post.category == 'misc' or post.category == 'software' or post.category == 'oceans'" %}
<div class="container"  markdown="1">
{%- for post in latest_posts limit:5 -%}
  <div class="row">
    <div class="col-md-12">
      <h2 class="post-title-list">
      <a href="{{post.url | absolute_url }}">
        {{ post.title }} {{ post.emoji }}
        </a>
      </h2>
      <br>
    </div>
{%- endfor -%}
</div>
