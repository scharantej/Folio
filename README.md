## Flask Application Design for a Basic Portfolio Website

### HTML Files
#### index.html
- **Purpose**: Home page of the website.
- **Content**: Introduction to the portfolio, showcasing projects and relevant skills.

#### projects.html
- **Purpose**: Page dedicated to displaying portfolio projects.
- **Content**: List of projects with brief descriptions, images, and links to project details.

#### contact.html
- **Purpose**: Contact page for users to reach out.
- **Content**: Contact form and basic information like email and phone number.

### Routes
#### Main Routes
- **@app.route('/')**: Home page, renders `index.html`.
- **@app.route('/projects')**: Projects page, renders `projects.html`.
- **@app.route('/contact')**: Contact page, renders `contact.html`.

#### Project Details Routes
- Each project will have its own route, for example:
    - **@app.route('/projects/project-1')**: Project 1 details page.
- These routes will render a template with the specific project details, such as description, images, and additional information.

#### Contact Form Route
- **@app.route('/contact', methods=['POST'])**: Handles the contact form submission.
- This route will process the form data, such as name, email, message, and can be integrated with a service like SendGrid for sending emails.