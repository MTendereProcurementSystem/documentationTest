<div class="sidenav">
    <h1 id="h.aqvdwxcpbumt">Table of contents</span></h1>
        {% for p in site.pages %}
            <button class="accordion" {% if p.url == page.url %} class="active" {% endif %}> {{page.title}} </button>
        {% endfor %}
</div>

<script>
    var acc = document.getElementsByClassName("accordion");
    var i;
    for (i = 0; i < acc.length; i++) {
        acc[i].addEventListener("click", function () {
            this.classList.toggle("active");
            var panel = this.nextElementSibling;
            if (panel.style.display === "block") {
                panel.style.display = "none";
            } else {
                panel.style.display = "block";
            }
        });
    }
</script>
