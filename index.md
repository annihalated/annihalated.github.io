---
hide_sidebar: true  
---
{% include intro.md %}

<h2 class="bottom15">Recent Essays</h2>
<div class="row bottom15">

{% for post in site.posts limit:3 %}
  <div class="post-header-home col-sm-4">
    <h3 class="post-title-home"><a href="{{ post.url | prepend:site.baseurl}}">{{post.title}}</a></h3>
    <div class="post-excerpt-home">
      {{post.excerpt}}
        <p class="text-right"><a href="{{ post.url | prepend:site.baseurl}}">Continue Reading &rarr;</a></p>
    </div>
  </div>
{% endfor %}
</div>


<hr>  
<div class="home-read-more">
  <a href="{{ "/archive" | prepend:site.baseurl }}" class="btn btn-primary btn-block btn-lg">All {{ site.posts | size }} Essays →</a>
</div>

