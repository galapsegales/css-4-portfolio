# Adam Keyes Portfolio

## Description

A modern and responsive front-end developer portfolio website showcasing professional skills, experience, and projects. The site features a clean design with a hero section, skills showcase, project gallery, and a contact form. Built with a mobile-first approach and fully responsive across all devices.

## Technologies Used

- **HTML5** - Semantic markup structure
- **Sass/SCSS** - CSS preprocessor for modular and maintainable styles
- **Vite** - Fast build tool and development server
- **JavaScript (ES6+)** - For form validation and interactivity
- **BEM Methodology** - CSS naming convention for component-based architecture
- **Git & GitHub Pages** - Version control and deployment

## Getting Started

1. Clone the repository
2. Run `npm install` to install dependencies
3. Run `npm run dev` to start the development server
4. Run `npm run build` to create a production build

## BEM Structure

This project follows the **BEM (Block Element Modifier)** methodology for CSS class naming, ensuring a scalable and maintainable codebase.

### BEM Architecture Breakdown

**Blocks** represent standalone components:
- `.header` - Navigation and branding section
- `.hero` - Main landing area with introduction
- `.features` - Skills and experience showcase
- `.projects` - Portfolio projects gallery
- `.project` - Individual project card
- `.footer` - Contact form and footer navigation
- `.btn` - Reusable button component

**Elements** are parts of blocks, denoted by double underscores (`__`):
- `.header__nav` - Navigation container within header
- `.header__nav--logo` - Logo element
- `.header__nav--social` - Social media links container
- `.hero__img` - Hero image container
- `.hero__content` - Hero text content wrapper
- `.hero__content--title` - Hero main heading
- `.hero__content--subtitle` - Hero description text
- `.hero__content--btn` - Hero call-to-action button
- `.features__item` - Individual skill item
- `.features__item--title` - Skill name
- `.features__item--description` - Years of experience
- `.project__img` - Project thumbnail
- `.project__img-overlay` - Hover overlay for projects
- `.project__img--cta` - Project call-to-action buttons
- `.project--title` - Project name
- `.project--tech` - Technology tags container
- `.footer__contact` - Contact section content
- `.footer__form` - Contact form container
- `.footer__form--group` - Form input groups

**Modifiers** alter the appearance or behavior of blocks/elements (using `--`):
- `.br-tablet` - Line break visible only on tablet breakpoint
- `.br-tablethorizontal` - Line break for tablet horizontal orientation
- `.underline` - Text decoration modifier

### SCSS File Structure

The stylesheets follow a modular architecture using the 7-1 pattern:

```
src/styles/
├── main.scss              # Main import file
├── abstracts/
│   ├── _mixins.scss       # Reusable mixins (breakpoints, image switchers)
│   └── _variables.scss    # Color, typography, and breakpoint variables
├── base/
│   ├── _base.scss         # Base styles and HTML elements
│   ├── _reset.scss        # CSS reset
│   └── _typography.scss   # Font definitions and text styles
├── components/
│   └── _buttons.scss      # Button component styles
├── layout/
│   ├── _container.scss    # Layout containers and wrappers
│   ├── _features.scss     # Skills section layout
│   ├── _footer.scss       # Footer layout and form styles
│   ├── _header.scss       # Header and navigation layout
│   ├── _hero.scss         # Hero section layout
│   └── _projects.scss     # Projects gallery layout
├── pages/
│   └── _home.scss         # Home page specific styles
├── themes/
│   └── _default.scss      # Theme variables and colors
└── vendors/
    └── _vendors.scss      # Third-party styles
```

### BEM Naming Examples in This Project

**Header Navigation:**
```scss
.header {
  &__nav { } // Block__Element
    &--logo { } // Block__Element--Modifier
    &--social { } // Block__Element--Modifier
}
```

**Hero Section:**
```scss
.hero {
  &__img { } // Block__Element
  &__content { } // Block__Element
    &--title { } // Block__Element--Modifier
    &--subtitle { } // Block__Element--Modifier
    &--btn { } // Block__Element--Modifier
}
```

**Projects Gallery:**
```scss
.projects {
  &__header { } // Block__Element
    &--title { } // Block__Element--Modifier
    &--btn { } // Block__Element--Modifier
}

.project {
  &__img { } // Block__Element
    &-overlay { } // Block__Element-variant
    &--cta { } // Block__Element--Modifier
  &--title { } // Block--Modifier
  &--tech { } // Block--Modifier
    &-name { } // Block--Modifier-element
}
```

## Author

**Gala P Segales**
