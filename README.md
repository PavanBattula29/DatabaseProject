# DatabaseProject
Objective:

The goal of this program is to develop a tool that takes a dataset (relation) and a set of functional dependencies as input. It then normalizes the relations based on the provided functional dependencies, generates SQL queries to create the normalized database tables, and optionally determines the highest normal form of the input table.


Program inputs:

To effectively use the program, provide your input data in 'exampleInputTable.csv', specify functional dependencies in 'dependencies.txt' (e.g., 'StudentID -> FirstName, LastName'), list multi-valued dependencies in 'mvd_dependencies.txt' (e.g., 'Course ->> Professor'), define your primary key(s) as a comma-separated list (e.g., 'StudentID, Course'), select your desired normalization form (e.g., 4 for 4NF), decide if the program should determine the highest normal form (1: Yes, 2: No), and for 5NF, provide candidate keys in the format '(A, B), (C, D)'. These inputs guide the program in normalizing your data effectively.

Working of the program:

The program systematically normalizes the input relation, progressing through each normalization form until it attains the specified highest normal form. At each stage, it rigorously evaluates whether the relation adheres to the required normalization form and generates normalized tables, complete with data, if needed. Once the desired highest normal form is achieved, the program concludes by producing SQL queries for creating the normalized tables. Users have the option to choose whether or not to display the highest normal form of the input table. Furthermore, the SQL queries for creating the normalized tables are neatly stored in the 'output.txt' file for convenient reference.

Functionality of each file:
The program is organized into four essential components:

1.main.py: This serves as the main execution file, responsible for managing input redirection and controlling the overall flow of the program.
2.data_parser.py: Handling the parsing of inputs from various sources, including CSV files, text files, and user input, this module ensures the efficient utilization of data throughout the program.
3.normalizedformtables.py: This module contains the core logic for normalizing the input relation, guiding it through the normalization process from 1NF to 5NF.
4.outputallformtables.py: A critical component for generating the necessary SQL queries, it takes the normalized tables as input and produces the queries needed to create these normalized tables. This well-structured architecture ensures a clean and organized approach to database normalization.

Team Members:

Ashok Kumar Pola (apm8p@mst.edu)
Vivek Reddy Mekala (vmm6d@mst.edu)
Pavan Kumar Reddy Battula (pbpc8@mst.edu)
Madhumitha Chalamala (mcw2b@mst.edu)
Akhila Arthi (aahvk@mst.edu)
