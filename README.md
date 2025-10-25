**E-commerce Web Application**

A E-commerce application using Spring Boot (Java) for the backend. This application demonstrates the integration of RESTful APIs with a modern frontend stack, ideal for learning and demonstration purposes.

📁 **Project Structure**
SpringBoot-Ecommerce-main/
├── Ecommerce-Backend/       # Spring Boot REST API backend
├── Ecommerce-Frontend/      # React + Vite frontend application

🧩** Backend - Spring Boot**
🔧 Technologies Used
Java 17+
Spring Boot
Spring Data JPA
MySQL (can be adapted)
Maven

📂 **Backend Directory Structure**
Ecommerce-Backend/
├── controller/      # REST endpoints
├── model/           # JPA entity classes
├── repo/            # Spring Data JPA interfaces
├── service/         # Business logic
├── resources/
│   ├── application.properties
│   └── data1.sql
└── pom.xml          # Maven build config

⚙️ **Setup Instructions**
1.Database Setup:

Create a MySQL database, e.g., ecomdb.

Update application.properties:

spring.datasource.url=jdbc:mysql://localhost:3306/ecomdb
spring.datasource.username=root
spring.datasource.password=yourpassword
spring.jpa.hibernate.ddl-auto=update

2.Run the App:

cd Ecommerce-Backend
mvn spring-boot:run
Data Initialization:

3.On first run, data1.sql inserts seed product data into your DB.

📡 **REST API Endpoints**
Method	Endpoint	Description
GET	/products	Fetch all products
GET	/products/{id}	Get product by ID
POST	/products	Add new product
PUT	/products/{id}	Update product
DELETE	/products/{id}	Delete product

▶️ **Getting Started**
Install dependencies:

1.cd Ecommerce-Frontend
npm install

2.Run the app:

npm run dev
This will launch the frontend at http://localhost:5173.

3.Connect to Backend:

Update the backend URL in API service files (usually inside src/ or src/services/) if needed:

axios.get('http://localhost:8080/products')

🧩 Features
1.Product List (from Spring Boot backend)
2.Fully responsive UI
3.Easy integration with further features (cart, checkout, login)
