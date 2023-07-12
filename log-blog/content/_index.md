---
date: "Fri Jul 07 2023 01:30"
title: "Home"
---

<style>
img.thumb {
  width: 100%;
  height: auto;
  margin-top: 15px;
}
.content:hover {
  box-shadow: 0 3px 10px rgb(0 0 0 / 0.5);
  border: 2px solid black;
}

.content {
  height: auto;
  width: 30%;
  padding: 5px;
  border: none;
  border-radius: 2px;
  margin: 5px 0px;
  position: relative;
}
.content::before,
.content::after {
  --scale: 0;
  position: absolute;
  top: -0.25rem;
  left: 50%;
  transform: translateX(-50%) translateY(-100%) scale(var(--scale));
  transform-origin: bottom center;
  transition: 200ms transform;
}

.content::before {
  content: attr(data-tooltip);
  width: max-content;
  max-width: 75%;
  height: auto;
  padding: 0.5rem;
  border-radius: 2px;
  border: 1px solid black;
  box-shadow: 0 3px 10px rgb(0 0 0 / 0.5);
  text-align: center;
  font-size: 11px;
  background: white;
  color: black;
}

.content:hover::before {
  --scale: 1;
}
a {
  border-bottom: none !important;
}
.flex-container{
    display:flex;
    flex-flow: row wrap;
    justify-content: center;
    margin: 20px;
}
h4#img-title {
  padding-top: 5px !important;
}
</style>

<div align="center">
  <img alt="avatar" src="avatar_me.png" width="200" >
  <p>
    Hi! I'm Parker and welcome to the Log Blog! <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="25px">
    <br/><br/>
    This is my personal site that serves as a reference point containing
    information regarding my past and current projects, such as Shopify Theme Development,
    web applications, data mining/analysis, research and blogging.
  </p>
  <hr>
  <p>
    Click on the below links to go to these projects or use the Log Blog menu to view local
    content.
  </p>
  <div class="flex-container">
    <div class="content" data-tooltip="GitHub is a code hosting platform for version control and collaboration.">
      <a href="https://github.com/alanoakes">
      <h4 id="img-title">GitHub</h4>
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" class="thumb" />
      </a>
    </div>
    <div class="content" data-tooltip="Shopify is a user-friendly e-commerce platform that helps small businesses build an online store and sell online through one streamlined dashboard.">
      <a href="about:blank">
      <h4 id="img-title">Shopify</h4>
        <img src="shopify.svg" class="thumb" />
      </a>
    </div>
    <div class="content" data-tooltip="Rpubs is an open publishing platform for HTML documents produced using RMarkdown from within RStudio ...">
      <a href="https://rpubs.com/alanoakes/">
      <h4 id="img-title">RPubs</h4>
        <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/rstudio/rstudio-original.svg" class="thumb" />
      </a>
    </div>
    <div class="content" data-tooltip="... is considered a 'micro-task' site, where you can do relatively quick, small one-off tasks which they call 'gigs.'">
      <a href="about:blank">
      <h4 id="img-title">Fiverr</h4>
        <img src="fiverr.svg" class="thumb" />
      </a>
    </div>
    <div class="content" data-tooltip="Upwork is an online freelance marketplace. Clients come to the platform to look for freelance talent to work on their projects.">
      <a href="about:blank">
      <h4 id="img-title">Upwork</h4>
        <img src="upwork.svg" class="thumb" />
      </a>
    </div>
  </div>

  </p>
</div>
