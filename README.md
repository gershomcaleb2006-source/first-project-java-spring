# Spring Framework Application - Task 1
**Author:** Gershom Goldlin Ranjit
**University:** Vistula University

## Project Overview
This repository contains a fully functional Java web application built using the Spring Framework (Spring Boot). This project was completed as "Task 1" for university coursework to demonstrate a basic understanding of Spring MVC architecture, controllers, and serving dynamic web content.

### Technologies Used
* **Java**
* **Spring Boot** (Spring Web)
* **Maven** (Dependency Management)
* **Thymeleaf** (Template Engine for HTML views)

---

## Application Features & Use Cases

This application demonstrates the ability to map HTTP GET requests to specific Java methods and return both raw text and rendered HTML views.

### Endpoint 1: Basic Text Response
* **Method:** `GET`
* **Path:** `/`
* **Description:** When a user navigates to the root URL, the application uses the `@ResponseBody` annotation to return a simple confirmation string.
* **Response:** "Hello Vistula, in my first Spring controller."

**Screenshot:**
<img width="2553" height="1599" alt="Screenshot 2026-04-26 162606" src="https://github.com/user-attachments/assets/68e4d73e-f8b6-4611-bf7c-8aea4476a3d1" />


### Endpoint 2: Dynamic HTML View (Thymeleaf)
* **Method:** `GET`
* **Path:** `/greeting?name={value}`
* **Description:** This endpoint accepts a query parameter (`name`). The Controller uses a `Model` to pass this parameter to a Thymeleaf HTML template (`greeting.html`). The template renders a personalized greeting along with CSS formatting and a static image (the Vistula University logo).
* **Default Behavior:** If no name is provided in the URL, it defaults to "World".

**Screenshot:**
<img width="2559" height="1599" alt="Screenshot 2026-04-26 162452" src="https://github.com/user-attachments/assets/57b454ba-ecfe-48f8-a76c-c65d619292bd" />


---

## How to Run This Application
1. Clone the repository to your local machine.
2. Open the project in IntelliJ IDEA (or your preferred Java IDE).
3. Ensure Maven has downloaded the required dependencies (`spring-boot-starter-web`, `spring-boot-starter-thymeleaf`).
4. Run the `FirstProjectJavaSpringApplication.java` main class.
5. Open a web browser and navigate to `http://localhost:8080`.
