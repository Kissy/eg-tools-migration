+++
outputs = ["Reveal"]
title = "EG Tools Migration"
+++

{{< slide background-color="#009" >}}

<h1>EG Tools<br />migration</h1>
<span>(a.k.a. Github & Primer)</span>

---
{{< slide background-color="#009" background-image="background/ian-dooley-hpTH5b6mo2s-unsplash.jpg"
background-repeat="none" background-position="center right" background-size="50%" >}}

<div style="width: 50%; transform: translate(-10vh, 0)">
    <h2>Multiple Outcomes</h2>
</div>

---
## Release faster

Parallel build <i class="fas fa-rocket"></i>  
Compilation ~15% faster  
On <i class="fab fa-aws"></i> cloud  

<img src="primer-executors.png">

---
## Simplified workflow

* Requires a JIRA key to commit
* Code Review using Github PR
* Sonar integration in PR

---

### SSAE Workflow enforced

<img src="pr-review-required.png" />

---
### Alert developer on   code issues

<img src="sonar-error-report.png" />

---
### Warn reviewer of introduced issues

<img src="sonar-full-report.png" />

---
## Building Containers

<br />
<p style="font-size: 4em;">
    <img src="eg-logo.png" style="margin: 0; height: 1em; width: auto; vertical-align: top;">
    <i class="fas fa-cogs"></i>
    <i class="fab fa-docker"></i>
</p>

---
### Managed by 
## EG Delivery Platform
* 6 Engineering Managers
* ~40 Engineers worldwide
* 3 Product owners

---
{{< slide background-color="#009" background-image="background/keo-oran-oD4zvae0IDA-unsplash.jpg"
background-repeat="none" background-position="center right" background-size="50%" >}}

<div style="width: 50%; transform: translate(-10vh, 0)">
    <h2>Behind the scene</h2>
</div>

---
{{< slide background-image="background/three-sections-bg.png"
background-repeat="none" background-position="center" background-size="contain" >}}

<div class="three-sections">
  <h2><i class="fab fa-github"></i>&nbsp;Github</h2>
  <h2 style="color: white;">Deployment Console</h2>
  <h2><i class="fab fa-jenkins"></i>&nbsp;Primer</h2>
</div>

---
{{< slide auto-animate="" >}}

## Migration scope
<div data-id="gitlab-to-github" class="arrow-container" style="font-size: 5em;">
    <i data-id="gitlab" class="fab fa-gitlab"></i>
</div>

<p>~620 projects</p>

---
{{< slide auto-animate="" >}}

## Migration scope
<div data-id="gitlab-to-github" class="arrow-container" style="font-size: 5em;">
    <i data-id="gitlab" class="fab fa-gitlab"></i>
    <div data-id="arrow" style="display: inline-block;">
        <span class="css-arrow"><span class="css-arrow__leg"></span> <!----></span>
    </div>
    <i data-id="github" class="fab fa-github"></i>
</div>

1. Copy all projects data
2. Configure settings (PCI & SSAE)
3. Update ~500 project files
4. Create ~2300 config files

---
{{< slide background-image="background/python-code.png" background-size="contain"
background-repeat="none" background-position="center left" >}}

<h3 class="r-fit-text"><i class="fab fa-python"></i> Python & APIs</h3>

Call Gitlab & Github APIs,  
bulk modify configuration files.

---
{{< slide background-image="background/hide-the-pain.jpeg"
background-repeat="none" background-position="top" background-size="cover" >}}

<br />
<br />
<br />
<br />
<br />
<br />
<h2  class="r-fit-text">That works well until you are blocked</h2>
<p class="r-fit-text">for reaching API Limits <i class="far fa-hourglass"></i><p>

---
## Deployment Console

No public API available <i class="fas fa-ban" style="color: red"></i>  
Written in ReactJS <i class="fab fa-react"></i>  
  
<span class="fragment">Still ~500 projects to onboard...</span>

---

<img src="react-dev.png" />  

Allow access to ReactJS <i class="fab fa-react"></i>  
components from Chrome console 

---

{{< slide background-image="background/three-sections-bg.png"
background-repeat="none" background-position="center" background-size="contain" >}}

<div class="three-sections">
  <h2 style="display: inline">
    <span style="display: inline-block; margin-top:0.5em;">Github</span>
    <span style="display: block;" class="fragment"><i class="fas fa-check" style="color: green"></i></span>
  </h2>
  <h2 style="color: white; display: inline;">
    <span style="display: inline-block;">Deployment Console</span>
    <span style="display: block;" class="fragment"><i class="fas fa-check" style="color: green"></i></span>
  </h2>
  <h2 style="display: inline">
    <span style="display: inline-block; margin-top:0.5em;">Primer</span>
    <span style="display: block;" class="fragment"><i class="fas fa-sign-language"></i></span>
  </h2>
</div>

---

# Migration done in  
# 7 days thanks to automation
