---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: features
    content:
      title: Skills
      items:
        - name: Python
          description: 90%
          icon: python
          icon_pack: fab
        - name: DeepLearning
          description: 70%
          icon: deeplearning
          icon_pack: fab
        - name: Photography
          description: 50%
          icon: camera-retro
          icon_pack: fas
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-formciat
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Remote Sensing Geologist
          company: NHAZCA Srl
          company_url: ''
          company_logo: org-gc
          location: Italy
          date_start: '2018-10-01'
          date_end: '2019-01-01'
          description: |2-
              Responsibilities include:

              * Beta-testing activities of proprietary software for the processing of data acquired through TInSAR technique and semi-automatic tools for data post-processing.
              * Photointerpretation and displacement analysis using satellite optical (Pleiades, Sentinel-2, Aster, Landsat) and SAR (Sentinal-1, COSMOSkyMed) data and terrestrial optical and GBSAR data.
              * Realization of multiple 3D point clouds using photogrammetry technique using airborne and terrestrial images for 3D modeling and for change detection analysis.
        - title: Field Geologist
          company: Self Employed
          company_url: ''
          company_logo: org-x
          location: Italy
          date_start: '2014-04-01'
          date_end: '2018-05-01'
          description: |2-
              Performed several field activities, including:

              * Gravimetric and Microgravimetric survey using LaCoste & Romberg gravimeter.
              * Magnetometric surveys using the Profiler EMP400.
              * Geoelectrical profiling surveys up to AB-1000.
              * Seismic surveys (MASW, Down-Hole, TROMINO
        - title: ESA Analog 1 - MIRACLES 2022
          company: Jacobs University Bremen
          company_url: ''
          company_logo: org-x
          location: Italy
          date_start: '2022-06-22'
          date_end: '2022-06-30'
          description: |2-
              Part of the geologists team who prepared and supported the sample collection of the Interact rover field operations.
    design:
      columns: '2'
  
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: DeepLandforms
          tag: DeepLandforms
        - name: EXPLORE L-HEX & L-EXPLO
          tag: EXPLORE
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  

---
