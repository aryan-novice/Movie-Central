<img width="1887" height="1002" alt="Screenshot 2025-12-27 123246" src="https://github.com/user-attachments/assets/a8725e98-06bc-4092-acd5-83ebd2d0344c" />



<img width="1896" height="1013" alt="Screenshot 2025-12-27 123158" src="https://github.com/user-attachments/assets/7360fef3-5f5d-4b12-a26b-de6aeaff6c1b" />



<img width="1896" height="1020" alt="Screenshot 2025-12-27 123506" src="https://github.com/user-attachments/assets/24beb573-6d27-4dfe-b714-df0b7a0b4604" />



<img width="1886" height="1011" alt="Screenshot 2025-12-27 123541" src="https://github.com/user-attachments/assets/e8df2722-9b0a-469b-9e34-42c6d89099cd" />



<img width="1893" height="998" alt="Screenshot 2025-12-27 123403" src="https://github.com/user-attachments/assets/26eb392d-3545-4c0b-b0df-3996351aef65" />



<img width="1036" height="785" alt="Screenshot 2025-12-27 123616" src="https://github.com/user-attachments/assets/0f5398a8-29bb-4df7-967a-5175a5ba3859" />



Movie Central – A Movie Management System
 
Project Date:June 2024  
Tech Stack: Java, MySQL, JDBC, REST API, JSON

Overview
Movie Central is a Java-based backend application designed to manage a collection of movies and users. It allows you to perform CRUD operations on movies, manage user data, and integrate with external APIs to fetch real-time movie information. The system uses MySQL for data storage, JDBC for database connectivity, and JSON for API communication.

 Features
 1.Movie Management:
  Add, update, delete, and search for movies stored in the database.

 2.User Management:  
  Maintain records of users and track their interactions with the movie system.

  3.REST API Integration:
  Connects to third-party APIs (like TMDB or OMDb) to fetch dynamic movie details such as posters, ratings, and release info.

  4.Data Storage (MySQL + JDBC): 
  Efficient relational database design with JDBC-based operations for real-time access and manipulation.

   5.JSON Support:  
  Handles all API data exchange in JSON format, enabling modern and lightweight communication.

  Technologies Used

- Programming Language:Java  
- Database: MySQL  
- Connectivity:JDBC  
- API Protocol:REST  
- Data Format:JSON






🟢 Application Startup Flow

IMDB.java
   ↓
User_login.java
   ↓
[Login Success]
   ↓
user_home.java



🔐 Login Flow

User_login.java
   ↓
Validate Input
   ↓
DBLoader → MySQL
   ↓
✔ Valid → user_home
✖ Invalid → Error Message



📝 Sign-Up Flow

user_sign_up.java
   ↓
Validate Fields
   ↓
DBLoader → Insert User
   ↓
Redirect to Login



🎬 Movie Fetching Flow (API Based)

User clicks category
   ↓
TopTrending / TopRated / TopUpcoming
   ↓
MyClient.java
   ↓
HTTP API Request
   ↓
JSON Response
   ↓
Parse JSON
   ↓
Display movies (Posters, Titles, Dates)




👤 Profile Management Flow

manage_profiel.java
   ↓
Fetch user details
   ↓
Update profile
   ↓
DBLoader → Update DB




🔑 Change Password Flow

Change_password.java
   ↓
Validate old password
   ↓
DBLoader → Update password
   ↓
Success / Failure Message



