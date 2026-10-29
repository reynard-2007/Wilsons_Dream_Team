
#COS10026

# DTShop Recruitment Website

A static recruitment website for **DTShop**, an online retail platform expanding its technical and user experience teams. The site advertises job vacancies and lets candidates submit an application through a validated HTML5 form.

Built for the group project, industry allocation **G05: E-Commerce & Digital Retail Platform**.

- **Live site:** https://reynard-2007.github.io/Wilsons_Dream_Team/
- **Jira project:** https://cos10026wilsondoan.atlassian.net/jira/software/projects/SCRUM/boards/1
- **GitHub repository:** https://github.com/reynard-2007/Wilsons_Dream_Team.git

## Tech Stack

- HTML5 (semantic elements, validated)
- CSS3 (external stylesheet, plus embedded and inline examples)
- No JavaScript, no Bootstrap or other frameworks
- Deployed with GitHub Pages

## Project Structure

```
/
├── index.html      Home page
├── jobs.html       Job descriptions
├── apply.html      Job application form
├── about.html      Group information
├── styles.css      External stylesheet
├── images/         Logo, home image, group photo (< 300KB)
└── README.md
```

## Pages

| Page | Purpose |
|------|---------|
| `index.html` | Company logo, name, slogan, description and image. Shared navigation, search box with button, a table using merged cells, and a footer with Jira, GitHub and email links. Background graphic made with CSS. |
| `jobs.html` | Two or more job descriptions, each with a 5-character alphanumeric reference number, title, short description, salary, reporting line, responsibilities, and essential and preferable requirements. Uses multiple `<section>` elements, two heading levels, one ordered list, one unordered list, and a floated `<aside>`. |
| `apply.html` | Application form posting to `formtest.php` (POST) with HTML5 validation, regex patterns and suitable input types. All fields are required except "Other skills". Layout built with Flexbox or Grid. |
| `about.html` | Group name and class day/time (nested list), member contributions and quotes (definition list, with first-language quote and English translation), group photo in `<figure>` with caption, and a fun facts table with caption. |

## Application Form Validation

| Field | Rule |
|-------|------|
| Job reference number | Exactly 5 alphanumeric characters |
| First name, Last name | Letters only, max 20 characters |
| Date of birth | `dd/mm/yyyy` |
| Gender | Radio buttons in a `fieldset` with `legend` |
| Street address, Suburb/Town | Max 40 characters |
| State | Dropdown: VIC, NSW, QLD, NT, WA, SA, TAS, ACT |
| Postcode | Exactly 4 digits |
| Email | Valid email format |
| Phone number | 8 to 12 digits |
| Skill list | Checkboxes |
| Other skills | Textarea (optional) |

## Styling Notes

- Single external stylesheet (`styles.css`) with section comments and a wide range of selectors.
- Responsive layout using media queries.
- Accessibility: sufficient colour contrast, visible focus states, readable font sizes, labelled form controls, alt text on images.
- One embedded `<style>` block and one inline style on every page, kept to a minimum.
- Page-specific styling:
  - `index.html`: CSS background graphic
  - `jobs.html`: `<aside>` floated right, 25% width, with margin, padding and border
  - `about.html`: styled student IDs, bordered figure, table with hex colours and hover effects
  - `apply.html`: Flexbox/Grid form layout

## Acknowledgement of Aboriginal and Torres Strait Islander Peoples

The site includes [describe your element, e.g. an Acknowledgement of Country on the home page and an inclusive employment statement on the jobs page]. [Briefly explain why it was included and how it connects to the company's values and hiring practice.]

## Running Locally

No build step is needed. Clone the repository and open `index.html` in a browser.

```
git clone [GitHub repository URL]
cd [repository-name]
```

## Validation

- HTML: https://validator.w3.org/
- CSS: https://jigsaw.w3.org/css-validator/

All pages pass validation with no errors.

## Team

**Group:** Wilson's dream team
**Class:** Thurday, 7a.m-10a.m
| Name | Student ID | Contribution |
|------|------------|--------------|
| Yuki | 106394628 | Jobs.html |
| Khang | 106391302 | Index.html |
| Hung | 106726072 | About.html |
| Anh | 106727091 | Apply.html |

## Deployment

Hosted on GitHub Pages from the `main` branch, root folder.
