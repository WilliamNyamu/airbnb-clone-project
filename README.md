# AirBnB Clone Project
- The backend for the Airbnb Clone project is designed to provide a robust and scalable foundation for managing user interactions, property listings, bookings, and payments. This backend will support various functionalities required to mimic the core features of Airbnb, ensuring a smooth experience for users and hosts.

## Team Roles
### Backend Engineer
- Responsible for implementing API endpoints, database schemas, and business logic
### Database Administrator
- Manages database design, indexing, and optimizations
### DevOps Engineer
- Handles deployment, monitoring, and scaling of the backend services
### QA Engineer
- Ensures the backend functionalities are thoroughly tested and meet quality standards

## Technology Stack
### Django
- A high-level Python web framework used for building the RESTful API
### Django REST Framework
- Provies tools for creating and managing RESTful API.
### PostgreSQL
- A powerful relational database used for data storage.
### GraphQL
- Allows for flexible and efficient querying of data.
### Celery
- For handling asynchronous tasks such as sending notifications or processing payments
### Redis
- Used for caching and session management
### Docker
- Containerization tool for consistent developmnet and deployment environments
### CI/CD Pipelines
- Automated pipelines for testing and deploying code changes.


## Database Design
### User
- Key fields include: id(pk), email(unique), first_name, last_name, profile_picture, phone_number.
### Property
- Key fields include: id, name, location, price, owner, propery_images, 
  - A user can have multiple properties
### Booking
- Key fields include: id(pk), user, property, booked_date, duration_stay,
    - A booking is for a particular user.
### Review
- Key fields include: id(pk), user, property, comment, rating, created_date
  - A property can have multiple reviews, but a user can have only one review for a particular property
### Payment
- Key fields include: id(pk), user, price, payment_date, property


## Feature Breakdown
### User Management
- Implement a secure system for user registration, authentication, and profile management
### Property Management
 -  Develop features for property listing creation, updates, and retrieval.
### Booking System
 - Create a booking mechanism for users to reserve properties and manage booking details.
### Payment Processing
 - Integrate a payment system to handle transactions and record payment details.
### Review System
 - Allow users to leave reviews and ratings for properties.
### Data Optimization
 -  Ensure efficient data retrieval and storage through database optimizations.


## API Security
### Authentication
 - Authenticate users to allow performing certain actions such as booking, and accessing certain portals.
### Authorization
 - Allow only authorized users to perform certain CRUD actions such as hotel management.
### Rate Limiting
 - Controlling how often a particular action such as booking can happen in a specific time period.


## CI/CD Pipeline
- To automate build, test, and deploy code changes for production.
- Tools: Docker, Kubernetes, Github Actions
