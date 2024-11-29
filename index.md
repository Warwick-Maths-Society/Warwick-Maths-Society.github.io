---
layout: landingpage
title: Warwick Maths Society
subtitle: University of Warwick
excerpt: 
header_type: splash
header_img: "./assets/img/dan-cristian-padure-h3kuhYUCE9A-unsplash.jpg"
og_image: "./assets/img/banner.png"
include_on_search: true
show_sociallinks: false
project_links:
    - url: https://www.warwicksu.com/societies-sports/societies/maths/
      icon: fa-solid fa-heart
      label: Join us!
---

<style>
body {
    background-image: url("./assets/desync/tiling-background.png");
    background-repeat: repeat;
}
</style>

<div class="text-center my-4 py-5 px-3 bg-primary rounded-lg">
    <h2> Our Latest Post</h2>
    {% assign post = site.posts.first %}
    <a href="{{ post.url }}">
        <h3>{{ post.title }}</h3>
    </a>
    <p class="blogdate">{{ post.date | date: "%d %B %Y" }}</p>
    <p>{{ post.content | strip_html | truncatewords: 60 }}</p>
</div>

<br/>

---

<br/>

<div class="text-center my-4 py-5 px-3 bg-primary rounded-lg chulapa-overlay-img">
    <p><i class="fa-solid fa-users fa-3x"></i></p>
    <h2 class="font-weight-light py-3">Community</h2>
    <p class="lead font-weight-light py-2">Our community of over 500 members is free-to-join, and is committed to being inclusive and welcoming to all!</p>
</div>

<div class="text-center my-4 py-5 px-3 bg-primary rounded-lg chulapa-overlay-img">
    <p><i class="fa-solid fa-book-bookmark fa-3x"></i></p>
    <h2 class="font-weight-light py-3">Academic Resources</h2>
    <p class="lead font-weight-light py-2">
    Drop in to the weekly <span class="font-weight-bold">Maths Café</span> event for some free food and academic help from our Academic Support officers!
    <br/>
    <br/>
    The website is also well-stocked with academic resources, including our <a href="{% link _pages/module-reviews.md %}">module reviews</a>, <a href="{% link _pages/module-guides.md %}">revision guides</a>, <a href="{% link _pages/book-reviews.md %}">book recommendations</a>, and <a href="{% link _pages/essays.md %}">essay archive</a>!
    </p>
</div>

<div class="text-center my-4 py-5 px-3 bg-primary rounded-lg chulapa-overlay-img">
    <p><i class="fa-solid fa-mug-hot fa-3x"></i></p>
    <h2 class="font-weight-light py-3">Weekly Events</h2>
    <p class="lead font-weight-light py-2">Socialise and relax at our weekly <span class="font-weight-bold">Coffee and Cake</span> welfare event run by our Equal Opportunities and Welfare officers, or come along to our <span class="font-weight-bold">Board Game Nights</span> or <span class="font-weight-bold">Movie Showings</span>!</p>
</div>

<div class="text-center my-4 py-5 px-3 bg-primary rounded-lg chulapa-overlay-img">
    <p><i class="fas fa-solid fa-microphone-lines fa-3x"></i></p>
    <h2 class="font-weight-light  py-3">Academic Talks</h2>
    <p class="lead font-weight-light py-2">Attend weekly talks given by guest lecturers covering a variety of exciting topics beyond the standard syllabus</p>
</div>

<div class="text-center my-4 py-5 px-3 bg-primary rounded-lg chulapa-overlay-img">
    <p><i class="fa-solid fa-comments fa-3x"></i></p>
    <h2 class="font-weight-light py-3">Socials</h2>
    <p class="lead font-weight-light py-2">Get to know your coursemates at our various socials, from integration bees to circles and bar crawls.
    <br/>
    <br/>
    Many of our events are sober, so don't worry if you don't want to or can't drink!</p>
</div>