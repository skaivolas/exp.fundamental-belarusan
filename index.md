---
title: Index
layout: post
---


  <!---<h1 class="content-listing-header sans">Articles</h1>          <hr class="slender">--->
  <h2>Pages</h2>
  <ul class="content-listing ">
    {% assign pages=site.pages | where: "iflanding", "yes"  %}    
    {% for spage in pages  %}      
        <li class="listing">
          <a href="{{ spage.url | prepend: site.baseurl }}"><h3 class="contrast">{{ spage.title }}</h3>
          <!---<br><span class="smaller">{{ page.date | date: "%B %-d, %Y" }}</span>  <br/>--->
          <div><img style="float:right;padding:15px;" width="164" src="{{ spage.demoimage | prepend: site.baseurl }}" />{{ spage.excerpt }}</div></a>
        </li> 
    {% endfor %}
  </ul>

  <!---<h1 class="content-listing-header sans">Articles</h1>          <hr class="slender">--->
  <h2>Posts</h2>
  <ul class="content-listing ">
    {% assign pages=site.posts | where: "iflanding", "yes"  %}    
    {% for spage in pages  %}      
        <li class="listing">
          <a href="{{ spage.url | prepend: site.baseurl }}"><h3 class="contrast">{{ spage.title }}</h3>
          <!---<br><span class="smaller">{{ page.date | date: "%B %-d, %Y" }}</span>  <br/>--->
          <div><img style="float:right;padding:15px;" width="164" src="{{ spage.demoimage | prepend: site.baseurl }}" />{{ spage.excerpt }}</div></a>
        </li> 
    {% endfor %}
  </ul>


 <h2>Repositories</h2>

<div class="github-widget" data-user="skaivolas"></div>


<script src="github-widget/github-widget.min.js"></script>

