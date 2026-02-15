# Secure-Authentication-System-

This project is a secure authentication system I built using Python and SQLite. The aim of the project was to understand how user credentials should be handled securely in a real application, rather than just learning how to store the data in a database.

The system focuses on safe password handling , basic database design, and separating responsibilities between different parts of the application.

# Why I Built This Project

I wanted to build something that reflects real world security practices rather than continue to build simple python scripts. Authentication is a core part of almost every application, and poor implementation can lead to serious vulnerabilities.

This project helped me understand:

* Why passwords should never be store in plain text
* How hashing protects user credentials
* How databases should be structured for authentication systems
* How to seperate database logic from application logic

# How the System Works

* A SQLite database is created programmaticaly if it does not already exist
* User credentials are stored only after the password is hashed
* User creatiionand database setup are handled in seperate files

# Security Considerations

Security was a key focus throughout the project:

* Passwords are hashed using SHA-256 before being stored
* Plain text passwords are never written to the database
* Parameterised SQL queries are used to prevent SQL injection
* The SQLite database file is excluded from GitHub to avoid exposing sensitive data
* Database schema creation is handled in code so the system can be safely recreated

# Technologies and Concepts Used

* Python
* SQLite
* SQL table design
* Password hashing
* Seperation of concerns
* Basic secure coding principles

# What I Learned

This project helped me understand that secure software development is not just about making code work, but about making it safe and maintainable.

I also learned the importance of:

* Thinking about how data could be misused
* Designing systems with security in mind from the start
* Structuring code in a way that mirrors real applications

# Possible Improvements

If I were to extend this project I would:

* I would implement limited login attempts that makes you try again after a few hours
* Enrypt the database file
* Add password salting and stronger hashing methods
* Add role based access control

# Disclaimer

This project was created for educational purposes only. All testing was perfromed using test data, and no real user credentials are stored or shared.
