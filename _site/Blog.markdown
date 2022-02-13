
<!DOCTYPE html>
<html lang="en">

{% include head.html %}

<body>
{% include hero.html %}

<div class="container">
  <div class="row animate">
    {% if site.posts.size > 0 %}
      {% for post in paginator.posts %}
        {% include article.html %}
      {% endfor %}
    {% endif %}
  </div>
</div>

{% include pagination.html %}

{% include section-tags.html %}
    {% if site.google-analytics %} {% include google-analytics.html %} {% endif %} {% include header.html %}

    <!-- begin content -->
    <main class="content" aria-label="Content">
        {{ content }}
    </main>
    <!-- end content -->

    {% include footer.html %}
    <!-- <script>
        const htmlEl = document.documentElement;
        htmlEl.classList.remove('no-js');
        htmlEl.classList.add('js');
    </script>
    <script async defer data-website-id="500347eb-53e0-4928-8591-812d258324f1" src=""></script>
    <script>
        window.$crisp = [];
        le id;
        (function() {
            d = document;
            s = d.createElement("script");
            s.src = "https://client.crisp.chat/l.js";
            s.async = 1;
            d.getElementsByTagName("head")[0].appendChild(s);
        })();
    </script> -->
    <script src="{{ site.baseurl }}/js/scripts.js"></script>
    <script src="{{ site.baseurl }}/js/common.js"></script>
    <!-- <script src="./js/site.min.js?v=f185ff50be96284c5d2aada4716af199" async="async" defer="defer"></script> -->
</body>

</html>




{% include hero.html %}

<div class="container">
  <div class="row animate">
    {% if site.posts.size > 0 %}
      {% for post in paginator.posts %}
        {% include article.html %}
      {% endfor %}
    {% endif %}
  </div>
</div>

{% include pagination.html %}

{% include section-tags.html %}