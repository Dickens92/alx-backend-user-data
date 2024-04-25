0x03. User authentication service TASKS

0. a SQLAlchemy model named User for a database table named users (by using the mapping declaration of SQLAlchemy).

1. the DB class provided below to implement the add_user method.

2. implement the DB.find_user_by method

3. implement the DB.update_user method that takes as argument a required user_id integer and arbitrary keyword arguments, and returns None.

4. define a _hash_password method that takes in a password string arguments and returns bytes

5. set up a basic Flask app

6. implement the end-point to register a user. Define a users function that implements the POST /users route.

7. implement the Auth.valid_login method. It should expect email and password required arguments and return a boolean.

8.  implement a _generate_uuid function in the auth module. The function should return a string representation of a new UUID. Use the uuid module.

9.  implement the Auth.create_session method. It takes an email string argument and returns the session ID as a string.

10. implement a login function to respond to the POST /sessions route.

11. implement the Auth.get_user_from_session_id method. It takes a single session_id string argument and returns the corresponding User or None.

12. implement Auth.destroy_session. The method takes a single user_id integer argument and returns None.

13. implement a profile function to respond to the GET /profile route.

14. implement a logout function to respond to the DELETE /sessions route.

15. implement the Auth.get_reset_password_token method. It take an email string argument and returns a string.

16.  implement the Auth.update_password method. It takes reset_token string argument and a password string argument and returns None.

17. implement the update_password function in the app module to respond to the PUT /reset_password route

18. End-to-end integration test
