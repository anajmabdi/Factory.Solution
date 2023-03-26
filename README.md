# <div align="center"> **Dr. Sillystringz's Factory**</div>

#### <div align="center"> By Najma Abdi </div>  
<p>&nbsp;</p>

# <div align="center"> Technologies Used
- <div align="center">C#
- <div align="center">HTML
- <div align="center">ASP.NET Core MVC
- <div align="center">EF Core
- <div align="center">Markdown
- <div align="center">Razer
- <div align="center">MySQL

<p>&nbsp;</p>

# <div align="center"> Description </div>
<div align="center"> Dr. Sillystringz owns a factory and will use this application to keep track of their machine repairs. The factory manager will be able to add a list of engineers, a list of machines, and specify which engineers are licensed to repair which machines.

The factory manager will:
- Be able to select an engineer, see their details, and see a list of all machines that engineer is licensed to repair. They will also be able to select a machine, see its details, and see a list of all engineers licensed to repair it.
- Be able to add new engineers to their system when they are hired. They will also add new machines to their system when they are installed.
- Not be able to create an engineer or a machine if the form's fields are empty or contain invalid values.
- Be able to add new machines even if no engineers are employed. They will also be able to add new engineers even if no machines are installed.
- Be able to add or remove machines that a specific engineer is licensed to repair. They will also be able to modify this relationship from the other side, and add or remove engineers from a specific machine.
- They will not be able to add a machine to an engineer if there are no machines. Likewise, they will not be able to add an engineer to a machine if there are no engineers.


<p>&nbsp;</p>


# <div align="center">Installation Requirements 
You must make sure the following software packages are locally installed in order to use this application:
- A preferred code editor (my case: VS Code)
- .NET6
- MySQL and MySQL workbench


<p>&nbsp;</p>

## <div align="center"> Setup

- Clone the repository.
- Launch the terminal and go to the "Factory" production directory for this project.
- Create a new appsettings.json file in the "Factory" production directory.
- Launch a code editor, then go to appsettings.json.
- Insert the following code in appsettings.json, substituting the values in the brackets with your personal MySQL username and password.

        {
         "ConnectionStrings": {
            "DefaultConnection": "Server=localhost;Port=3306;database=[DATABASE_NAME];uid=[uid];pwd=[pwd];"
         }
        }
- Add this file in your .gitignore, along with obj and bin files.


<p>&nbsp;</p>

## Import the Database

- Locate the Navigator pane in MySQL Workbench by opening it on the left-hand side of the program window. Selecting this option will bring up the Data Import page, where you can import data.
- Choose the "Import from Self Contained File" option. Locate the files you downloaded from this repository's top directory ("Factory").
- From "Factory," choose the najma_abdi.sql file.
- Click the "New" box next to "Default Schema to be Imported To", type "najma_abdi.sql" as the database name, and then click "OK".
- Locate the "Start Import" button in the Data Import Pane's lower right corner.
- The "Schemas" tab can be found on the Navigator panel. The database should appear if you click the "refresh" icon, which is represented by two arrows in a circle in the top right corner of the pane.


<p>&nbsp;</p>

## To run the server:
- Navigate to this project's production directory and run 'dotnet restore' if you haven't already. This will establish project-specific tools and dependencies that are listed in the project file
- Run 'dotnet watch' to start the server.

<p>&nbsp;</p>
<p>&nbsp;</p>


# <div align="center"> Known bugs </div>
None
<p>&nbsp;</p>

#### License

MIT License

Copyright (c) [2022] [Najma Abdi]

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions: