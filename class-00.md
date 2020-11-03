# SMACCS and responsive web design

## Responsive Web Design

- the practice of building a website suitable to work on every device and every screen size
  - Flexible layout
  - media queries
  - flexible media


### Responsive vs. Adaptave vs Mobile

- responsive means to react quickly and positively to any change

- adaptive means to be easily modified for a new purpose

- mobile is more to build a seperate domain for the mobile devices

## Flexible Layouts

### *Key to finding dimensions for elements* 

- target % context(container) = result


## Media Queries

- built as an etension to media types commonly found when targeting and includes styles

- initailizing media queries
  - `<link href="styles.css" rel="stylesheet" media="all and (max-width: 1024px)">` seperates css
` 
  - inside css
    - `@media all and (max-width: 1024px) {...}` media rule
    - `@import "reset.css";`import rule

- many different types of queries

  - ands work
  - oreintation


  design for moble first


  ##SMACSS

  >Style
  - normalize.css
    - new defaults
  - base.css
    - `<main>`
    - `<body>`
    - box sizing
    - font
    - background color
  - layout.css
    - positioning
    - class and id targeting
  - modules.css
    - reusable markup 
    - list item
    - images
  - state.css
    - hovers
    - click
    - mouse over
    - etc
    - focus
  - theme.css
    - colors
    - fonts
    - temp changes
