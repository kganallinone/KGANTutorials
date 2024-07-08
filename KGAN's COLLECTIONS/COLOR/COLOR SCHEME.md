# README

This README file outlines the usage of the color scheme in your project and provides examples of how to apply these colors using Tailwind CSS in your React components.

## Color Scheme

### Primary: `#a855f7`
- **Buttons**: Primary action buttons such as "Submit", "Save", or "Continue".
- **Headers**: Main headers or section titles.
- **Links**: Hyperlinks or call-to-action text.

```jsx
<button className="bg-primary text-white py-2 px-4 rounded">Submit</button>
```

### Secondary: `#f5f5f5`
- **Backgrounds**: General background color for sections or the entire page.
- **Cards**: Background of card components.
- **Forms**: Form backgrounds to differentiate from the main content area.

```jsx
<div className="bg-secondary p-4 rounded">Content here</div>
```

### Accent: `#15803d`
- **Highlight Text**: Important pieces of text that need emphasis.
- **Icons**: Accent icons to draw attention.
- **Borders**: Borders around components to make them stand out.

```jsx
<span className="text-accent">Highlighted Text</span>
```

### Dark: `#3E3F40`
- **Text**: Main body text color.
- **Navbar**: Background color for the navigation bar.
- **Footer**: Background color for the footer section.

```jsx
<nav className="bg-dark text-white p-4">Navbar Content</nav>
```

### Light: `#f5f5f5`
- **Backgrounds**: Background color for lighter sections.
- **Buttons**: Secondary or tertiary action buttons.
- **Form Inputs**: Background color for form input fields.

```jsx
<input type="text" className="bg-light p-2 rounded" placeholder="Enter text" />
```

### Neutral: `#6b7280`
- **Text**: Secondary text color.
- **Icons**: Neutral icons.
- **Borders**: Default border color for form inputs and other elements.

```jsx
<p className="text-neutral">Secondary Text</p>
```

### Success: `#15803d`
- **Alerts**: Success messages or notifications.
- **Badges**: Success badges or tags.
- **Buttons**: Success action buttons like "Complete" or "Approve".

```jsx
<div className="bg-success text-white p-2 rounded">Success Message</div>
```

### Warning: `#f59e0b`
- **Alerts**: Warning messages or notifications.
- **Badges**: Warning badges or tags.
- **Icons**: Warning icons.

```jsx
<div className="bg-warning text-white p-2 rounded">Warning Message</div>
```

### Danger: `#ef4444`
- **Alerts**: Error or danger messages.
- **Buttons**: Danger action buttons like "Delete" or "Remove".
- **Icons**: Danger icons.

```jsx
<div className="bg-danger text-white p-2 rounded">Error Message</div>
```

## Applying the Colors in Tailwind CSS

Here’s how you can define these colors in your Tailwind CSS configuration and use them in your components:

### Tailwind CSS Configuration

```js
// tailwind.config.js
module.exports = {
  theme: {
    extend: {
      colors: {
        primary: "#a855f7",
        secondary: "#f5f5f5",
        accent: "#15803d",
        dark: "#3E3F40",
        light: "#f5f5f5",
        neutral: "#6b7280",
        success: "#15803d",
        warning: "#f59e0b",
        danger: "#ef4444",
      },
    },
  },
};
```

### Using the Colors in React Components

```jsx
const MyComponent = () => (
  <div className="p-4">
    <h1 className="text-primary">Primary Header</h1>
    <button className="bg-primary text-white py-2 px-4 rounded">Primary Button</button>
    <div className="bg-secondary p-4 rounded">Secondary Background</div>
    <span className="text-accent">Accent Text</span>
    <nav className="bg-dark text-white p-4">Navbar Content</nav>
    <input type="text" className="bg-light p-2 rounded" placeholder="Enter text" />
    <p className="text-neutral">Neutral Text</p>
    <div className="bg-success text-white p-2 rounded">Success Message</div>
    <div className="bg-warning text-white p-2 rounded">Warning Message</div>
    <div className="bg-danger text-white p-2 rounded">Error Message</div>
  </div>
);

export default MyComponent;
```
