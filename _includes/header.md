[![CH](%7B%7Bsite.baseurl%7D%7D/assets/img/photoeffect.png)](%7B%7Bsite.baseurl%7D%7D/)
[{{site.title}}](%7B%7Bsite.baseurl%7D%7D/) {% assign sorted\_pages =
site.pages | where\_exp: "page", "page.navlevel == 'header'" | sort:
"position" %} {% for node in sorted\_pages %} {% unless
node.nav\_exclude %} {% if page.url == node.url %}
[{{node.title}}](%7B%7Bnode.url%20%7C%20prepend:%20site.baseurl%7D%7D)
{% else %}
[{{node.title}}](%7B%7Bnode.url%20%7C%20prepend:%20site.baseurl%7D%7D)
{% endif %} {% endunless %} {% endfor %} [To the main
site](%7B%7Bsite.maininstitutesite%7D%7D)
