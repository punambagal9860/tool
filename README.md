Jenkins Web Application - Date and Time Display
This is a simple Java-based web application built using Servlets and JSP, deployed on 
a Tomcat server. The project demonstrates how to display the current date and time using Servlets 
and integrates with Jenkins CI/CD pipeline for automated build and deployment.

1> Description
This project is a basic Java web application that includes:

A homepage (index.jsp) with a link.

A Servlet (DateServlet.java) mapped to /dateurl that displays the current system date and time.

Integration with Jenkins for automatic deployment and build.

The project serves as a hands-on learning demo for:

Java Servlets and JSP

Deployment using Apache Tomcat

Jenkins pipeline configuration for CI/CD

2.Technologies Used
Java (Servlet API)

Jakarta Servlet (jakarta.servlet.http)

Apache Tomcat (v9 or v10)

JSP (JavaServer Pages)

Jenkins (for CI/CD)

Maven or Gradle (build tool, if used)

Git & GitHub

3. Project Structure
pgsql
Copy
Edit
/YourProjectName
│
├── src/main/java/com/nt/servlet/DateServlet.java
├── webapp/index.jsp
├── WEB-INF/web.xml (if using XML configuration)
│
└── pom.xml / build.gradle (if using Maven/Gradle)
⚙️ How It Works
User accesses the home page (index.jsp).

User clicks on the link "Show Date And Time".

The link triggers a GET request to /dateurl.

DateServlet processes the request and responds with the current date and time.

3. Deployment Using Jenkins
This application can be integrated into a Jenkins pipeline using the following steps:

Create a GitHub repository and push your project.

Configure Jenkins job:

Connect to your GitHub repo.

Use Maven/Gradle to build.

Deploy the .war file to Tomcat (using plugins or shell scripts).

Configure Poll SCM or Webhook for auto-triggering builds on every code change.

On successful build, Jenkins deploys the latest version to the Tomcat server.
