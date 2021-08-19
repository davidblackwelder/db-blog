# Blog Software Requirements Specification (SRS)

<br>

## Section 1 - Purpose

You will be building a blogging content management system. This application will be multi-tenant and use
role based security to route the end user to the correct areas of the application. The application will allow all
users to view blog posts and comments, registered users will be allowed to add comments, moderators will
be able to edit comments posted by others, and authors will be able to create new blog posts.
<br>
<br>

## Section 2 - Technology

This application should be built using Ruby on Rails. The application will be congured to use a Postgres SQL database and will be hosted on Heroku. The user interface will be built on a Bootstrap template and will require the use of HTML, CSS, and JavaScript for customization and functionality. Additional JavaScript libraries may be used as needed to improve performance or display.
<br>
<br>

## Section 3 - Requirements

The requirements for this application are split into two broad categories: Functional and User Interface. Functional requirements describe the core functions of the application, the things the end user must be able to do. User Interface requirements describe aspects of the application that facilitate intuitive and userfriendly interaction. A functional application that is hard to use will struggle to reach an audience.
<br>
<br>

### Functional Requirements _(required)_

- **DATA**
  - Roles of Administrator and Moderator will be created
  - A user will be seeded and will occupy the role of Administrator
  - A user will be seeded and occupy the role of Moderator
    <br>
    <br>
- **BLOGS**
  - Blogs will carry an image
  - Blogs will have Posts
  - Blogs will be paged
- **POSTS**
  - Posts are created with Rich Text Editor
  - Posts allow upload of 1 or more images
  - Posts have Tags
  - Posts should have "human readable" URLs (Slug)
  - Posts can be ltered by Tags
  - Posts should display in a chronological order
  - Posts can be searched by the user
  - Posts will be paged
- **COMMENTS**
  - Administrators and Moderators can edit/delete comments
  - Registered users can leave comments
  - Users should be able to register using 3rd party authentication
  - Comments should display in a chronological order
    <br>
    <br>

### Functional Requirements _(desired)_

- Introduce the Author role
- Separate Blogs for individual authors
- Users in Author role can create Posts in their Blog
- New users can apply to be given the Author role
  <br>
  <br>

### User Interface Requirements

- The application should have a Bootstrap based template
- Navigation menu should be present on all pages
- Users should be able to update their personal information
- Navigation through the application should NOT rely on browser functionality
- Comment creation should be connected to specic posts
- Blogs should lead me to specic sets of Posts
- Color theme should be inviting
