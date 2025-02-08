### **FastAPI Interview Questions and Answers**  

#### **1. Installing and Introducing Python (venv and Flask) & Starting FastAPI Application**  

1. **What is a virtual environment, and why is it important in FastAPI development?**  
   - A virtual environment (venv) isolates dependencies for a project, preventing conflicts between different Python projects. It ensures a consistent development environment.  

2. **How do you install FastAPI, and what are its key dependencies?**  
   - Install FastAPI using `pip install fastapi` and `pip install "uvicorn[standard]"` for the server. Dependencies include Starlette (for web handling) and Pydantic (for data validation).  

3. **What is the purpose of Uvicorn in FastAPI applications?**  
   - Uvicorn is an ASGI server used to run FastAPI applications asynchronously, making them faster and more efficient.  

4. **How does FastAPI differ from Flask in terms of performance and functionality?**  
   - FastAPI is asynchronous, built for speed using ASGI, and has built-in type validation with Pydantic, whereas Flask is synchronous and requires additional libraries for async and validation.  

5. **What are the main features of FastAPI that make it suitable for modern web development?**  
   - It provides automatic OpenAPI documentation, built-in data validation, async support for high performance, and easy integration with databases and frontend applications.  

#### **2. CRUD Operations**  

6. **What does CRUD stand for, and how does FastAPI support it?**  
   - CRUD stands for Create, Read, Update, and Delete. FastAPI provides decorators (`@post`, `@get`, `@put`, `@delete`) to handle these operations easily.  

7. **What HTTP methods are commonly used for CRUD operations in FastAPI?**  
   - `POST` (Create), `GET` (Read), `PUT/PATCH` (Update), and `DELETE` (Delete).  

8. **How do path and query parameters work in FastAPI for retrieving data?**  
   - Path parameters (`/items/{id}`) are part of the URL, while query parameters (`/items?name=abc`) are passed in the URL query string. FastAPI automatically parses them.  

9. **What is the purpose of response models in FastAPI CRUD operations?**  
   - Response models ensure data consistency and security by defining the structure of returned data using Pydantic schemas.  

10. **How does FastAPI handle request validation for creating and updating records?**  
   - FastAPI uses Pydantic models to validate and parse request data automatically, ensuring correct data types and constraints.  

#### **3. DB Integrations (Movies) & Schemas and Models (Movies)**  

11. **What is the role of SQLAlchemy in FastAPI database integration?**  
   - SQLAlchemy is an ORM that helps interact with databases in a Pythonic way, making database queries easier and more efficient.  

12. **How do Pydantic schemas help in defining API request and response models?**  
   - Pydantic ensures type validation and serialization of data, providing a structured way to define API request and response models.  

13. **What is the difference between ORM models and Pydantic schemas in FastAPI?**  
   - ORM models (SQLAlchemy) represent database tables, while Pydantic schemas define request and response data validation.  

14. **How does FastAPI support asynchronous database queries?**  
   - FastAPI supports async database operations using `async def` and libraries like `Databases` or `SQLAlchemy with async engines`.  

15. **Why is dependency injection useful in FastAPI for database operations?**  
   - Dependency injection ensures better modularity, reusability, and testability by passing database sessions or services as function parameters.  

#### **4. Updating CRUD Operations (Movies)**  

16. **What is the difference between PUT and PATCH methods when updating data?**  
   - `PUT` replaces the entire resource, whereas `PATCH` updates only specific fields of an existing resource.  

17. **How do you ensure data validation when updating a movie record in FastAPI?**  
   - Use Pydantic models with optional fields for `PATCH` and required fields for `PUT` to validate input data.  

18. **What are the advantages of using Pydantic models for update operations?**  
   - They enforce type safety, prevent invalid data updates, and provide automatic serialization and validation.  

#### **5. Adding CORS and Showing Data in Frontend**  

19. **What is CORS, and why is it important in FastAPI applications?**  
   - CORS (Cross-Origin Resource Sharing) allows browsers to accept API requests from different domains. FastAPI provides `CORSMiddleware` to handle it.  

20. **How does FastAPI allow frontend applications to consume its API data?**  
   - FastAPI serves data as JSON, which can be consumed by frontend frameworks like React or Vue via HTTP requests using `fetch` or Axios.
