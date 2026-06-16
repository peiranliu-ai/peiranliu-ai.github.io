---
permalink: /
title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  @media screen and (min-width: 1600px) {
    .page {
      transform: translateX(-5rem);
    }
  }

  .home-news {
    margin-top: 1.7rem;
    padding-top: 0.35rem;
  }

  .home-news h2 {
    margin-bottom: 0.65rem;
    padding-bottom: 0.28rem;
    color: #174d78;
    font-size: 1.05rem;
    line-height: 1.25;
    border-bottom: 1px solid #d7e2ea;
  }

  .news-list {
    display: grid;
    gap: 0.48rem;
  }

  .news-item {
    display: grid;
    grid-template-columns: 5.6rem minmax(0, 1fr);
    gap: 0.68rem;
    align-items: center;
    min-height: 4.5rem;
    padding: 0.44rem 0.72rem;
    border: 1px solid #d9e2ea;
    border-left: 4px solid #2c6f9e;
    border-radius: 6px;
    background: #f8fbfd;
  }

  .home-news .news-date {
    color: #174d78;
    font-size: 0.64rem;
    font-weight: 800;
    line-height: 1.25;
    letter-spacing: 0;
    text-transform: uppercase;
  }

  .home-news .news-text {
    margin: 0;
    color: #263746;
    font-size: 0.7rem;
    line-height: 1.3;
  }

  .home-news .news-text strong {
    color: #142236;
    font-weight: 800;
  }

  @media screen and (max-width: 520px) {
    .news-item {
      grid-template-columns: 1fr;
      gap: 0.28rem;
    }
  }
</style>

<!--

This is the front page of a website that is powered by the [Academic Pages template](https://github.com/academicpages/academicpages.github.io) and hosted on GitHub pages. [GitHub pages](https://pages.github.com) is a free service in which websites are built and hosted from code and data stored in a GitHub repository, automatically updating when a new commit is made to the repository. This template was forked from the [Minimal Mistakes Jekyll Theme](https://mmistakes.github.io/minimal-mistakes/) created by Michael Rose, and then extended to support the kinds of content that academics have: publications, talks, teaching, a portfolio, blog posts, and a dynamically-generated CV. Incidentally, these same features make it a great template for anyone that needs to show off a professional template!

 You can fork [this template](https://github.com/academicpages/academicpages.github.io) right now, modify the configuration and Markdown files, add your own PDFs and other content, and have your own site for free, with no ads!

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, Academic Pages makes you separate the website's content from its form. The content & metadata of your website are in structured Markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various Markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your Markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over - just be sure to save the Markdown files! You can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

For those users that need more advanced functionality, the template also supports the following popular tools:
- [MathJax](https://www.mathjax.org/) for mathematical equations
- [Mermaid](https://mermaid.js.org/) for diagraming
- [Plotly](https://plotly.com/javascript/) for plotting

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this template](https://github.com/academicpages/academicpages.github.io) by clicking the "Use this template" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one Markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a Markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each Markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual Markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the Markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and Markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a Markdown file for a talk
![Editing a Markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.

-->

I am a third year PhD student at [Edwardson School of Industrial Engineering](https://engineering.purdue.edu/IE), [Purdue University](https://www.purdue.edu/), under guidence of [Prof. Denny Yu](https://engineering.purdue.edu/IE/people/ptProfile?resource_id=134078). I hold a Bachelor’s degree in Information Systems in University of Florida. I worked as an intern at [BrainCo](https://brainco.tech/#/) in 2023, and [Coohom](https://www.coohom.com/) [SpatialVerse](https://www.spatial-verse.com/) in 2025. My research focus on safety & usability in transportation and healthcare with AI and digital twin.

<section class="home-news" aria-label="News">
  <h2>News</h2>
  <div class="news-list">
    <article class="news-item">
      <div class="news-date">October 2026</div>
      <p class="news-text">Our work <strong>“Monitoring the Progress of Human-Centered Teaming Communication with Keep Talking Simulation”</strong> has been accepted to the IEEE International Conference on Systems, Man, and Cybernetics (SMC) 2026 in Bellevue.</p>
    </article>

    <article class="news-item">
      <div class="news-date">May 2026</div>
      <p class="news-text">Our work <strong>“Automated Assessment of PPE Compliance with Fast Lightweight Deep Learning Based Computer Vision”</strong> is presented at the IISE Annual Conference 2026 in Arlington, TX.</p>
    </article>

    <article class="news-item">
      <div class="news-date">October 2025</div>
      <p class="news-text">Our work <strong>“Are LLMs the New Ergonomists? Predicting Lifting Risks with LLMs And Machine Learning”</strong> is presented at ASPIRE&mdash;The HFES International Annual Meeting 2025 in Chicago.</p>
    </article>

    <article class="news-item">
      <div class="news-date">September 2024</div>
      <p class="news-text">Our work <strong>“Computer vision embedded post-processing algorithm on lifting risks”</strong> is presented at ASPIRE&mdash;The HFES International Annual Meeting 2024 in Phoenix.</p>
    </article>

    <article class="news-item">
      <div class="news-date">June 2024</div>
      <p class="news-text">Our work <strong>“Are LLMs the New Ergonomists? Predicting Lifting Risks with LLMs And Machine Learning”</strong> is presented at the IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR) 2024 in Seattle.</p>
    </article>

    <article class="news-item">
      <div class="news-date">March 2024</div>
      <p class="news-text">Our work <strong>“Computer vision and tactile glove: A multimodal model in lifting task risk assessment”</strong> is presented at the 27th Annual Applied Ergonomics Conference (AEC) 2024 in Louisville, KY.</p>
    </article>
  </div>
</section>
