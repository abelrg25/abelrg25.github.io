---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional) 
      button: 
        text: Download CV
        url: ../uploads/ARG_DataAnalyst_CV_Eng_v3.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: unsplash.jpg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 Scientific Research & Data Analytics: My Experience'
      subtitle: ''
      text: |-
        <div align="justify"> As an Early Career Researcher, I led various projects that resulted in the publication of two research articles in high-impact journals worldwide. I also collaborated with international groups on different projects, leading to the publication of three additional scientific articles.

        During this period, I developed a range of skills, including a comprehensive understanding of **Python** and its various data analysis packages such as **Pandas**, **NumPy**, **SciPy**, **Astropy**, and **Scikit-learn**, as well as visualization tools like **Matplotlib**, which helped me prepare and interpret data effectively. I also gained experience working with operating systems such as **macOS**, **Linux**, and **Windows**.

        Additionally, I completed the Google Data Analytics Certificate, expanding my expertise in **SQL**, **Excel**, **R**, and **Tableau**. This allowed me to strengthen my ability to manipulate, visualize, and analyze data efficiently.

        Finally, I learned to present my results at various national and international conferences, in both English and Spanish, tailoring my communication for audiences from a wide range of scientific disciplines. 
        Please reach out to collaborate! 😃 </div>
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Talks
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 1
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 👉 Build your own academic website like this
      text: |-
        This site is generated by Hugo Blox Builder - the FREE, Hugo-based open source website builder trusted by 250,000+ academics like you.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>

        Easily build anything with blocks - no-code required!
        
        From landing pages, second brains, and courses to academic resumés, conferences, and tech blogs.
      button:
        text: Get Started
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
