---
avatar: "avatar.jpg"
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: '6rem'

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: |-
        I’m a PhD researcher in Climate Science / Physical Oceangraphy at the University of Cambridge, Department of Earth Sciences. My work focuses on Southern Ocean and Atlantic water-mass dynamics, with particular interest in Antarctic Bottom Water, Circumpolar Deep Water, and shelf processes in the Bellingshausen Sea near the Antarctic Peninsula.

        Methodologically, I combine observations (GO-SHIP, GLODAP, Argo, autonomous gliders), inverse methods, and machine learning to classify water masses and map their variability. I also work with data-assimilating and high-resolution models (ECCO/MITgcm) to study the processes that enable warm water to access ice shelves.

        I build Python workflows (xarray, dask, scikit-learn) on HPC systems and maintain tooling for large NetCDF/Zarr datasets and glider QC/calibration. Current projects include classifying Atlantic water masses from OMP-derived fractions, assessing poleward migration of CDW, and producing a global mapped transient tracer product.

        If you’d like to collaborate, please get in touch.
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: 'About'
        education: 'Education'
        interests: 'Research interests'
    design:
      # Apply a gradient background
      css_class: hbx-bg-gradient
      # Avatar customization
      avatar: 
        size: medium # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded

  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I study large-scale overturning and water-mass pathways from the Atlantic to the Antarctic margin, with emphasis on:

        - **Southern Ocean water masses:** AABW formation/change; CDW variability and southern boundary shifts; shelf processes in the Bellingshausen Sea.  
        - **Classification & mapping:** Training ensemble machine learning models to apply water-mass labels to Argo and model fields, integrating GO-SHIP/GLODAP/Argo with ECCO and MITgcm. Mapping transient tracer distributions with Neural Networks. 
        - **Gliders:** Cross-over calibration/QC and workflow tooling for Slocum/Seaglider missions on the Antarctic shelf.

        
    design:
      columns: '1'

  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      view: article-grid
      columns: 2

  - block: collection
    content:
      title: Recent Publications
      text: ''
      filters:
        folders:
          - publications
        exclude_featured: false
    design:
      view: citation

  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - events
    design:
      view: card
---

