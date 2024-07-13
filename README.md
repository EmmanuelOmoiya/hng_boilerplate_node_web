# Strany Integration Documentation

## Overview

Strany is a robust boilerplate API that offers developers with the ease and speed in creating lightning fast, robust and scalable web servers for their web apps.

## Features
This boilerplate includes the following features:

- Authentication (including social and magic link)
- Email messaging with background processing
- Payment integrations (Stripe, Flutterwave, LemonSqueezy)
- User and organization management
- Superadmin interface
- Settings and profile management
- Landing pages (privacy policy, about us, etc.)
- Contact form
- GDPR-compliant cookie handling
- Basic dashboard
- Waitlist functionality
- Marketing/squeeze page
- User invitation flow
- User data export
- Random data management associated with users
- Search and sorting capabilities
- Data visualization with charts
- Content editing
- Notifications system
- Blog functionality
- Invite link generation
- Language and region settings
- Email template management
- AI integration
- Activity logging
- Push notifications

## Features

### Authentication
- User registration and login
- Social authentication (Google, Facebook, etc.)
- Magic link authentication
- In-app authentication screens (login, register, forgot password, reset password)
- Change password functionality

### Messaging
- Email integration with background processing
- Default email templates for common scenarios (welcome, password reset, etc.)

### Payments
- Integration with multiple payment gateways:
  - Stripe
  - Flutterwave
  - LemonSqueezy
- Support for both internal and external payments

### Users & Organizations
- User management system
- Organization management
- User roles and permissions

### Admin Interface
- Superadmin dashboard
- User management
- Organization management
- Payment oversight
- Activity log viewer

### Settings & Profile
- User profile settings
- Application settings page

### Landing Pages
- Privacy policy page
- About us page
- Contact us page with form submission
- GDPR-compliant cookie consent

### Dashboard
- Basic user dashboard
- Waitlist feature (coming soon)
- Squeeze/Marketing page

### Data Management
- Random data associated with users
- Dashboard widgets
- List view of user-associated data
- Single data item view
- Searchable and sortable data lists
- Chart page for data visualization
- Content editing page

### Notifications
- In-app notification system

### Blog
- Basic blog functionality

### Internationalization
- Language and region selection
- Localization support

### Email Template Management
- HTML email template management in the admin interface

### Database & Migrations
- Database schema and migrations
- Recommendations for optimal database usage

### AI Integration
- Basic AI integration capabilities

### Activity Log
- Comprehensive activity logging system

### Push Notifications
- Support for push notifications

# Concept Studies:
[ERD Design](https://app.swaggerhub.com/apis/EMMANUELOMOIYA6/Backend-stage-3/1.0.0)
The Entity-Relationship Diagram represents a robust and flexible schema for a multi-faceted application. Here's an analysis of the relationships and key design aspects:

## User-Centric Design:
The User collection is at the center of the ERD, with many other collections referencing it. This allows for a personalized experience across various features.

## Organization Management:
The Organization collection has a many-to-many relationship with Users through the members array, enabling flexible team structures.

## Payment Tracking:
The Payment collection is linked to Users, allowing for detailed financial tracking per user.

## Messaging System:
The Message and EmailTemplate collections work together to provide a flexible messaging system with reusable templates.

## Customizable Widgets:
The Widget collection, linked to Users, allows for personalized dashboard experiences.

## Activity Logging:
The ActivityLog collection, tied to Users, enables comprehensive tracking of user actions.

## Content Management:
The Content and BlogPost collections provide a foundation for managing various types of content.

## Notification System:
The Notification collection, linked to Users, allows for a personalized notification experience.

## Invitation System:
The Invite collection facilitates user onboarding to organizations.


## Dependencies (Dev)

- Node.js
- TypeScript
- Express
- ts-node-dev
- stripe-node-sdk
- nodemailer
- cookie-js
- recharts
- auth-js

## Getting Started

Before you begin, ensure you have the following installed on your machine:

- [Node.js](https://nodejs.org/) (v14 or later)
- [npm](https://www.npmjs.com/) (Node Package Manager, included with Node.js)
- [Git](https://git-scm.com/)


#### If you don't have git on your machine, [install it](https://docs.github.com/en/get-started/quickstart/set-up-git).

## Fork this repository

Fork this repository by clicking on the fork button on the top of this page.
This will create a copy of this repository in your account.

## Clone the repository

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/clone.png" alt="clone this repository" />

Now clone the forked repository to your machine. Go to your GitHub account, open the forked repository, click on the code button and then click the _copy to clipboard_ icon.

Open a terminal and run the following git command:

```bash
git clone "url you just copied"
```

where "url you just copied" (without the quotation marks) is the url to this repository (your fork of this project). See the previous steps to obtain the url.

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/copy-to-clipboard.png" alt="copy URL to clipboard" />

For example:

```bash
git clone git@github.com:this-is-you/first-contributions.git
```

where `this-is-you` is your GitHub username. Here you're copying the contents of the first-contributions repository on GitHub to your computer.

## Create a branch

Change to the repository directory on your computer (if you are not already there):

```bash
cd first-contributions
```

Now create a branch using the `git switch` command:

```bash
git switch -c your-new-branch-name
```

For example:

```bash
git switch -c add-alonzo-church
```

### Make Changes

Make your changes to the codebase. Ensure your code follows the project's coding standards and guidelines.

### Run Tests

Run the existing tests to ensure your changes do not break anything. If you added new functionality, write corresponding tests.

```sh
npm run test
```

## commit those changes

Now open `Contributors.md` file in a text editor, add your name to it. Don't add it at the beginning or end of the file. Put it anywhere in between. Now, save the file.

<img align="right" width="450" src="https://firstcontributions.github.io/assets/Readme/git-status.png" alt="git status" />

If you go to the project directory and execute the command `git status`, you'll see there are changes.

Add those changes to the branch you just created using the `git add` command:

## Push changes to GitHub

Push your changes using the command `git push`:

```bash
git push -u origin your-branch-name
```

replacing `your-branch-name` with the name of the branch you created earlier.

<details>
<summary> <strong>If you get any errors while pushing, click here:</strong> </summary>

- ### Authentication Error
     <pre>remote: Support for password authentication was removed on August 13, 2021. Please use a personal access token instead.
  remote: Please see https://github.blog/2020-12-15-token-authentication-requirements-for-git-operations/ for more information.
  fatal: Authentication failed for 'https://github.com/<your-username>/first-contributions.git/'</pre>
  Go to [GitHub's tutorial](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account) on generating and configuring an SSH key to your account.

</details>

## Submit your changes for review into Staging

If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.

<img style="float: right;" src="https://firstcontributions.github.io/assets/Readme/compare-and-pull.png" alt="create a pull request" />

Now submit the pull request.

<img style="float: right;" src="https://firstcontributions.github.io/assets/Readme/submit-pull-request.png" alt="submit pull request" />

Soon your changes will be merged into the staging branch of this project. You will get a notification email once the changes have been merged.

## Setup Instructions

### 1. Clone the Repository

First, clone the repository to your local machine using Git.

```sh
git clone https://github.com/your-username/Strany.git
cd Strany
```

### 2. Install Dependencies

Navigate to the project directory and install the required dependencies.

```sh
npm install
```

### 3. Configure Environment Variables

Create a `.env` file in the root directory of the project and add your environment-specific variables. You can use the provided `.env.example` file as a reference.

```sh
cp .env.example .env
```

Edit the `.env` file to match your environment configuration.

### 4. Compile TypeScript

Compile the TypeScript code to JavaScript.

```sh
npm run build
```

### 5. Run the Development Server

Start the development server with the following command. This will also watch for any changes in your code and automatically restart the server.

```sh
npm run start:dev
```

### 6. Run the Production Server

To run the application in a production environment, use the following command:

```sh
npm run start
```

### 7. Verify the Setup

Open your browser and navigate to `http://localhost:3000/api/v1/` to verify that the application is running correctly.

## Folder Structure

Here's an overview of the project's folder structure:

```
|--- src
|    |--- controllers
          |--- v1
|    |--- database
|    |--- interfaces
|    |--- middlewares
|    |--- modules
|         |--- user
|         |--- organisation
|         |--- notification
|         |--- payment
|         |--- message
|         |--- emailTemplate
|         |--- widget
|         |--- activityLog
|         |--- contact
|         |--- content
|         |--- notification
|         |--- blog
|         |--- invitedatabase
|    |--- routes
|         |--- v1
|    |--- services
|    |--- utils
|    |--- server.ts
|--- .env
|--- config
|   |---config.ts
|   |--- roles.ts
|--- app.tsx
|--- index.tsx
|--- app.ts
|--- .gitignore
|--- package.json
|--- tsconfig.json
```

## Scripts

Here are some useful npm scripts that you can use during development and production:

- `npm run build`: Compiles the TypeScript code to JavaScript.
- `npm run start:dev`: Starts the development server with live reloading.
- `npm run start`: Starts the production server.
- `npm run test`: Runs the test suite (if available).
- `npm run lint`: Runs the linter to check for code style issues.

## Additional Resources

- [Node.js Documentation](https://nodejs.org/en/docs/)
- [TypeScript Documentation](https://www.typescriptlang.org/docs/)
- [Express Documentation](https://expressjs.com/)

By following these steps, you should have your Node.js and TypeScript application up and running. If you encounter any issues, please refer to the documentation of the respective tools or seek help from the community.

## API Endpoints

Here are API endpoints and their specifications:

## User Management:
- POST /api/users - Create a new user
- GET /api/users/:id - Retrieve user details
- PUT /api/users/:id - Update user information
- DELETE /api/users/:id - Delete a user (or deactivate)


## Authentication:

- POST /api/auth/login - User login
- POST /api/auth/register - User registration
- POST /api/auth/forgot-password - Initiate password reset
- POST /api/auth/reset-password - Reset password
- POST /api/auth/social/:provider - Social authentication


## Organization Management:

- POST /api/organizations - Create a new organization
- GET /api/organizations/:id - Retrieve organization details
- PUT /api/organizations/:id - Update organization information
- DELETE /api/organizations/:id - Delete an organization
- POST /api/organizations/:id/members - Add a member to an organization
- DELETE /api/organizations/:id/members/:userId - Remove a member from an organization


## Payment Management:

- POST /api/payments - Create a new payment
- GET /api/payments/:id - Retrieve payment details
- GET /api/users/:id/payments - Retrieve user's payment history


## Messaging:

- POST /api/messages - Send a new message
- GET /api/messages/:id - Retrieve message details
- GET /api/users/:id/messages - Retrieve user's message history


## Email Templates:

- POST /api/email-templates - Create a new email template
- GET /api/email-templates/:id - Retrieve template details
- PUT /api/email-templates/:id - Update a template
- DELETE /api/email-templates/:id - Delete a template


## Widget Management:

- POST /api/widgets - Create a new widget
- GET /api/widgets/:id - Retrieve widget details
- PUT /api/widgets/:id - Update a widget
- DELETE /api/widgets/:id - Delete a widget
- GET /api/users/:id/widgets - Retrieve user's widgets


## Activity Logging:

- GET /api/activity-logs - Retrieve activity logs (with filtering options)
- GET /api/users/:id/activity-logs - Retrieve user's activity logs


## Content Management:

- POST /api/content - Create new content
- GET /api/content/:id - Retrieve content
- PUT /api/content/:id - Update content
- DELETE /api/content/:id - Delete content


## Blog Management:

- POST /api/blog-posts - Create a new blog post
- GET /api/blog-posts/:id - Retrieve a blog post
- PUT /api/blog-posts/:id - Update a blog post
- DELETE /api/blog-posts/:id - Delete a blog post
- GET /api/blog-posts - Retrieve all blog posts (with pagination)


## Notification System:

- POST /api/notifications - Create a new notification
- GET /api/notifications/:id - Retrieve notification details
- PUT /api/notifications/:id - Update a notification (e.g., mark as read)
- GET /api/users/:id/notifications - Retrieve user's notifications


## Invitation System:

- POST /api/invites - Create a new invite
- GET /api/invites/:id - Retrieve invite details
- PUT /api/invites/:id - Update an invite (e.g., accept/reject)
- DELETE /api/invites/:id - Delete an invite


## Versioning

This project is versioned to ensure backward compatibility and easy maintenance. The current version is [version].

## Contributors

- Emmanuel Omoiya emmanuelomoiya6@gmail.com
- Aroso Emmanuel Adedeji emarc.aroso@outlook.com
- Nnenna Kehinde nneukamaka@gmail.com

## Contributing
We welcome contributions to this Boilerplate project. Please follow these guidelines when contributing:

1. Fork the repository and create a new branch for your feature or bug fix.
2. Follow the coding standards and conventions used in the project.
3. Keep your code as decoupled as possible to maintain modularity.
4. Write clear and concise commit messages.
5. Submit a pull request with a detailed description of your changes.

For more information on our coding standards and best practices, please refer to the [CONTRIBUTING.md](https://github.com/EmmanuelOmoiya/hng_boilerplate_node_web/blob/main/CONTRIBUTORS_GUIDE.md) file.

