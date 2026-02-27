name: Project
description: Larger multi-step effort for MA3D Prints
title: "[Project] "
labels: ["project"]
body:
  - type: textarea
    id: goal
    attributes:
      label: Goal
      description: What are we trying to achieve?
      placeholder: "Improve local lead conversions from the website."
    validations:
      required: true
  - type: textarea
    id: outcome
    attributes:
      label: Success criteria
      description: How will we know this is done / working?
      placeholder: "Contact form submissions have all needed info and I can quote within one email."
    validations:
      required: false
  - type: textarea
    id: breakdown
    attributes:
      label: Breakdown / checklist
      description: Break this into smaller tasks or checklist items.
      placeholder: |
        - Update contact form fields
        - Add local-focused homepage copy
        - Create canned email replies
    validations:
      required: false
  - type: dropdown
    id: area
    attributes:
      label: Area
      options:
        - Website
        - Marketing
        - Operations
        - Customer Work
        - Finance
    validations:
      required: false
