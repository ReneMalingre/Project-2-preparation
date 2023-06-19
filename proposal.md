# Project Two - Proposal

## My Idea - *InfoPulse*

## 💡Customer Fact Sheet Generator

### Use Case: Health Clinic/Consultant/Personal Services/Etc business needing to give out information or instructions to clients on demand

40-80% of advice given to clients is forgotten immediately. Information in written form helps to clarify and reinforce important messages and advice and instructions. Paper leaflets are sometimes provided, but it is a burden to keep these up-to-date and printed in the appropriate quantity to ensure they are on hand and that money is not wasted on printing. There can be a reluctance to give them out if the patient or client believes they can remember what was said, in a normal over-estimation of their own ability to recall information. Sometimes more personal information or clarifications/extensions of information are required, and this is often done by hand or by email, which is time-consuming and inefficient.

### ✅Proposal

Lets create an application that allows a business owner/administrator to give a client access to one or more fact sheets that are optionally personalised to ensure they have correct instructions or information relevant to them, enhancing the value they gain from using the services of the business.

The business owner will enrol the client as a user for a web application, providing the client a single-use token that allows them to create an account using their known email address. The business owner will then use a web-based interface to select from a list of pre-written fact sheets, with the option to append custom information and attach them to the user file.

When the user logs on, they will be able to see the list of fact-sheets, and then click on one of them to view the information. The user will be able to open the fact sheet in a new tab, and use browser functions to print it, copy it or save it.

The user will be able to log out, and log back in to view the fact sheets again, and add their own comments to the fact-sheets.

A business will be able to add new fact sheets, edit existing fact sheets, and delete fact sheets.

A business will be able to add new users, edit existing users, and delete users.

A business administrator will be able to add new administrators who can add new fact sheets, edit existing fact sheets, and delete fact sheets.

The fact sheets will be in entered in as markdown, and converted to HTML for display by an npm package.

Images will be able to be uploaded and attached to the fact sheets as a markdown link in the normal way, and will be displayed in the HTML, with an interface in the edit screen to insert a link into the markdown text. The images will be saved in the database as a BLOB, and will be able to be displayed in the HTML using a normal GET request.

## 💁‍♂️ User Story 💁‍♀️

### *MVP*

As a business owner I want to be able to select from a list of pre-written fact sheets, that will generate a HTML page dynamically that can be viewed online through a login
so that I can ensure that my client has the correct information and/or instructions.

As a business owner I want to be able to add custom information to the fact sheets so that I can ensure that the information is personalised to the client.

As a business owner I want to allow authorised users to be able to create, edit and delete the fact sheets so that I can ensure that the information is up-to-date and relevant.

As a business owner I want to create and edit the fact sheets using markdown syntax and convert it to html using an npm package (marked or markdown-it or markdown-js or markdown-to-html) so that I can ensure that the information is formatted correctly and is easy to read.

As a business owner I want to restrict access to the fact sheets to authorised users so that I can ensure that the information is not misused or abused or inaccurate.

As a business owner I want authorised users to be able to be able to enrol the client in the system and whitelist their email address, and give them a permission code to access the information so that I can ensure that the information is only available to them so that I can maintain my clients' privacy and confidentiality.

As a business owner I want to be enable my clients to view the information online or (extending the MVP) receive it via email so that I can ensure that the information is available to them in a convenient format.

As a business owner I want to enable my clients to add notes to the fact sheets so that extra information or clarifications can be added to the information.

As a business owner I want my clients to be able to login to view their information so that I can ensure that the information is only available to them so that I can maintain my clients' privacy and confidentiality and so that all of their information is available to them in one place.

### *Extension*

As a business owner I want to be able to send the information to the client via html email so that I can ensure that the information is available to them in a convenient format.

As a business owner I want to be able to send the information to the client via a PDF attachment to their email so that I can ensure that the information is available to them in a convenient format.

As a business owner I want a selection of non-personalised fact sheets to be viewable available on the landing page as a community service and as a marketing tool to encourage the public to become clients

As a business owner I want to be able to send the sign-up information to the client via a SMS link to make the sign-up process easier for the client

As a business owner I want to be able to send the information to the client via a SMS link with a one-time password to make the information available to the client in a convenient form

As the owner of the service I want to be able to sell subscriptions to the service to other businesses so that I can make money from the service

As the owner of the service I want to provide customised branding for the service to other businesses so that I can make money from the service

## 📃Proposed Pages

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
  - Permission Code (created using *generate-passphrase*)
  - Email (whitelisted in database)
  - Username
  - Password
- Sign up page: client  - same interface as administrator?
  - Permission Code (created using *generate-passphrase*)
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

## 🎨 Design Elements

### Font

<https://fonts.google.com/specimen/Roboto>

### Color Scheme

Healthcare and medical services often use blue tones for their calming, professional, and trustworthy associations. This is a good colour combination:

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

## 📃 Requirements, according to a tutor session

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

## 👷 Suggested work breakdown

- wireframe the app
- design the database schema
- set up the repository
- set up the file system
- set up eslint and prettier

- split the work into tasks:
  - one person working on the database (model)
  - one person working on the routes
  - one person working on the views (handlebars)
  - one person working on the front end javascript to consume the API

  I'm happy to work on anything, but I think I'm best suited to the model as it is the backbone of the application and it is my idea. I can work on converting the markdown to html, and saving and retrieving the images, and on generating the single-use pass phrase.
