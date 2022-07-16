---
layout: post
title:  "Mgen AdvanceCare Medical Network Map"
categories:
- Stuff
tags: [mgen, advancecare, app]
summary: Plays sound when new bike appears
feature_image: "https://picsum.photos/2560/600?image=666"
date:   2022-07-16
comment: "curl 'https://api-manager-prd-ne.azure-api.net/api/v1/Search/Aggregated?location=Lisboa&networks=4&networks=9'"
---
<script src="https://unpkg.com/vue@3.2.37/dist/vue.global.prod.js" type="text/javascript"></script>
<script
      src="https://maps.googleapis.com/maps/api/js?key=AIzaSyDxwyBxZbZtTzx3uWcSlqncFcDU4kvuE5o"
    ></script>

<style>
.mgen-map {
    height: 500px;
}
.mgen-filters {
    display: flex;
    flex-wrap: wrap;
    padding: 1rem 0;
}
.mgen-filter {
    padding: 0 1rem;
}
.mgen-filter__label {
    padding-left: 0.5rem;
}
.mgen-filter__select {
    width: 10rem;
}
</style>

Web services in western europe suck ass. My health insurance company do it as well: it is nowhere to find a map with all medical services they cover — neither on their website, nor in mobile app. You have to crawl over thousands of rows of data manually looking for your ZIP code and googling addresses all the time.

I've just dumped their JSON API data and saved it locally to make this masterpiece.

Use at your own risk — it's about **6 Mb** of JSON data 😵.

<div id="mgen_app">
</div>

<script async src="app.js" type="module"></script>