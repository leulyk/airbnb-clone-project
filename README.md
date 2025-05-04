# AirBnB Clone Project

> This project is a full-stack clone of the popular accommodation booking platform AirBnB. 
The goal is to build a functional web application that allows users to browse property listings, view detailed property information, and complete bookings.
The project will cover frontend development, backend APIs, database design, and deployment with the technology stack described below.

### Project Roles and Responsibilities

- #### Project Manager
  - Oversees timeline, coordinates team, manages deliverables

- #### Frontend Developers
  - Implements UI components, ensures responsive design

- #### Backend Developers
  - Builds APIs, manages database, implements business logic

- #### Designer
  - Creates mockups, maintains design system, ensures UX quality

- #### QA/Testers
  - Writes test cases, performs testing, reports bugs

- #### DevOps Engineer
  - Manages deployment, CI/CD pipeline, server infrastructure

- #### Product Owner
  - Defines requirements, prioritizes features, represents stakeholders

- #### Scrum Master
  - Facilitates agile processes, removes blockers, organizes meetings

- #### Database Administrator
  - Dedicated to database design, setup and maintenance

### Feature Breakdown

- User authentication
 
- User management
 
- Property management
 
- Booking system
 
- Review submission & management

- Secure checkout process


### Technology Stack

- **Design Tools**: 
  - **Figma**: a web based design and prototyping tool for UI/UX design.

- **Frontend**: 
  - **TypeScript**: the typed superset of JavaScript that provide type safety and improved development process.
  - **React.js / Next.js**: modern and progressive frontend frameworks to build highly dynamic, reactive and responsive layouts.

- **Backend**: 
  - **Django**: a robust python web framework for building secure and scalable web applications.
  - **MySQL**: a popular RDBMS known for it's reliability and scalability. 
  - **GraphQL**: a modern query language to communicate with APIs.

- **Version Control**: 
  - **Git**: a versatile & powerful distributed version control system.
  - **GitHub**: a cloud based hosting platform for hosting and collaborating with code.

### UI/UX Design Planning

#### Design Goals

- Create intuitive booking flow

- Maintain visual consistency

- Ensure fast loading times

- Prioritize mobile responsiveness

#### Primary Pages

| Page                   | Description                                            |
|------------------------|--------------------------------------------------------|
| Property Listing View	 | Grid display of available properties with filters      |
| Listing Detailed View	 | Complete property details with images and booking form |
| Simple Checkout View	  | Streamlined payment and booking confirmation           |

#### Importance of User-Friendly Design

A well-designed booking system reduces friction in the user journey, increases conversion rates, and improves customer satisfaction. Clear navigation, intuitive interfaces, and responsive design are critical for success.

#### Figma Design Specifications

##### Color Styles:

- **Primary**: `#FF5A5F`

- **Secondary**: `#008489`

- **Background**: `#FFFFFF`

- **Text**: `#222222`

- **Secondary Text**: `#717171`

##### Typography:

- **Primary Font**: Circular, Medium (500), 16px
- **Headings**: Circular, Bold (700), 24px-32px
- **Secondary Text**: Circular, Book (400), 14px

### UI Component Patterns

- Navbar: Top navigation bar with links to sign in, signup, search for properties and checking in/out.
- Property Card: Small card showing a property with image, title, price, and rating.
- Property details: image gallery, property info, booking form, review form and list.
- Booking: Section to select dates, see price, and confirm booking.
- Footer: Bottom section with links to about, support, terms, and more.

### Database Design

#### Key Entities and Fields

- Users
  - id
  - name
  - email
  - password
  - profilePictureUrl
  - createdAt
  - updatedAt
- Properties
  - id
  - ownerId *(foreign key)*
  - title
  - description
  - address
  - city
  - country
  - numberOfBedrooms
  - numberOfBathrooms
  - createdAt
  - updatedAt
- Bookings
  - id
  - propertyID *(foreign key)*
  - userID *(foreign key)*
  - startDate
  - endDate
  - status
  - createdAt
  - updatedAt
- Reviews
  - id
  - propertyID *(foreign key)*
  - userID *(foreign key)*
  - bookingID *(foreign key)*
  - rating
  - comment
  - timestamps
- Payments
  - id
  - bookingID *(foreign key)*
  - userID *(foreign key)*
  - amount
  - currency
  - paymentMethod
  - createdAt

### API Security

#### Key Security Measures

- Authentication: the process of identifying a user in our application.
- Authorization: the process of identifying if a user has privilege to access a certain resource in our application.
- Rate Limiting: the number of requests a client can make to our API in a given period of time.
- HTTPS: encrypted communication between client and server to prevent sending sensitive data over a network.

### CI/CD Pipeline

CI/CD provides a structured and automated way to build, test and deploy code. It has the following benefits:
- Faster development cycles
- Continuous feedback
- Early bug detection
- Test automation
- Enhance scalability

#### Tools

- GitHub Actions
- Docker