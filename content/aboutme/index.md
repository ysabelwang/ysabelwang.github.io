---
# Show the page's date?
show_date: false

# Show social sharing links?
share: false

type: landing

sections:
  - block: markdown
    id: aboutme
    text: Test text
    #(will update) I was born and raised in the Philippines. In 2018, I graduated from the National Institute of Physics of the University of the Philippines Diliman with a BS in Physics. After this, I worked for 3 years at the Marine Science Institute as a research associate in the Physical Oceanography Laboratory, led by Cesar Villanoy.\nIn 2021, I moved to the US to start my MS Oceanography program at Texas A&M University with Steve DiMarco as my adviser. I graduated in August of 2023.\nIn the fall of 2023, I started my PhD in Physical Oceanography at the MIT-WHOI Joint Program with Magdalena Andres and Glen Gawarkiewicz as my advisers.\n\nOutside of school and research, I enjoy playing the guitar, powerlifting, reading, video games, and the occasional pro-wrestling show. I also enjoy elaborate methods of preparing my coffee.

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
            # description: Taught electronic engineering and researched semiconductor physics.
          - title: BS in Physics
            company: University of the Philippines Diliman
            company_url: ''
            company_logo: up-logo
            location: Quezon City, Philippines
            date_start: '2013-06-01'
            date_end: '2018-06-30'
            # description: Taught electronic engineering and researched semiconductor physics.
      design:
        columns: '2'

---




