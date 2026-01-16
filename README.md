# HibernateProductInventorySystem

## Description
A **console-based Product Inventory Management System** developed using **Java, Hibernate ORM, and JPA**, connected to a **PostgreSQL database**.  
This project demonstrates the use of **JPA inbuilt methods** and **HQL (JPQL) queries** to manage, analyze, and maintain product inventory data.

## Database Details
- **Database Name:** inventory_db
- **ORM Framework:** Hibernate (JPA)
- **Configuration:** persistence.xml (META-INF)

## Entity: Product

### Fields
- productid (Primary Key)
- productname
- category
- price
- quantity
- status (AVAILABLE / OUT_OF_STOCK)

## Features

### JPA Operations (Mandatory)
- Add product using `persist()`
- Search product by ID using `find()`
- Update product price and quantity using `merge()`
- Delete product by ID using `remove()`

### HQL (JPQL) Operations (Mandatory)
- Fetch all products
- Fetch products by category (dynamic)
- Fetch products with quantity less than N (dynamic)
- Increase product price by 50 for a category (dynamic)
- Delete products with zero quantity
- Count total products
- Fetch product by product name (dynamic)
- Automatically update product status to `OUT_OF_STOCK` when quantity becomes 0

## Technologies Used
- Java
- Hibernate ORM
- JPA
- PostgreSQL
- Maven
- pgAdmin 4
- Eclipse / IntelliJ IDEA

## Project Structure
HibernateProductInventorySystem/
├─ src/
│ └─ main/
│ ├─ java/
│ │ └─ com/example/hibernate/
│ │ ├─ Product.java
│ │ ├─ ProductDAO.java
│ │ └─ InventoryApp.java
│ └─ resources/
│ └─ META-INF/
│ └─ persistence.xml
├─ pom.xml
├─ README.md
└─ .gitignore
