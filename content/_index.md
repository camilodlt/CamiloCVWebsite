---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2026-03-23
type: landing

design:
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      button:
        text: View Publications
        url: /publications/
      headings:
        about: ''
        education: ''
        interests: ''
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
    content:
      title: Research
      subtitle: ''
      text: |-
        I am currently in the third year of my PhD, supervised by Sylvain
        Cussat-Blanc, Dennis Wilson, and Hervé Luga. My doctoral work focuses
        on developing a type-aware extension of Cartesian Genetic Programming,
        with applications to program synthesis, game playing, and image
        classification.

        More recently, I have been exploring the intersection of deep learning
        and genetic programming, with the goal of improving GP systems to
        approach deep learning performance while remaining interpretable.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Selected Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: markdown
    id: contact
    content:
      title: Contact
      subtitle: ''
      text: |-
        Use this section for your academic contact details.

        - Email: dlt.camilo@gmail.com
        - GitHub: https://github.com/camilodlt
        - Google Scholar: https://scholar.google.com/citations?user=b7ZpuzkAAAAJ&hl=en
    design:
      columns: '1'
---
