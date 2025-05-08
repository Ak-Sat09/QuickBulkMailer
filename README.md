#QuickBulkMailer
A Java Spring Boot-based application for sending bulk emails using SMTP. It allows you to send personalized emails to a list of up to 500 recipients per day. Using Hibernate ORM for database interactions and MySQL for storing recipient data, this app enables a seamless, one-click solution for mass email outreach.

🔧 Tech Stack:
Java Spring Boot: Backend framework to manage the application logic.

Hibernate: ORM framework to interact with the MySQL database.

MySQL: Database to store email recipient details.

SMTP: Used for sending emails via Gmail, Outlook, or custom SMTP servers.

REST API: Exposes endpoints for sending bulk emails, fetching recipients, etc.

Thymeleaf: (Optional) For rendering HTML email templates.

📄 Description:
QuickBulkMailer allows users to upload a list of email addresses and send personalized emails to up to 500 recipients per day via SMTP. With a user-friendly REST API and a robust backend powered by Spring Boot, this app is ideal for startups, marketing campaigns, or individual developers needing efficient email outreach.

🔑 Features:
Send up to 500 emails/day via SMTP

Bulk email dispatch from a list stored in MySQL

REST API to manage recipients, email templates, and send bulk emails

Email Logging: Tracks email delivery success or failure

Database Management: Store recipient data using Hibernate and MySQL

SMTP Integration: Use Gmail or custom SMTP servers to send emails

📁 Folder Structure:
css
Copy
Edit
QuickBulkMailer/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   ├── com/
│   │   │   │   └── quickbulkmailer/
│   │   │   │       ├── controller/
│   │   │   │       ├── model/
│   │   │   │       ├── repository/
│   │   │   │       ├── service/
│   │   │   │       ├── smtp/
│   │   │   │       └── QuickBulkMailerApplication.java
│   │   └── resources/
│   │       ├── application.properties
│   │       └── static/
│   └── test/
├── pom.xml
└── README.md
⚙️ How to Run:
Clone the repository:

bash
Copy
Edit
git clone https://github.com/your-username/QuickBulkMailer.git
cd QuickBulkMailer
Configure application.properties:
In src/main/resources/application.properties, add your SMTP and MySQL configurations:

ini
Copy
Edit
spring.datasource.url=jdbc:mysql://localhost:3306/quickbulkmailer
spring.datasource.username=root
spring.datasource.password=password
spring.jpa.hibernate.ddl-auto=update
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

smtp.host=smtp.gmail.com
smtp.port=587
smtp.user=your_email@gmail.com
smtp.pass=your_app_password
Install dependencies:
If you're using Maven, run:

bash
Copy
Edit
mvn clean install
Run the application:

bash
Copy
Edit
mvn spring-boot:run
Access the app:
The REST API will be running on http://localhost:8080. You can use endpoints to manage recipients and send emails.

🔑 API Endpoints:
POST /emails/send: Send bulk emails to a list of recipients.

GET /emails/recipients: Fetch the list of stored recipients.

POST /emails/recipients: Add new recipients to the database.

🚀 Future Enhancements:
Add support for HTML email templates using Thymeleaf.

Implement email scheduling to send emails at specific times.

Add email tracking to monitor open and click rates.

Implement user authentication for managing campaigns.
