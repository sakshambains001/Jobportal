# HireX

HireX is a simple BCA-level job portal project built with HTML, CSS, JavaScript, SQLite, and SQL. The project is designed to be beginner-friendly, easy to explain in viva, and easy to modify.

## Project Features

- Job seeker registration and login
- Employer registration and login
- Admin login and dashboard
- Job search and filtering
- Job apply and save functionality
- Employer job posting and management
- Application status tracking
- SQLite schema and sample SQL queries
- Responsive and simple UI

## Folder Structure

- `index.html` - Home page
- `jobs.html` - Job listing page
- `job-details.html` - Job details page
- `login.html` - Login page
- `register.html` - Registration page
- `about.html` - About page
- `contact.html` - Contact page
- `seeker-dashboard.html`, `seeker-profile.html`, `my-applications.html`, `saved-jobs.html`
- `employer-dashboard.html`, `company-profile.html`, `post-job.html`, `manage-jobs.html`, `applicants.html`
- `admin-dashboard.html`, `manage-users.html`, `manage-applications.html`
- `css/style.css` - Main stylesheet
- `js/*.js` - JavaScript files
- `database/schema.sql` - SQLite schema
- `database/sample-data.sql` - Sample data
- `database/migrate-work-mode.sql` - One-time upgrade for an existing database
- `jobportal.db` - SQLite database file

## Important Note About SQLite

This project keeps the front-end and database design separate, because a browser-only HTML/JavaScript website cannot directly connect to SQLite in the same way as a server-side application. To connect to a real SQLite database in a production-style project, you would need a small server-side bridge such as Node.js with the SQLite package.

Since your requirement was to use HTML, CSS, JavaScript, SQLite 3, and SQL only, the project here focuses on a beginner-friendly demo website plus a proper SQLite schema and SQL examples. The database files are included so you can explain the design clearly in your viva.

## How to Use

1. Open `index.html` in a browser.
2. Use the registration page to create account roles.
3. Login as job seeker, employer, or admin.
4. Explore jobs, save them, apply, manage posts, and review dashboard pages.

## Autonomous Testing

Open `test-runner.html` in the browser and click **Run tests**. The runner checks all 19 pages, role-based access, login validation, job search and filtering, seeker apply/save actions, employer job posting, and admin controls. It restores the original browser storage after the run, so test data does not change the demo state.

## Database Notes

The SQLite database is created using the SQL script in `database/schema.sql` and sample records in `database/sample-data.sql`.
For an existing database, run `database/migrate-work-mode.sql` once before using the updated schema. It adds a defaulted work mode to existing jobs and converts legacy `Remote` locations to an eligible region (`India`) with `Remote` work mode. The existing database file and records are not replaced.

## Viva Tip

When presenting this project in class, explain:

- HTML builds the page structure.
- CSS adds styling and responsiveness.
- JavaScript handles validation, filters, and page behavior.
- SQL creates the database and manages records.
- SQLite stores the project data in a simple database file.

This project is made for easy explanation and BCA-level understanding.
