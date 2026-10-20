# MotoCare — Motorcycle Service Booking System

A front-end demonstration of an online motorcycle service booking website, built as a
student project. The site is **static**: plain HTML5, CSS3 and vanilla JavaScript with
no backend, no database and no third-party frameworks.

> **Scope note.** MotoCare is a portfolio / academic prototype. The forms do not send
> email, do not create real appointments and do not store any data. Every price,
> address, phone number and email address in the project is a clearly marked sample
> value for demonstration purposes.

## Pages

| File | Purpose |
| --- | --- |
| `index.html` | Landing page: hero, service highlights, process steps, sample prices and calls to action. |
| `services.html` | Full service catalogue with sample prices, plus an interactive **cost estimator**. |
| `booking.html` | **Appointment request** form with client-side validation. |
| `about.html` | About the workshop, the team, values and answers to common questions. |
| `contact.html` | Workshop contact details, map-style panel and a validated **contact form**. |

## Folder structure

```
MotoCare/
├── index.html          Landing page
├── services.html       Service catalogue + cost estimator
├── booking.html        Appointment request form
├── about.html          About / team page
├── contact.html        Contact page + contact form
├── README.md           This file
├── css/
│   └── style.css       Single shared stylesheet (design tokens + responsive rules)
├── js/
│   └── script.js       All page behaviour (estimator, forms, navigation)
├── assets/
│   ├── bike-hero.svg        Hero illustration
│   ├── workshop-scene.svg   Workshop illustration
│   ├── avatar-1.svg         Team member avatar
│   ├── avatar-2.svg         Team member avatar
│   ├── avatar-3.svg         Team member avatar
│   └── .gitkeep
└── docs/
    ├── DEPLOYMENT.md            GitHub Pages deployment guide
    ├── FINAL-AUDIT-REPORT.md    Verification results
    ├── SCHOOL-CHECKLIST.md      Requirement-by-requirement checklist
    ├── CONCEPT.md               Project concept and objectives
    ├── INTERVIEW-QUESTIONS.md   Interview questions for a motorcycle owner
    ├── SURVEY.md                15-respondent customer survey
    ├── EVIDENCE-CHECKLIST.md    Screenshot and evidence checklist
    ├── PRESENTATION.md          Slide-by-slide presentation outline
    └── DEMO-SCRIPT.md           Live demonstration script
```

## Features

1. **Service cost estimator** (`services.html`) — pick a service and a quantity, and the
   page totals the job in Philippine pesos. It rejects a quantity of `0` or `99+`,
   recalculates when the inputs change, and always labels the result as a guide rather
   than a final quotation.
2. **Appointment request form** (`booking.html`) — asks for the customer's name, Philippine
   mobile number, motorcycle brand and model, optional plate number, a required service,
   a future preferred date and time, and optional notes. Invalid submissions are blocked
   and explained inline.
3. **Contact form** (`contact.html`) — name, email and message with validation, and a
   success notice that states plainly that no message was actually sent.
4. **Responsive layout** — CSS Grid and Flexbox with breakpoints at 560px, 900px and
   1120px. Cards stack into a single column on small screens, and the navigation
   collapses into a CSS-only hamburger menu.
5. **Accessibility and polish** — semantic landmarks, visible focus states, skip link,
   `prefers-reduced-motion` support, and print styles.

## Sample price list

Prices are unverified student-project samples and are displayed as such on the site.

| Service | Sample price |
| --- | --- |
| Oil Change | ₱250 |
| Brake Inspection | ₱150 |
| Tire Service | ₱300 |
| Engine Tune-Up | ₱500 |
| Chain Adjustment | ₱150 |
| General Motorcycle Inspection | ₱200 |

## Running the project locally

The project uses only relative paths, so it works from any web server or from the
project folder directly.

**With XAMPP:** copy the `MotoCare` folder into `C:\xampp\htdocs\`, start Apache from
the XAMPP control panel, then open
`http://localhost/MotoCare/index.html`.

**With any static server** (from inside the `MotoCare` folder):

```bash
python -m http.server 8000
# then open http://localhost:8000/index.html
```

Opening `index.html` directly from the file system also works, because no request has
to be made to a server for the page to render.

## Deploying to GitHub Pages

See [`docs/DEPLOYMENT.md`](docs/DEPLOYMENT.md) for the complete walkthrough, including
the optional GitHub Actions workflow.

## Before submitting

- [ ] Replace the sample business details in `contact.html` and `about.html` (each one is
      marked with an `<!-- EDITABLE: ... -->` comment).
- [ ] Replace the two placeholder team member names in `about.html`.
- [ ] Replace the sample price list if your workshop uses different prices.
- [ ] Deploy to GitHub Pages and confirm the public URL loads all five pages.

## Project documentation

| Document | Contents |
| --- | --- |
| [`docs/DEPLOYMENT.md`](docs/DEPLOYMENT.md) | GitHub Pages deployment guide. |
| [`docs/FINAL-AUDIT-REPORT.md`](docs/FINAL-AUDIT-REPORT.md) | Verification results for every page, feature and file. |
| [`docs/SCHOOL-CHECKLIST.md`](docs/SCHOOL-CHECKLIST.md) | Requirement-by-requirement checklist. |
| [`docs/CONCEPT.md`](docs/CONCEPT.md) | Project concept and objectives. |
| [`docs/INTERVIEW-QUESTIONS.md`](docs/INTERVIEW-QUESTIONS.md) | Interview questions for a motorcycle owner. |
| [`docs/SURVEY.md`](docs/SURVEY.md) | 15-respondent customer survey. |
| [`docs/EVIDENCE-CHECKLIST.md`](docs/EVIDENCE-CHECKLIST.md) | Screenshot and evidence checklist. |
| [`docs/PRESENTATION.md`](docs/PRESENTATION.md) | Slide-by-slide presentation outline. |
| [`docs/DEMO-SCRIPT.md`](docs/DEMO-SCRIPT.md) | Live demonstration script. |
