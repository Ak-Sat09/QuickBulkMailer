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
