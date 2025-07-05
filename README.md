# Product Management CRUD Application ASP.NET Core MVC Web Application

Load:

![image alt](https://github.com/Muzammil-khan-uni/Product-Management-CRUD-Application-ASP.NET-Core-MVC-Web-Application/blob/main/Output%20SS/Load.png)

ADD:

![image alt](https://github.com/Muzammil-khan-uni/Product-Management-CRUD-Application-ASP.NET-Core-MVC-Web-Application/blob/main/Output%20SS/ADD.png)
![image alt](https://github.com/Muzammil-khan-uni/Product-Management-CRUD-Application-ASP.NET-Core-MVC-Web-Application/blob/main/Output%20SS/ADD2.png)


UPDATE:

![image alt](https://github.com/Muzammil-khan-uni/Product-Management-CRUD-Application-ASP.NET-Core-MVC-Web-Application/blob/main/Output%20SS/UPDATE.png)
![image alt](https://github.com/Muzammil-khan-uni/Product-Management-CRUD-Application-ASP.NET-Core-MVC-Web-Application/blob/main/Output%20SS/UPDATE2.png)

DELETE:

![image alt](https://github.com/Muzammil-khan-uni/Product-Management-CRUD-Application-ASP.NET-Core-MVC-Web-Application/blob/main/Output%20SS/DELETE.png)
![image alt](https://github.com/Muzammil-khan-uni/Product-Management-CRUD-Application-ASP.NET-Core-MVC-Web-Application/blob/main/Output%20SS/DELETE2.png)

DETAILS:

![image alt](https://github.com/Muzammil-khan-uni/Product-Management-CRUD-Application-ASP.NET-Core-MVC-Web-Application/blob/main/Output%20SS/DETAILS.png)

This CRUD (Create, Read, Update, Delete) web application built using ASP.NET Core MVC framework. It allows users to manage a list of products — each with a name, price, and description — by performing basic operations such as adding new products, viewing details, editing existing records, and deleting them.

The application follows the MVC (Model-View-Controller) architecture pattern and uses Entity Framework Core for database interaction. Bootstrap 5 is used for UI styling to create a clean, responsive user interface.

🏗️ Architecture: MVC (Model - View - Controller)

✅ Model Layer:

Product.cs

Defines the structure of the Product entity with properties:

Id: Primary key.

Name: Required field for product name.

Price: Required field for product price.

Description: Optional product description.

AppDbContext.cs

Configures Entity Framework's DbContext to interact with the Products table in the database.

ErrorViewModel.cs

Used for error handling and debugging during development.

✅ View Layer (Razor Pages):

All views are created using Razor syntax with Bootstrap 5 styling:

_Layout.cshtml

Shared layout with Bootstrap, header, and container for rendering views.

Index.cshtml

Displays a list of all products in a table with buttons to:

Edit

Delete

View Details

Add New Product

Create.cshtml

Form to create a new product (fields for Name, Price, Description).

Edit.cshtml

Form to edit an existing product's details.

Delete.cshtml

Confirmation page to delete a product.

Details.cshtml

Displays complete details of a single product.

✅ Controller Layer:

ProductsController.cs

Manages all product-related actions:

Index() – Lists all products.

Details(int?) – Shows full product information.

Create() – Displays the create form.

[HttpPost] Create(Product) – Adds the new product to the database.

Edit(int?) – Displays the edit form for the selected product.

[HttpPost] Edit(int, Product) – Updates the product in the database.

Delete(int?) – Displays confirmation page for deleting.

[HttpPost] DeleteConfirmed(int) – Deletes the product from the database.

ProductExists(int) – Helper to check if a product exists.

HomeController.cs

Contains default home actions (Index, Privacy, Error).

🧪 Technologies Used:

| Component    | Technology              |
| ------------ | ----------------------- |
| Framework    | ASP.NET Core MVC        |
| Language     | C#                      |
| ORM          | Entity Framework Core   |
| View Engine  | Razor Pages (.cshtml)   |
| UI Framework | Bootstrap 5             |
| IDE          | Visual Studio / VS Code |
| Database     | SQL Server (or SQLite)  |

🛠️ Key Features:

🔍 View a list of all products

➕ Add a new product

🖊️ Edit existing product details

❌ Delete products

📄 View product details

✅ Form validation using DataAnnotations

💾 Uses EF Core for seamless data handling

🎨 Clean and responsive Bootstrap UI

