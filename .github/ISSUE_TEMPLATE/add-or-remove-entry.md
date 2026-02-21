---
name: Add or Remove Entry
about: Request a change to the Gist
title: ''
labels: ''
assignees: ''

---

name: Add or Remove Entry
description: Request a change to the Gist
title: "[Request]: "
labels: ["gist-request"]

body:
  - type: dropdown
    id: action
    attributes:
      label: What do you want to do?
      options:
        - Add
        - Remove
    validations:
      required: true

  - type: input
    id: entry
    attributes:
      label: Entry
      description: What should be added or removed?
    validations:
      required: true

  - type: textarea
    id: reason
    attributes:
      label: Reason
      description: Optional explanation
