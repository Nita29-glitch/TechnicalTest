This Project implements a customer CRUD using ASP.NET Core It consists of two parts:
1. BackEnd Part=> ASP.NET Core Web API that provides endpoints for managing customer data (Create, Read, Update, Delete).
2. Frontend Part=> ASP.NET Core MVC application that interacts with the backend API to perform CRUD operations on customers.

Features :
1)View all customers
2)Add new customer
3)Update the existing customer
4)Delete an existing customer
5)communicate backend and frontend with HTTPClient

Prerequisites:
Here Used Visual Studio 2022 and SQL Server 2019.

configure the database connection string in appsettings.json of API_For_Backend application.

EF core for database migration:
open Package manager console and perform:
1)Add-Migration InitialCreat
2)Update-Database

Run both backend and front at the same time

BackEnd Part(BackEnd API):
1)Once you run the project the swagger UI will be available as https://localhost:{apiport}/swagger
	eg: https://localhost:7219/swagger/index.html
2)Test the API using following end points:    
	i)GET/api/customer -to retrieve all customers.
	ii)GET/api/customer/{id} - to retrieve the single cuatomer by Id.
	iii)POST/api/customer -to create a new customer.
	iv)PUT/api/customer/{id} -to update an existing customer by Id.
	v)DELETE/api/customer/{id} = to delete an existing customer by Id.
Frontend Part(UI Part):
1)The front end can be accesse using http://localhost:{port} 
	eg:https://localhost:7296/
2)It provides UI for managing customers using the CRUD operations.
	i)Customer list
	ii)Add Customer -open a create page to add customer.
	iii)Edit customer:open a edit page to the selected customer.
	iv)Delete cuatomer/:to delete the the selected customer.
	v)back to list: to go back to list.
3)Perform CRUD and check in the database

@Nita Kalukhe
