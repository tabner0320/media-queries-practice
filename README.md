# Responsive Web Design – Media Queries Practice

A responsive web design practice project built with **HTML5** and **CSS3**.

This project demonstrates how CSS media queries, Flexbox, and CSS Grid can be used to create layouts that adapt to different screen sizes, including desktop, tablet, mobile, and small mobile devices.

## Live Demo

[View the Live Website](https://tabner0320.github.io/media-queries-practice/)

## Features

- Responsive navigation
- Responsive hero section
- Multi-column desktop layout
- Two-column tablet layout
- Single-column mobile layout
- CSS Grid
- Flexbox
- CSS media queries
- Responsive typography
- Mobile-friendly spacing
- Semantic HTML structure
- Sticky navigation header
- Smooth scrolling
- Responsive cards and content sections

## Technologies Used

| Technology | Purpose |
| --- | --- |
| HTML5 | Page structure and semantic content |
| CSS3 | Styling and responsive design |
| Flexbox | Navigation and layout alignment |
| CSS Grid | Responsive card layouts |
| Media Queries | Adapting the layout to different screen sizes |
| Git | Version control |
| GitHub | Source code hosting |
| GitHub Pages | Website deployment |

## Responsive Breakpoints

The project uses several breakpoints to adjust the layout depending on the width of the browser.

### Desktop

**1024px and above**

The desktop layout uses the available horizontal space to display content in multiple columns.

### Tablet

**768px – 1023px**

The tablet layout reduces the card grids from three columns to two columns and adjusts the overall layout for medium-sized screens.

```css
@media (max-width: 1023px) {
  .card-grid,
  .breakpoint-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}
```

### Mobile

**Below 768px**

The mobile layout stacks the navigation and content vertically and changes the card grids to a single column.

```css
@media (max-width: 767px) {
  .site-nav {
    flex-direction: column;
  }

  .card-grid,
  .breakpoint-grid {
    grid-template-columns: 1fr;
  }
}
```

### Small Mobile

**Below 480px**

Additional adjustments are made to typography, padding, and spacing for smaller mobile screens.

```css
@media (max-width: 480px) {
  .container {
    width: 92%;
  }

  .hero h2 {
    font-size: 2rem;
  }

  .hero p {
    font-size: 1rem;
  }
}
```

## Project Structure

```text
media-queries-practice/
│
├── css/
│   └── style.css
│
├── index.html
├── notes.md
└── README.md
```

## What I Practiced

Through this project, I practiced:

- Creating responsive layouts with CSS media queries
- Using CSS Grid for responsive card layouts
- Using Flexbox for navigation and alignment
- Creating desktop, tablet, and mobile layouts
- Designing mobile-friendly interfaces
- Creating reusable CSS classes
- Working with responsive typography
- Using semantic HTML elements
- Testing websites at different browser widths
- Using Chrome Developer Tools responsive mode
- Managing source code with Git and GitHub
- Deploying a static website with GitHub Pages

## How It Works

The website uses a desktop-first responsive design.

The default CSS displays the content in a larger desktop layout. Media queries then detect when the browser width becomes smaller and modify the layout.

For example, the desktop card layout uses three columns:

```css
.card-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 1.5rem;
}
```

At tablet widths, the layout changes to two columns:

```css
@media (max-width: 1023px) {
  .card-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}
```

At mobile widths, the layout changes to one column:

```css
@media (max-width: 767px) {
  .card-grid {
    grid-template-columns: 1fr;
  }
}
```

This allows the same website to provide a readable and usable layout across different screen sizes.

## Responsive Testing

The project was tested using Chrome Developer Tools at several browser widths:

| Width | Layout |
| --- | --- |
| 1200px | Desktop |
| 900px | Tablet |
| 600px | Mobile |
| 375px | Small Mobile |

These tests demonstrate how the CSS media queries respond as the available screen width changes.

## Running the Project Locally

Clone the repository:

```bash
git clone https://github.com/tabner0320/media-queries-practice.git
```

Navigate into the project:

```bash
cd media-queries-practice
```

Open `index.html` directly in a browser or use the **Live Server** extension in Visual Studio Code.

## Repository

[View the Source Code on GitHub](https://github.com/tabner0320/media-queries-practice)

## Author

**Theophilus M. Abner Jr.**

Software Developer and IT Professional focused on **C#, .NET, web development, responsive design, APIs, cloud technologies, and software development**.