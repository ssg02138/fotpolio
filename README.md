# Kim Bumsuk Portfolio

This repo contains an easy-to-customize personal dev portfolio template that was created with Sass and JavaScript. It is lightweight and fully responsive, as well as comes with the Bootstrap grid system and loaded with Font Awesome. The site is static and comes production ready if you just want to add your information and go. Alternatively, you can edit styles, colours, and scripts fairly easily. The site was built as modular as possible to make it easy to shift around styles and content.

To view a my portfolio, [click here](https://ssg02138.github.io/).

## Features

* Gulp ready (compiles Sass and minifies JS)
* Sass ready with lots of commenting
* Fully responsive
* Comes with Bootstrap grid system
* Easy colour changes can be done through simple variable edits

## Contents

- [Sections](#sections)
    - [About](#about)
    - [Achievement](#achievement)
    - [Education](#education)
    - [Certificate](#certificate)
    - [Experience](#experience)
    - [Projects](#projects)
    - [Skills](#skills)
    - [Contact](#contact)
- [Changelog](#changelog)

## Sections

### About

In about, `Introduce my self`.
About contains the following: [About](https://ssg02138.github.io/index.html#about)

### Achievement

In achievement, show the achievement list.
Achievement contains the following: [Achievement](https://ssg02138.github.io/index.html#achievement)

* Win a Prize to 2019 National Assembly Hackerton - Smart Streetlight System Using Public Data - `Team Leader`
* Win a Prize to 2019 Software Development Security Competition - Location-based tourism information docent service using OpenAPI - `Team Leader`
* Win a Prize to 2019 Hanium ICT Competition - Disaster response and safety management system using Arduino - `Team Leader`
* Patent Application - USER ADAPTIVE NEWS SERVICE METHOD AND SERVER BASED ON DEEP LEARNING

### Education

The header section can be found within the `<header>` tag and simply contains an unordered list of anchors to different sections of the page. If you add a new section and want to be able to quickly navigate to it from the top, simply add another list element with an anchor that has the href of the ID of the section. Conversely, if you remove a section, don't forget to remove the associated navigation element.

If you wish to add a header link to an external page, simply add the class `no-scroll` to the anchor. For example:

```HTML
<li>
    <a href="https://google.com" class="no-scroll">Google</a>
</li>
```

If you wish to have a sticky (fixed) header, you simply need to add a class of `sticky` to the main header. For example, that would be accomplished as follows:

```HTML
<header class="sticky">
    <!-- Header content -->
</header>
```

### Projects

The Lead section is pretty straightforward, it contains an h1 for your name and an h2 for your title. It also contains a link that can be used to link to your resume should you wish to add it as well.

If you want your resume to automatically download when the button is clicked instead of opening up in another tab (the default behaviour), add the following code (Thanks to jkfran for the suggestion) in the lead:

```HTML
<a href="path/to/resume.pdf" download="resume.pdf" class="btn-rounded-white">Download Resume</a>
```

The href attribute points to where your resume is stored and the download attribute is what triggers the download / provides the name the file will be downloaded as when the user clicks the button (In this case, it will download as resume.pdf).

### Skills

The about section contains a quick about blurb that can be edited by changing the text within the paragraph tags.

### Contact

The experience section creates a vertical timeline with all your relevant experience. The code for the timeline creation can be found within `js/scripts.js` and is an adaptaion of [RyanFitzgerald/vertical-timeline](https://github.com/RyanFitzgerald/vertical-timeline).

The default format is as follows:

```HTML
<div id="experience-timeline">
    <div data-date="September 2015 – September 2016">
        <h3>Employer Name</h3>
        <h4>Job Title</h4>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur in iaculis ex.
        </p>
    </div>
</div>
```

The data attribute `data-date` is what is used to add a date to the associated timeline point. All that is really required is a wrapping div (i.e. `#experience-timeline`) and nested divs to build the timeline. The h3, h4, and p tags are optional and the contents of the div can be styled however you wish.

To add additional section, simply add additional nested divs under the main wrapping div.

## Changelog

### 1.0.0

* As of 2020. 05. 23.
