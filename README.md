# HTML Contact Form

A simple, semantic, accessible contact form built using plain HTML5.

This project was developed as part of the HTML Fundamentals learning path on [roadmap.sh](https://roadmap.sh/projects/contact-form), with a focus on form structure, labels, validation attributes, and proper grouping of form controls.

## Live Demo

[View the Live Contact Form](https://7amarah.github.io/html-contact-form/)

## Project Overview

The objective of this project is to build a real, accessible HTML form using only HTML, without CSS or JavaScript. The page is intentionally unstyled; styling is addressed in a later project.

There is no real backend. The form is wired up as if there were one, so a server inspecting the submission would receive exactly the expected name and value pairs. For demonstration, the form posts to [httpbin.org](https://httpbin.org/post), which echoes back the submitted data.

## Features

- A `<form>` element with a placeholder `action` URL and `method="post"`.
- A real `<label>` for every control, paired by `for` and `id` (or wrapped around the input).
- Full name field (`type="text"`, `required`).
- Email field (`type="email"`, `required`).
- Subject `<select>` with three options: General Inquiry, Technical Support and Feedback.
- Message `<textarea>` (`required`, with a `minlength` of 10).
- "How did you hear about us?" radio group inside a `<fieldset>` with a `<legend>`.
- Optional newsletter `<input type="checkbox">`.
- A `<button type="submit">` with clear text: "Send message".
- Head metadata: `<title>`, `<meta charset>`, `<meta viewport>`, SEO and Open Graph metadata.

## Form Fields

| Field                    | Element                     | `name`        | Required |
| ------------------------ | --------------------------- | ------------- | -------- |
| Name                     | `input type="text"`         | `fullName`    | Yes      |
| Email                    | `input type="email"`        | `email`       | Yes      |
| Subject                  | `select`                    | `subject`     | No       |
| Message                  | `textarea` (`minlength=10`) | `message`     | Yes      |
| How did you hear about us? | `input type="radio"` group | `hearAbout`   | No       |
| Product updates          | `input type="checkbox"`     | `newsletter`  | No       |

*Note: Browser validation is a UX layer, not a security boundary. A real server would still have to validate all submitted data on its own.*

## Technologies Used

- HTML5
- Semantic HTML
- HTML form controls and validation attributes
- SEO metadata
- Open Graph metadata

## Project Structure

```text
html-contact-form/
├── index.html
├── README.md
├── favicon.ico
├── favicon-16x16.png
├── favicon-32x32.png
├── apple-touch-icon.png
├── site.webmanifest
└── og-image.png
```

*Note: Some assets are optional and should only be included if they are present in the repository and referenced by the HTML document.*

## Getting Started

### Prerequisites

You only need:

- A web browser.
- A code editor (such as Visual Studio Code).
- Git (optional, for cloning the repository).

### Running Locally

1. Clone the repository:

   ```bash
   git clone git@github.com:7amarah/html-contact-form.git
   ```

2. Navigate into the project directory:

   ```bash
   cd html-contact-form
   ```

3. Open `index.html` directly in your browser.

Alternatively, open the project in Visual Studio Code and use the Live Server extension to preview the webpage.

No package installation, build process, or development server is required. Submitting the form requires an internet connection, since it posts to `httpbin.org`.

## Deployment

The project is hosted using GitHub Pages.

To deploy:

1. Push the project files to the `main` branch of the public GitHub repository.
2. Navigate to the repository's **Settings → Pages**.
3. Select **Deploy from a branch**.
4. Choose `main` and `/ (root)` as the deployment source.
5. Save the configuration.

GitHub Pages will publish the webpage.

## Learning Objectives

This project demonstrates an understanding of:

- Building a form with correct `action`, `method`, `name` and `value` attributes.
- Pairing labels and controls for accessibility.
- Grouping related controls with `<fieldset>` and `<legend>`.
- Using browser validation attributes (`required`, `minlength`, `type="email"`).
- Why client-side validation is not a substitute for server-side validation.
- Basic search engine optimisation and Open Graph metadata.
- Static website hosting using GitHub Pages.

## Author

**Tamarabrakaemi Waritimi**

- GitHub: [@7amarah](https://github.com/7amarah)
- LinkedIn: [Tamarah Waritimi](https://www.linkedin.com/in/tamarah-waritimi-4850bb111)