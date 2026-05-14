# Accessible Interactive Photo Gallery

This project is an accessible and interactive photo gallery created using HTML, CSS, and JavaScript.  
The gallery supports mouse and keyboard interaction and follows accessibility best practices.

## Live Website

https://sibhi.github.io/accessible-photo-gallery/

## GitHub Repository

https://github.com/sibhi/accessible-photo-gallery

---

## Features

- Interactive image gallery
- Mouse hover support
- Keyboard accessibility using `tabindex`
- `onfocus` and `onblur` event handling
- `onmouseover` and `onmouseleave` event handling
- Page load event support
- Accessible alternative text for all images
- Responsive layout
- W3C validated HTML
- Tested using WAVE and aXe accessibility tools

---

## Technologies Used

- HTML5
- CSS3
- JavaScript

---

## Accessibility Improvements

The following accessibility features were added:

- Added meaningful `alt` text for all images
- Added keyboard navigation using `tabindex`
- Added focus and blur event listeners
- Maintained proper heading order
- Added page title element
- Tested using:
  - W3C Validator
  - WAVE Accessibility Tool
  - aXe Accessibility Extension

---

## JavaScript Functionality

The project includes:

- `onmouseover`
- `onmouseleave`
- `onfocus`
- `onblur`
- `onload`

events for interactive image previews.

A loop is used to automatically add `tabindex="0"` to all figure elements for keyboard navigation.

Example:

```javascript
window.onload = function () {
    let figures = document.querySelectorAll("figure");

    for (let i = 0; i < figures.length; i++) {
        figures[i].setAttribute("tabindex", "0");
        console.log("Tabindex added");
    }
};
