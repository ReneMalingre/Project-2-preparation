# Project Two - Proposal

## Requirements, according to the tutor

- MySQL, sequelize, express, node, handlebars, express-sessions, sequelize-sessions
- **one other npm package**
- There should be a landing page that explains the purpose of the app and invites the user to log in or sign up
- login, sign-up, logout
- at least one other page that can only accessible by a logged in user
- must be a one-to-many or many-to-many relationship between two models
- must have complete CRUD functionality for at least one of the models
- must have a user model and at least one other model
- should have home route for page navigation
- should have user route for user functions
- should have at least one other route for other functions
- must display data from the database on the page

## Suggested work breakdown

- wireframe the app
- design the database schema

- split the work into tasks
  - one person working on the database (model)
  - one person working on the routes
  - one person working on the views (handlebars)
  - one person working on the front end javascript to consume the API

## My Ideas

## 💡Informational Fact Sheet Generator - *InfoPulse*

### User: Health Clinic/Consultant/Personal Services/Etc business needing to give out information or instructions to clients on demand

40-80% of advice given to clients is forgotten immediately. Information in written form helps to clarify and reinforce important messages and advice and instructions. Paper leaflets are sometimes provided, but it is a burden to keep these up-to-date and printed in the appropriate quantity to ensure they are on hand and that money is not wasted on printing. There can be a reluctance to give them out if the patient or client believes they can remember what was said, in a normal over-estimation of their own ability to recall information. Sometimes more personal information or clarifications/extensions of information are required, and this is often done by hand or by email, which is time-consuming and inefficient.

#### ✅Proposal

Using a web-based form to select from a list of pre-written fact sheets, with the option to add custom information, will generate a HTML page dynamically that can either be viewed online through a login or (extension to MVP) sent via an HTML email directly to the patient.

- Eg: You are myopic – here are some facts
- Everything is fine: see you in two years unless you have problems
- Here is how to clean your eyelash line to avoid infection and improve your dry-eye
- Thanks for visiting: here is some information about your visit and your practitioner, and when you should return.
- Suggest fact sheets are edited in markdown and use an npm package to convert it to html.
- Ability to add images to the fact sheets to enhance the information.

### User Story

#### *MVP*

As a business owner:

- I want to be able to select from a list of pre-written fact sheets, that will generate a HTML page dynamically that can be viewed online through a login
- so that I can ensure that my client has the correct information and/or instructions.
As a business owner:
- I want to be able to add custom information to the fact sheets
- so that I can ensure that the information is personalised to the client.
As a business owner:
- I want to authorised users to be able to create, edit and delete the fact sheets
- so that I can ensure that the information is up-to-date and relevant.
As a business owner:
- I want to create and edit the fact sheets using markdown syntax and convert it to html using an npm package (marked or markdown-it or markdown-js or markdown-to-html)
- so that I can ensure that the information is formatted correctly and is easy to read.
As a business owner:
- I want to restrict access to the fact sheets to authorised users
- so that I can ensure that the information is not misused or abused or inaccurate.
As a business owner:
- I want authorised users to be able to be able to enrol the client in the system and whitelist their email address, and give them a permission code to access the information
- so that I can ensure that the information is only available to them so that I can maintain my clients' privacy and confidentiality.
As a business owner:
- I want to be enable my clients to view the information online or (extending the MVP) receive it via email
- so that I can ensure that the information is available to them in a convenient format.
As a business owner:
- I want my clients to be able to login to view their information
  - so that I can ensure that the information is only available to them so that I can maintain my clients' privacy and confidentiality.
  - and so that all of their information is available to them in one place.

#### *Extension*

As a business owner:

- I want to be able to send the information to the client via html email
  - so that I can ensure that the information is available to them in a convenient format.
As a business owner:
- I want to be able to send the information to the client via a PDF attachment to their email
  - so that I can ensure that the information is available to them in a convenient format.
As a business owner:
- I want a selection of non-personalised fact sheets to be viewable available on the landing page
  - as a community service and as a marketing tool to encourage the public to become clients
As a business owner:
- I want to be able to send the sign-up information to the client via a SMS link
  - to make the sign-up process easier for the client
As a business owner:
- I want to be able to send the information to the client via a SMS link with a one-time password
  - to make the information available to the client in a convenient form
As the owner of the service:
- I want to be able to sell subscriptions to the service to other businesses
  - so that I can make money from the service
As the owner of the service:
- I want to provide customised branding for the service to other businesses
  - so that I can make money from the service

Landing page

#### Proposed Pages

- Landing page
  - Pretty, simple, inviting, professional
  - Choose if you are a client or an administrator
  - Login
  - Sign up
- Login page: Administrator
  - Username
  - Password
- Login page: client - same interface as administrator?
  - Username
  - Password
- Sign up page: Owner/Administrator/Staff
  - Permission Code (created using generate-passphrase)
  - Email (whitelisted in database)
  - Username
  - Password
- Sign up page: client  - same interface as administrator?
  - Permission Code (created using generate-passphrase)
  - Email (whitelisted in database)
  - Username
  - Password
- Dashboard: Administrator
  - View list of clients, add, edit, delete clients, reset password
  - View list of administrators, add, edit, delete administrators, reset password
  - View list of fact sheets, add, edit, delete fact sheets
  - Add/replace images for fact sheets
  - Select fact sheets, add custom information, generate HTML page to preview, make available to client via their dashboard
- Dashboard: client
  - View list of fact sheets, select one to view
  - logout
  - update profile
  - change password

### Design Elements

#### Font

<https://fonts.google.com/specimen/Roboto>

#### Color Scheme

Healthcare and medical services often use blue tones for their calming, professional, and trustworthy associations. Here are a few color combinations:

Classic Medical Palette:

Light Blue (#5698C6)
Dark Blue (#31557F)
White (#FFFFFF)
Light Grey (#F2F2F2)
Viridian (#4A7C59)
Dark Grey (#333333)

utilize this color palette for various elements of the website:

Background: Light Grey (#F2F2F2) for the website's main background color. This color is light and neutral, which makes it perfect for a background color.

Navigation Bar / Footer: Use Dark Blue (#31557F) for the navigation bar and footer. Dark colors are often used for these sections to provide a solid base.

Buttons / Links / CTAs: Light Blue (#5698C6) could be used for clickable elements such as buttons, links, or Call to Actions (CTAs). This color will stand out against the other colors, drawing the user's attention.

Text: For primary text, you can use Dark Blue (#31557F) and Dark Grey (#333333) to ensure readability. White (#FFFFFF) can be used for text on darker backgrounds (like on buttons, navigation bar).

Highlights / Accents: Viridian (#4A7C59) can be used as an accent color for highlights, icons, or to draw attention to specific areas.

Borders / Dividers / Shadows: Light Blue (#5698C6) and Viridian (#4A7C59) can be used for borders, dividers, or shadows, creating depth and definition.
