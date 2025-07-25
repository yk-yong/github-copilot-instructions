---
applyTo: '**/*.{tsx,html}'
---
Provide project context and coding guidelines that AI should follow when generating code, answering questions, or reviewing changes.

# General Guidelines for HTML tags
This is a set of general guidelines for HTML tags that should be followed in the most cases. These guidelines are not exhaustive and may not cover every possible scenario, but they provide a solid foundation for writing clean, maintainable HTML code.

## General Guidelines
- Use semantic HTML tags to improve accessibility and SEO.
- Use lowercase for all HTML tags and attributes, as per HTML5 standards (This is not applicable for JSX).
- Use hyphens for class names and IDs (e.g., `my-class`, `my-id`).
- Use kebab-case for file names (e.g., `my-component.tsx`, `my-style.css`).
- Use camelCase for JavaScript variables and functions (e.g., `myVariable`, `myFunction`).
- Use PascalCase for React component names (e.g., `MyComponent`, `UserProfile`).
- Use meaningful names for classes and IDs that describe the purpose of the element (e.g., `header`, `footer`, `main-content`).
- Use double quotes for attribute values.
- Use self-closing tags for void elements (e.g., `<img />`, `<br />`, `<hr />`).
- Use indentation for nested elements to improve readability.
- Use comments to explain complex or non-obvious code.
- Use meaningful class names that describe the purpose of the element.
- Use IDs sparingly and only when necessary for JavaScript or CSS targeting.
- Use the `lang` attribute on the `<html>` tag to specify the language of the document (e.g., `<html lang="en">`).
- Use the `charset` attribute in the `<meta>` tag to specify the character encoding (e.g., `<meta charset="UTF-8">`).
- Use the `viewport` meta tag to control the layout on mobile devices (e.g., `<meta name="viewport" content="width=device-width, initial-scale=1.0">`).
- Use the `title` attribute on links to provide additional context.
- Use the `alt` attribute on images to provide alternative text for accessibility.
- Use the `aria-*` attributes to enhance accessibility for screen readers.
- Use the `data-*` attributes for custom data that needs to be accessed via JavaScript.
- Use the `role` attribute to define the role of an element when necessary.
- Use the `tabindex` attribute to control keyboard navigation when necessary.
- Use the `rel` attribute on links to specify the relationship between the current document and the linked document.
- Use the `target` attribute on links to specify where to open the linked document (e.g., `_blank` for a new tab).
- Use the `style` attribute sparingly and prefer external CSS for styling.
- Use the `script` tag with the `defer` attribute to load JavaScript files asynchronously.
- Use the `noscript` tag to provide fallback content for users with JavaScript disabled.
- Use the `meta` tag to provide metadata about the document (e.g., charset, viewport, description).
- Use the `link` tag to include external stylesheets and icons.
- Use the `form` tag to create forms and include appropriate input types.
- Use the `label` tag to associate labels with form controls for better accessibility.
- Use the `fieldset` and `legend` tags to group related form controls and provide context.
- Use the `button` tag for clickable buttons and specify the `type` attribute (e.g., `submit`, `reset`, `button`).

## MUST NOT DO

- Do not use inline styles; prefer external CSS files for styling.
- Do not use deprecated HTML tags or attributes (e.g., `<font>`, `<center>`, `<b>`).
- Do not use non-semantic tags (e.g., `<div>`, `<span>`) when a semantic tag is available (e.g., `<header>`, `<footer>`, `<article>`, `<section>`).
- Do not use IDs for styling; use classes instead.
- Do not use empty tags without content (e.g., `<div></div>`); if a tag is not needed, remove it.
- Do not use excessive nesting of elements; keep the HTML structure flat and simple.
- Do not use inline JavaScript; prefer external scripts or event listeners.
- Do not use the `style` attribute for layout; use CSS for layout and positioning.
- Do not use the `onclick` attribute for event handling; use JavaScript event listeners instead.
- Do not use the `target="_blank"` attribute without the `rel="noopener noreferrer"` attribute for security reasons.
- Do not use the `style` attribute for styling; prefer external CSS files or CSS-in-JS solutions.
- Do not use the `script` tag in the `<head>` section without the `defer` or `async` attribute; this can block rendering.
- Do not use the `noscript` tag to hide content; it should only be used to provide fallback content for users with JavaScript disabled.
- Do not use the `meta` tag for styling or layout purposes; it should only be used for metadata.
- Do not use the `link` tag for JavaScript files; use the `script` tag instead.
- Do not use the `form` tag without specifying the `action` and `method` attributes; this can lead to unexpected behavior.
- Do not use the `label` tag without associating it with a form control using the `for` attribute; this can lead to accessibility issues.
- Do not use the `fieldset` and `legend` tags without grouping related form controls; this can lead to confusion for users.
- Do not use the `button` tag without specifying the `type` attribute; this can lead to unexpected behavior (e.g., a button acting as a submit button without intention).
- Do not use the `data-*` attributes for styling or layout purposes; they should only be used for custom data that needs to be accessed via JavaScript.
- Do not use the `role` attribute unnecessarily; it should only be used to enhance accessibility when the semantic meaning of an element is not clear.
- Do not use the `tabindex` attribute unnecessarily; it should only be used to control keyboard navigation when necessary.
- Do not use the `rel` attribute on links without specifying the relationship; this can lead to confusion for users and search engines.
- Do not use the `target` attribute on links without considering the user experience; opening links in a new tab can be disruptive if not done thoughtfully.
- Do not use the `alt` attribute on images without providing meaningful alternative text; this can lead to accessibility issues for users with visual impairments.
- Do not use the `aria-*` attributes unnecessarily; they should only be used to enhance accessibility when the semantic meaning of an element is not clear.
- Do not use the `lang` attribute on the `<html>` tag without specifying the correct language; this can lead to accessibility issues for users with screen readers.
- Do not use the `charset` attribute in the `<meta>` tag without specifying the correct character encoding; this can lead to rendering issues in different browsers.
- Do not use the `viewport` meta tag without considering the layout on mobile devices; this can lead to poor user experience on smaller screens.
- Do not use the `title` attribute on links without providing meaningful context; this can lead to confusion for users and search engines.