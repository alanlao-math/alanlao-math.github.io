---
# Leave the homepage title empty to use the site title
title: ''
summary: ''
date: 2022-10-24
type: landing

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: me

      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
      headings:
        about: 'Professional Summary'
        education: 'Education'
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
      title: 'Resume'
      subtitle: ''
      text: |-
        <div class="not-prose mb-4">
          <a href="/uploads/resume.pdf" target="_blank" rel="noopener" class="inline-flex items-center rounded-md bg-primary-600 px-4 py-2 text-sm font-medium text-white no-underline hover:bg-primary-700">
            Open full CV / Resume
          </a>
        </div>

        <iframe src="/uploads/resume.pdf" title="Alan Hin Lon Lao resume" width="100%" height="900" style="border:0; border-radius:0.75rem; background:#f8fafc;"></iframe>
    design:
      columns: '1'

  - block: markdown
    content:
      title: 'Research'
      subtitle: ''
      text: |-
        I am a mathematician working in combinatorics, with a focus on matroid theory and geometric lattice theory. My research explores the structural and algebraic properties that connect these areas and informs problems in discrete geometry and enumeration.

        I’m especially interested in how combinatorial objects can reveal deeper patterns across mathematics, and I welcome collaboration with researchers working at the intersection of algebra, geometry, and combinatorics.
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
