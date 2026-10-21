## What Did I Build?
A **Full Stack web application** that connects three components: a user interface, a backend server, and a database.

Designed and developed a Full-Stack financial management web application using React to build a responsive user interface and .NET 10 (C#) for a robust backend. Implemented Entity Framework Core with SQLite for local data persistence, establishing a decoupled, efficient, and maintainable architecture.


<p align="center">
  <img
    src="https://github.com/user-attachments/assets/709e7fc4-4ae5-4b00-ab30-4db2af31f73d"
    width="250"
    alt="Arquitectura Full Stack de DotNet Financial Tracker"
  />
</p>

### 🎨 Frontend — React
The frontend is the visual part of the application. It is what users see and interact with through their web browser.
### ⚙️ Backend — C# and .NET 10
The backend is the server responsible for processing requests from the frontend.
I used SQLite as the database, which can store information in a local file named `financial.db`.

## Creating the Main Project Folder
Before building the application, we need to organize the files inside a main project directory.
**Command used in the terminal:**


<p align="center">
<img width="65%"   alt="01" src="https://github.com/user-attachments/assets/c5775623-af42-4cc3-88ca-d66280e01a13" />
</p>


 
```
mkdir -p Documents/DotNet-Financial-Tracker
```
- `mkdir`: creates a directory.
- `-p`: creates any necessary parent directories and avoids errors if they already exist.
- `Documents/DotNet-Financial-Tracker`: specifies the path and name of the directory.

## Creating the Backend with .NET 10

Once we are inside the main project directory, we create the backend.

**Command used in the terminal:**

```bash
dotnet new webapi -o Backend
```
This command generates the initial server structure, including configuration files and C# source code.

- `dotnet`: runs the .NET command-line tool.
- `new`: creates a new project from a template.
- `webapi`: selects the template for building a web API.
- `-o Backend`: creates the project files inside a directory named `Backend`.

## Installing the SQLite Dependencies

To allow the backend to communicate with SQLite through Entity Framework Core, I installed the following packages.
**Commands used in the terminal:**

```bash
dotnet add package Microsoft.EntityFrameworkCore.Sqlite
dotnet add package Microsoft.EntityFrameworkCore.Design
```
The `Microsoft.EntityFrameworkCore.Sqlite` package allows Entity Framework Core to use SQLite as a database provider.

**Second Package: Microsoft.EntityFrameworkCore.Design**
The `Microsoft.EntityFrameworkCore.Design` package provides design-time tools required for development tasks, such as managing Entity Framework Core migrations.

**What Did We Achieve with These Commands?**
We added the required dependencies to the .NET project to integrate the database and use the necessary Entity Framework Core tools.
## Setting Up the Frontend with React

The frontend is responsible for displaying the graphical interface and allowing users to interact with the application.

**First, I navigated to the frontend directory**

```bash
cd Frontend
```
**Then, I installed the project dependencies:**

```bash
npm install
```

**What Does This Command Do?:**
- `npm`: is the package manager for Node.js.
- `install`: installs the dependencies declared in the `package.json` file.

Next, I installed two libraries used in the user interface.

**Command used in the terminal:**

```bash
npm install lucide-react recharts
```
**What Are These Libraries Used For?**
- `lucide-react`: allows us to add icons to React components.
- `recharts`: allows us to create charts and represent information visually.

## Running the Backend Server

To start the backend server, I navigated to the `Backend` directory and executed the following command.

```bash
cd Backend
```

```bash
dotnet run
```
**What Does dotnet run Do?**
1. Builds the project if necessary.
2. Runs the .NET application.
3. Starts the web server configured in the project.
4. Allows the backend to receive HTTP requests while the process is running.

**What Does This Command Mean?**
- `npm`: runs the Node.js package manager.
- `start`: executes the script named `start` defined in the `package.json` file.

**Running the Frontend Server**
The frontend and backend run as two independent processes. Therefore, we need to keep them running in separate terminal windows.

I opened a second terminal and navigated to the frontend directory.

```bash
cd Frontend
```

Then, I executed the following command.

```bash
npm start
```
<p align="center">
<img width="65%" height="1000" alt="Captura de pantalla (1233)" src="https://github.com/user-attachments/assets/345176fd-ef8c-4016-8844-d268154128ac" />
</p>

<p align="center">
<img width="65%" height="991" alt="Captura de pantalla (1231)" src="https://github.com/user-attachments/assets/ac4bf7ce-c003-4f0e-ba6f-77a30b755ea5" />
</p>

<p align="center">
<img width="65%" height="1001" alt="17" src="https://github.com/user-attachments/assets/942bf8e6-8bc9-4584-8fc4-fb98450a336e" />
</p>

<p align="center">
<img width="65%" height="1014" alt="Captura de pantalla (1232)" src="https://github.com/user-attachments/assets/bf61c7c8-d674-4e5e-be84-a8d283ef2421" />
</p>

















