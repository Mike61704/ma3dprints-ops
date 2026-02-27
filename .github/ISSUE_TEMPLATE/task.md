name: Task
description: A single actionable task for MA3D Prints
title: "[Task] "
labels: ["task"]
body:
  - type: textarea
    id: summary
    attributes:
      label: Summary
      description: Short, clear description of what needs to be done.
      placeholder: "Update GoDaddy contact form fields"
    validations:
      required: true
  - type: textarea
    id: steps
    attributes:
      label: Steps
      description: Bullet list of steps if needed.
      placeholder: |
        - Open GoDaddy Website Builder
        - Update form fields to match spec
        - Test with a sample submission
    validations:
      required: false
  - type: dropdown
    id: area
    attributes:
      label: Area
      description: What part of the business is this for?
      options:
        - Website
        - Marketing
        - Operations
        - Customer Work
        - Finance
    validations:
      required: false
  - type: input
    id: estimate
    attributes:
      label: Time estimate
      description: Rough guess (e.g. 15m, 1h, 2h)
      placeholder: "30m"
    validations:
      required: false
