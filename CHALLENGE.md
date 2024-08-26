# Coding Challenge: Employee Enrollment Management Application

## Overview
Build a simplified enrollment mangement application where users can create, update, delete, and view insurance enrollments for the employees of a **group**.

**Group** - A group is defined as a collection of individuals who are covered under a single insurance policy.  
**Employee** - Is defined as an individual who works for an employer and is eligible to participate in the employer's group insurance plan.  
**Enrollment** - The start and end dates, where an employee is covered by a particular plan.

## Data Modeling
- A group must have a name, for example "Noyo Corporation"
- Each employee must have a First and Last Name.
- Each employee must be a member of a group.
- Each group can offer 1 to 3 types of plans. Medical, Dental, or Vision
- Each employee can enroll in any of the plans.
- Each plan has a start and end data.

![Figure 2](/data.png)



## Requirements

### Front-End
**Stories**  
- As a Noyo admin I want to create a group so I can add employees to the group.
- As a Noyo admin I want to create employees so I can enroll them in coverage
- As a Noyo admin I want to filter employees by first and last name so that i can identify potential duplicates.
- As a Noyo admin I want to update employee names so that I can correct errors.
- As a Noyo admin I want to delete employees when their coverage has ended.
- As a Noyo admin I want to enroll an employee in Medical Dental or Vision coverage as offered by its group.
- As a Noyo admin I want to see a list of groups and all the associated employees of the group.
- As a Noyo admin I want to see an individual employee and the list of their enrollments.


**Technical Requirements:**  
- React.js: Build the user interface using React.js.
- Next.js: Use Next.js to handle server-side rendering and routing.
- Tailwind CSS: Style the application using Tailwind CSS.
- Authentication: Implement authentication using a service like Firebase, Auth0, or a custom solution.

**Back-End:**

**API Routes:**
    Use Next.js API routes to create a RESTful API for managing all domain objects. 
    Implement CRUD operations (Create, Read, Update, Delete) for employees and enrollments  
**Database:** Store data in a database (e.g., MongoDB, PostgreSQL, or a cloud solution like Firebase Firestore).  
**Authorization:** Ensure that API routes are protected and only authenticated users can access their tasks.

**Technical Requirements:**

**TypeScrip*: Use TypeScript for type safety.  
**State Managemen**: Use React's Context API or a state management library (e.g., Redux) to manage the application state.  
**Code Quality**: Write clean, maintainable code following SOLID principles and best practices. Include comments where necessary and ensure code is well-structured.  
**Testing**: Implement unit and integration tests for key components and API routes.  


# Live Coding Extention

Live Coding Extention -
During your onsite you will discuss and demo your take home solution. As part of this there will be a live coding entension where you will implement additional functionality.


Add the ability to include multiple enrollment segments to specific lines of coverage. Your solution should allow Noyo admins to add enrollments to employee.

eg.
Each enrollment for a line of coverage has some metadata, eg. plan_id. With that this means that you can add segments to the an employees line.

Hint
segments dont overlap
add anywhere in the list
incoming segment wins

![Figure 2](/extension.png)


