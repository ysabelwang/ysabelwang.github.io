---
# Leave the homepage title empty to use the site title
title: ''
date: 2022-10-24
type: landing
  

sections:
  - block: about.biography
    id: about
    content:
      title: ''
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
    design:
      columns: '2'
      background:
        image:
          filename: footer_bio_new.png
  - block: experience
    id: education
    content:
      title: Education
      # Date format for experience
      #   Refer to https://docs.hugoblox.com/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: PhD in Physical Oceanography
          company: Massachusetts Institute of Technology, Woods Hole Oceanographic Institution
          company_url: ''
          company_logo: mit-logo
          location: Cambridge, MA and Woods Hole, MA
          date_start: '2023-09-01'
          date_end: ''
          # description: |2-
          #     Responsibilities include:

          #     * Analysing
          #     * Modelling
          #     * Deploying
        - title: MS in Oceanography
          company: Texas A&M University
          company_url: ''
          company_logo: tamu-logo
          location: College Station, Texas
          date_start: '2021-08-31'
          date_end: '2023-08-10'
          description: MS Thesis entitled "Formation and Fate of a Coastal Dense Water Mass$:$ The 2021 Texas Winter Storms" 
          # description: Taught electronic engineering and researched semiconductor physics.
        - title: BS in Physics
          company: University of the Philippines Diliman
          company_url: ''
          company_logo: up-logo
          location: Quezon City, Philippines
          date_start: '2013-06-01'
          date_end: '2018-06-30'
          description: BS Thesis entitled "Highly secure optical encryption using multiple diffuser phase retrieval and chaos phase masks"
          # description: Taught electronic engineering and researched semiconductor physics.
    design:
      columns: '1'
  # - block: skills
  #   id: skills
  #   content:
  #     title: Technical expertise
  #     text: '<p style="font-family: avenir;text-align: left;font-size: 15pt">All of the work that I do requires different programming languages and methods. These represent the level of familiarity and comfortability I have with each item.</p>'
  #     # Choose a user to display skills from (a folder name within `content/authors/`)
  #     username: admin
  #     design:
  #       columns: '1'
  #   design:
  #     columns: '1'
  #     # spacing:
  #     #   # Customize the section spacing. Order is top, right, bottom, left.
  #     #   padding: ['40px', '80px', '20px', '0']
  # - block: accomplishments
  #   content:
  #     # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
  #     title: 'Accomplish&shy;ments'
  #     subtitle:
  #     # Date format: https://docs.hugoblox.com/customization/#date-format
  #     date_format: Jan 2006
  #     # Accomplishments.
  #     #   Add/remove as many `item` blocks below as you like.
  #     #   `title`, `organization`, and `date_start` are the required parameters.
  #     #   Leave other parameters empty if not required.
  #     #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
  #     items:
  #       - certificate_url: https://www.coursera.org
  #         date_end: ''
  #         date_start: '2021-01-25'
  #         description: ''
  #         icon: coursera
  #         organization: Coursera
  #         organization_url: https://www.coursera.org
  #         title: Neural Networks and Deep Learning
  #         url: ''
  #       - certificate_url: https://www.edx.org
  #         date_end: ''
  #         date_start: '2021-01-01'
  #         description: Formulated informed blockchain models, hypotheses, and use cases.
  #         icon: edx
  #         organization: edX
  #         organization_url: https://www.edx.org
  #         title: Blockchain Fundamentals
  #         url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
  #       - certificate_url: https://www.datacamp.com
  #         date_end: '2020-12-21'
  #         date_start: '2020-07-01'
  #         description: ''
  #         icon: datacamp
  #         organization: DataCamp
  #         organization_url: https://www.datacamp.com
  #         title: 'Object-Oriented Programming in R'
  #         url: ''
  #   design:
  #     columns: '2'
  - block: portfolio
    id: research
    content:
      title: Research
      subtitle: 'This is a list of my current and some past research topics.'
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - research
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
      view: compact
      columns: '2'
      background:
        image:
          filename: footer_bio_new.png
  # - block: portfolio
  #   id: projects
  #   content:
  #     title: Projects
  #     filters:
  #       folders:
  #         - project
  #     # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
  #     default_button_index: 0
  #     # Filter toolbar (optional).
  #     # Add or remove as many filters (`filter_button` instances) as you like.
  #     # To show all items, set `tag` to "*".
  #     # To filter by a specific tag, set `tag` to an existing tag name.
  #     # To remove the toolbar, delete the entire `filter_button` block.
  #     buttons:
  #       - name: All
  #         tag: '*'
  #       - name: Deep Learning
  #         tag: Deep Learning
  #       - name: Other
  #         tag: Demo
  #   design:
  #     # Choose how many columns the section has. Valid values: '1' or '2'.
  #     columns: '1'
  #     view: showcase
  #     # For Showcase view, flip alternate rows?
  #     flip_alt_rows: false
  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        folders:
          - publication
        featured_only: false
    design:
      columns: '2'
      view: compact
  # - block: collection
  #   content:
  #     title: Recent Publications
  #     text: |-
  #       {{% callout note %}}
  #       Quickly discover relevant content by [filtering publications](./publication/).
  #       {{% /callout %}}
  #     filters:
  #       folders:
  #         - publication
  #       exclude_featured: true
  #   design:
  #     columns: '2'
  #     view: citation
  - block: collection
    id: conferences
    content:
      title: Conference Presentations
      filters:
        folders:
          - conferences
    design:
      columns: '2'
      view: compact
      background:
        image:
          filename: footer_bio_new.png
  # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'
  - block: markdown
    content:
      title: ''
      subtitle: ''
      text: |-
        {{< gallery album="pictures" >}}
    design:
      columns: '1'
      view: compact
      
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle: You can reach me through these links.
      # text: |-
      #   Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis ut magna et, vehicula efficitur enim.
      # # Contact (add or remove contact options as necessary)
      # email: ysabel@mit.edu
      contact_links:
        - icon: envelope
          icon_pack: fas
          name: E-mail me
          link: mailto:ysabel@mit.edu
        - icon: linkedin
          icon_pack: fab
          color: '#0e2841'
          link: https://www.linkedin.com/in/ysabelwang
          name: LinkedIn
        - icon: google-scholar
          icon_pack: ai
          color: '#0e2841'
          link: https://scholar.google.com/citations?user=UfLz5uEAAAAJ&hl=en
          name: Google Scholar
        - icon: orcid
          icon_pack: ai
          label: ORCID
          link: https://orcid.org/0000-0001-5862-5204
          name: ORCID
      # phone: 888 888 88 88
      # appointment_url: 'https://calendly.com'
      # address:
      #   street: 450 Serra Mall
      #   city: Stanford
      #   region: CA
      #   postcode: '94305'
      #   country: United States
      #   country_code: US
      # directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      # office_hours:
      #   - 'Monday 10:00 to 13:00'
      #   - 'Wednesday 09:00 to 10:00'
      # # Choose a map provider in `params.yaml` to show a map from these coordinates
      # coordinates:
      #   latitude: '37.4275'
      #   longitude: '-122.1697'  
    
        
      # Automatically link email and phone or display as text?
      autolink: false
      # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: false
    design:
      columns: '2'
      background:
        image:
          filename: footer_bio_new.png
---
