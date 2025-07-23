---
name: Work Hours issue template
about: For work Hours
title: ''
labels: ''
assignees: ''

---

name: Log Work Hours
description: Log daily work hours for a project
title: "Work Hours: [Employee Name] [Date]"
labels: ["work-hours"]
body:
  - type: dropdown
    id: project
    attributes:
      label: Project
      description: Select the project you worked on
      options:
        - PROJ001: Website Development
        - PROJ002: Mobile App
        - PROJ003: Database Optimization
        - PROJ004: Testing & QA
        - PROJ005: Client Support
      multiple: false
    validations:
      required: true
  - type: dropdown
    id: hours
    attributes:
      label: Hours Worked
      description: Select hours worked today
      options:
        - "1.0"
        - "1.5"
        - "2.0"
        - "2.5"
        - "3.0"
        - "3.5"
        - "4.0"
        - "4.5"
        - "5.0"
        - "5.5"
        - "6.0"
        - "6.5"
        - "7.0"
        - "7.5"
        - "8.0"
      multiple: false
    validations:
      required: true
  - type: textarea
    id: comments
    attributes:
      label: Work Description
      description: Brief description of work completed
      placeholder: "Worked on login feature, fixed 3 bugs, attended team meeting"
