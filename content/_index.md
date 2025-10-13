---
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
        I’m a PhD researcher in physical oceanography at the University of Cambridge (Department of Earth Sciences, Darwin College). My work focuses on Southern Ocean and Atlantic water-mass dynamics and overturning, with particular interest in Antarctic Bottom Water (AABW), Circumpolar Deep Water (CDW), and shelf processes in the Bellingshausen Sea near the Antarctic Peninsula.

        Methodologically, I combine observations (GO-SHIP, GLODAP, Argo, autonomous gliders), inverse methods (OMP via *pyompa*), and machine learning (ensemble/random forests) to classify water masses and map their variability. I also work with data-assimilating and high-resolution models (ECCO/MITgcm), interpolating temperature–salinity onto neutral density surfaces to study decadal change and uncertainty.

        I build open, reproducible Python workflows (xarray, dask, scikit-learn, Cartopy) on HPC systems (CSD3) and maintain tooling for large NetCDF/Zarr datasets and glider QC/calibration. Current projects include classifying Atlantic water masses from OMP-derived fractions, assessing CDW’s poleward migration, and evaluating implications for AABW contraction and shelf–ice interactions.

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
        - **Classification & mapping:** Training ensemble/random-forest models on OMP-classified fractions to apply water-mass labels to Argo and model fields.  
        - **Observations + models:** Integrating GO-SHIP/GLODAP/Argo with ECCO and MITgcm; interpolating onto neutral-density surfaces for consistent analysis.  
        - **Uncertainty:** Propagating ensemble/model variance under the “sum-to-one” constraint for water-mass fractions; diagnosing spatial discontinuities.  
        - **Gliders:** Cross-over calibration/QC and workflow tooling for Slocum/Seaglider missions on the Antarctic shelf.

        I prioritise open, reproducible code and careful uncertainty quantification.
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

  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: blog
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ''
        category: ''
        tag: ''
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ''
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: card
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]

  - block: cta-card
    content:
      title: 'Work with me'
      text: |-
        I’m always happy to discuss collaborations on Southern Ocean water masses, machine-learning classification, and glider workflows.  
        For code and datasets, see my GitHub, or drop me an email.
      button:
        text: Contact
        url: mailto:your@email.here
    design:
      card:
        css_class: 'bg-primary-300'
        css_style: ''
---

