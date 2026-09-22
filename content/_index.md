---
title: ''
summary: 'Zhenyue Gu — incoming PhD student researching embodied AI, multimodal perception, and computational cognitive modeling.'
type: landing
sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      headings:
        about: About me
        education: Education
        interests: Research interests
    design:
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle
  - block: markdown
    id: research
    content:
      title: Research
      text: |
        My research interests span embodied AI, multimodal perception, and computational cognitive modeling. My previous work has explored computer vision for UAV obstacle detection, and machine learning for machinery reliability analysis.

        [Explore my research projects](/projects/).
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publication
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: papers
    content:
      title: Publications
      text: '[View all publications](/publications/) or visit my [Google Scholar profile](https://scholar.google.com/citations?user=s4FCNVUAAAAJ&hl=en). \* denotes the corresponding author.'
      count: 6
      order: desc
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation
---
