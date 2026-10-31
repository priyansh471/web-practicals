# Practical 1.5 - Accessible Personal Profile Page

## 1. Title
Accessible Personal Profile Page

## 2. Aim
To build and review a structured personal profile page that follows basic web accessibility practices.

## 3. Tools Used
- Notepad / VS Code (text editor)
- Google Chrome (browser)
- Chrome DevTools Lighthouse (accessibility check)
- Git and GitHub (to upload the practical)

## 4. Theory
Web accessibility means building pages that everyone can use, including people who use screen readers, a keyboard only, or have low vision. Accessible pages are also easier for everyone else to use.

Accessibility features used in this practical:

| Feature | Purpose |
|---|---|
| `lang="en"` on `<html>` | Tells screen readers which language to speak |
| Skip link (`Skip to main content`) | Lets keyboard users jump past the navigation |
| One `<h1>` and headings in order (h1, h2, h3) | Gives a clear outline of the page |
| `aria-label` on `<nav>` | Gives the navigation a clear name |
| `aria-labelledby` on sections | Connects each section with its heading |
| Descriptive link text | "Visit Priyansh Singh's GitHub profile" is clearer than "click here" |
| `<time datetime>` | Marks dates in a machine-readable way |
| `<meta name="description">` | Short summary of the page |

Accessibility review checklist:
1. Can the whole page be used with the Tab key only?
2. Is the heading order correct?
3. Do all links make sense on their own?
4. Does the page have a language and a title?

## 5. Procedure
1. Create a folder named `1.5-accessible-profile` inside `web-practicals`.
2. Copy the page from practical 1.4 and save it as `index.html` in the new folder.
3. Add a skip link at the top of the `<body>`.
4. Add `aria-label` to the `<nav>` and `aria-labelledby` to each section and article.
5. Replace unclear link text with descriptive link text.
6. Wrap years in `<time>` tags.
7. Open the page in Chrome and press the Tab key to test keyboard navigation.
8. Run a Lighthouse accessibility audit in Chrome DevTools and note the score.
9. Take a screenshot and save it as `output.png`.
10. Upload the folder to GitHub using `git add .`, `git commit` and `git push`.

## 6. Code
The code is kept in a separate file: [index.html](index.html)

## 7. Input
No user input is required. Keyboard Tab key is used to test navigation.

## 8. Output
![Output screenshot](output.png)

## 9. Result
An accessible personal profile page was created with a skip link, correct heading order, labelled landmarks and descriptive links. The page can be used with a keyboard and works with screen readers.

### Review (Lighthouse)
Accessibility score: 94/100. One issue was found: touch targets for the
navigation links are small. This can be fixed later with CSS padding and spacing.


## 10. Viva Questions
1. What is web accessibility and why is it important?
2. What is the use of a skip link?
3. What is the difference between `aria-label` and `aria-labelledby`?
4. Why should link text be descriptive?
5. Why should heading levels not be skipped?
