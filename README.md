# Project Title

Create an API for social networking application using Django Rest Framework with
below functionalities

## Description

The Social Networking Application is a platform designed to facilitate social interactions between users. It provides features such as user authentication, friend requests, and user profiles. Users can sign up for an account, log in securely, and search for other users to connect with. They can send friend requests to establish connections and manage their list of friends.

## Installation
create virtual environment ```python -m venv venv```
activate the environment ``` venv/script/activate ```

## API Documentation
The project encompasses the following features:

## User Authentication:
### Signup:
Users can sign up using only their email (no OTP verification required).
The email format must be valid.
### Login:
Users can log in using their email and password.
The email should be case-insensitive.
## Authentication Requirement:
All APIs, except for signup and login, require users to be authenticated.

## Search Functionality:
### Search Users by Email or Name:
Users can search for other users using a single keyword.
The search results are paginated, with a maximum of 10 records per page.
### Search by Email:
If the search keyword exactly matches an email, the API returns the user associated with that email.
### Search by Name:
If the search keyword matches any part of a user's name, the API returns a list of users whose names contain the keyword.

## Friend Request Management:
### Send Friend Request:
- Users can send friend requests to other users.
- A user cannot send more than 3 friend requests within a minute.
### Accept/Reject Friend Request:
 - Users can accept or reject friend requests received from other users.
 
## Friendship and Requests Listing:
### List Friends:
Users can retrieve a list of all users who have accepted their friend requests.
### List Pending Friend Requests:
Users can view a list of friend requests they have received but not yet responded to.
