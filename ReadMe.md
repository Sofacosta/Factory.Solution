<div align="center">

# Factory 🔩

</div>

<h3 align="center">An application to keep track of their machine repairs, Initiated: 06-03-2021 Modified:06-05-21</h3>
<h4 align="center"> By Sofia Acosta</h4>

## Description
MVC web application to manage their engineers, and the machines they are licensed to fix. The factory manager should be able to add a list of engineers, a list of machines, and specify which engineers are licensed to repair which machines. 

## Setup/Installation Requirements

##### Software Requirements

1. Internet browser
2. A code editor such as VSCode to view and edit the code
3. .NET or follow along with the Installing .NET instructions to install .NET

##### Open Locally

- Click on the link to my repository: [My Repository]()
- Click on the green "Code" button and copy the repository URL
- Open your terminal and use the command `git clone REPO URL HERE` into the directory you would like to clone the repository
- Open in text editor to view code and make changes

##### Installing .NET

In order to run the application, please install .NET for your computer to recognize the `dotnet` command.

1. Download [.NET Core SDK (Software Development Kit)](https://dotnet.microsoft.com/download/dotnet). Clicking this link will prompt a file download for your particular OS from Microsoft.
2. Open the file. Follow the installation steps.
3. Confirm the installation is successful by opening your terminal and running the command `dotnet --version`. The response should be something similar to this:`5.0.100`. This means it was successfully installed.

##### Installing MySQL

MySQL is a type of database software used to create, edit, query, and manage SQL data.

- For Mac Users please [Click Here](https://dev.mysql.com/downloads/file/?id=484914) to download MySQL Installer
- For Windows Users please [Click Here](https://dev.mysql.com/downloads/file/?id=484919)

- Verify MySQL installation by opening the terminal and entering the command `mysql -uroot -p[THEPASSWORDYOUSELECTED]`
- If you gain access you will see see the MYSQL command line!

##### Installing MySQL Workbench

- Please [Click Here](https://dev.mysql.com/downloads/workbench/) to install the correct version for your machine
- Open MySQL Workbench and select `Local instance 3306 server`. You will need to enter the password you selected

##### Compiling

- Navigate to the TODO folder in the command line
- Use the command `dotnet build` to compile

##### Installing Packages
- Navigate to the TODO folder in the command line
- Use the command `dotnet restore`

<details>

  <summary>Expand for Database Installation Essentials!</summary>

### Database Connection

Create a connection string to connect the database to the web application

1. Create a file in the root directory called `appsettings.json`
2. Add the code below:

```
{
  "ConnectionStrings": {
      "DefaultConnection": "Server=localhost;Port=3306;database=name_lastname;uid=root;pwd=[your password];"
  }
}
```

- CHANGE DBNAME
- Put in your MySQL password in `pwd=YourPassword`. Change the server, port, and uid if necessary.

### Import Database Using Entity Framework Core

1. Navigate to TODO directory in terminal
2. Use the command `dotnet ef database update` to generate the database through Entity Framework Core

### Update Database Using Entity Framework Core

1. Write any new code you wish to add to the database. Use the command `dotnet build` to check for any compiling errors. If no errors, proceed to step 2.
2. To update the database with any changes made to the code, use the command `dotnet ef migrations add [MigrationsName]`
3. Use the command `dotnet ef database update` to update the database

### Update Database Using MySQL Workbench

1. Open MySQL Workbench
2. Click on Server > Data Import in the top navigation bar
3. Select `Import from Self-Contained File`
4. Select the `Default Target Schema` or create new schema
5. Select all Schema Objects you would like to import
6. Select `Dump Structure and Data`
7. Click `Start Import`

</details>

##### View In Browser

- To view in browser, navigate to TODO folder in the command line
- Use the command `dotnet run` to execute the compiled code and start a localhost
- In browser navigate to http://localhost:5000

## Known Bugs

## Notes and Resources

- [HTML button callinng an MVC Controller and Action method](https://stackoverflow.com/questions/2503923/html-button-calling-an-mvc-controller-and-action-method)

- [Form buttons](https://getbootstrap.com/docs/4.0/components/buttons/)


## Support and Contact Details

If any errors or bugs occur with installation, delete both bin and obj folders and follow the Compiling and Installing Packages instructions again. Get help or report a bug you have found in the .NET platform at [.NET Support](https://dotnet.microsoft.com/platform/support). Or please email me, <agatakolohe@gmail.com>.

## Technologies Used

- .NET Core 5.0.1
- ASP.NET Core MVC
- ASP.NET Core Razor Pages
- Bootstrap
- C#
- CSS
- Entity Framework Core
- GitHub
- HTML
- MySQL
- MySQL Workbench
- VS Code

### License

This software is licensed under the [MIT License](https://choosealicense.com/licenses/mit/).