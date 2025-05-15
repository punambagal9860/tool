# 🧩 Jenkins Web Application – Date and Time Display

This is a simple Java-based web application built using **Servlets** and **JSP**, deployed on an **Apache Tomcat server**.  
The project demonstrates how to display the current date and time using Servlets and integrates with a **Jenkins CI/CD pipeline** for automated build and deployment.

---

## 🚀 Features

- A homepage (`index.jsp`) with a navigation link.
- A Servlet (`DateServlet.java`) mapped to `/dateurl` that displays the current system date and time.
- Integration with Jenkins for:
  - Automated build using Maven or Gradle.
  - Deployment to Apache Tomcat.
- Educational value:
  - Demonstrates use of Java Servlets and JSP.
  - Shows basic CI/CD configuration with Jenkins.

---

## 🛠️ Technologies Used

- Java (Servlet API)
- Jakarta Servlet (`jakarta.servlet.http`)
- JSP (JavaServer Pages)
- Apache Tomcat (v9 or v10)
- Jenkins (for CI/CD)
- Maven or Gradle (build tool)
- Git & GitHub


---

## ⚙️ How It Works

1. User accesses the home page (`index.jsp`).
2. The homepage contains a link labeled **"Show Date and Time"**.
3. Clicking the link sends a GET request to `/dateurl`.
4. `DateServlet` processes the request and responds with the **current system date and time**.

---

## 🧪 Deployment Using Jenkins (CI/CD)

To integrate and deploy this application via Jenkins:

1. **Push your project to GitHub.**
2. **In Jenkins:**
   - Create a new Freestyle or Pipeline job.
   - Connect it to your GitHub repository.
   - Use Maven or Gradle to build the project.
   - Generate the `.war` file.
   - Deploy the `.war` to the Apache Tomcat server:
     - Using **Deploy to Container plugin**, or
     - With custom **shell scripts**.
3. **Configure CI/CD triggers:**
   - Use **Poll SCM** or **GitHub Webhooks** to auto-trigger builds on code updates.

> On every successful build, Jenkins will automatically deploy the latest `.war` to the Tomcat server.

---

## 📚 Learning Outcomes

- Java Web Development with Servlets and JSP.
- Application packaging and deployment using Maven or Gradle.
- Setting up and configuring Jenkins pipelines.
- CI/CD automation in a real-world scenario.

---
## 🗂️ Project Structure
/YourProjectName
│
├── src/main/java/com/nt/servlet/DateServlet.java
├── webapp/index.jsp
├── WEB-INF/web.xml # (if using XML-based configuration)
├── pom.xml / build.gradle # (build tool)


## ⚙️ How It Works

1. User accesses the home page (`index.jsp`).
2. The homepage contains a link labeled **"Show Date and Time"**.
3. Clicking the link sends a GET request to `/dateurl`.
4. `DateServlet` processes the request and responds with the **current system date and time**.


## 📚 Learning Outcomes

- Java Web Development with Servlets and JSP.
- Application packaging and deployment using Maven or Gradle.
- Setting up and configuring Jenkins pipelines.
- CI/CD automation in a real-world scenario.


## 🙋‍♂️ Contributions

Feel free to fork the repository and submit pull requests. Issues and improvements are welcome!









