# EiconPicker Integration Guide

## Overview

This document provides instructions for integrating and using **EiconPicker** in your web project. EiconPicker is a tool for selecting icons in an input field.

![Preview Image](https://github.com/junaidzx90/eiconpicker/blob/main/preview.png?raw=true)

## Prerequisites

Ensure you have the following files available in your project:

- `jquery-3.6.0.min.js` (local jQuery library)

## Steps for Integration

### 1. Create Container

Add our `<e-iconpicker>` container element in your HTML where the EiconPicker fields will be rendered:

```html
<e-iconpicker theme="light" selected="fa-telegram" class="iconpic"></e-iconpicker>
```

### 2. Include JavaScript Libraries

Add the following script tag before the closing `</body>` tag of your HTML:

```html
<script src="https://cdn.jsdelivr.net/gh/junaidzx90/eiconpicker@v1.0.0/eiconpicker.min.js"></script>
```

### 3. Handling Events

To capture icon changes, use the following JavaScript code:

```javascript
$('.iconpic').on("change", handleChange);

function handleChange(event) {
    const selectedIcon = event.originalEvent.detail;
    console.log(selectedIcon);
}
```

## Customization

You can customize the options by adding the following attributes in the `<e-iconpicker>` tag:

- **theme**: `light`, `dark`  
  Default: `light`
- **selected**: Use this attribute to set a default selected icon.
- **class**: Use this attribute to add your own custom class.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For support or questions, please [contact me](mailto:contact@easeare.com).