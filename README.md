# **VOTING APP** :

This is a backend application for a voting system where users can vote for candidates. It provides functionalities for user authentication, candidate management, and voting.

## FEATURES :

- User sign up and login with Aadhar Card Number and password.
- User can view the list of candidates.
- User can vote for a candidate (only once).
- Admin can manage candidates (add, update, delete).
- Admin cannot vote.

# **API ENDPOINTS**

## AUTHENTICATION

### Sign Up

- POST /signup : endpoint to sign up a new user.

### Login

- POST /login : endpoint to login an existing user.

## CANDIDATES

### Get Candidates

- GET /candidate : endpoint to get the list of the candidates.

### Add Candidate

- POST /candidate : adds a new candidate(_Only Admin is authorized_).

### Update Candidate

- PUT /candidate/:id : Updates a candidate by using id(_Only admin is authorized_).

### Delete Candidate

- DELETE /candidate/:id : Deletes a candidate by id(_Only admin is authorized_).

## VOTING

### Get Vote Count

- GET /candidate/vote/count: Get the count of votes for each candidate.

### Vote for Candidate

- POST /candidate/vote/:id: Vote for a candidate (_Only User is authorized_).

## User Profile

### Get Profile

- GET /user/profile: Get user profile information
