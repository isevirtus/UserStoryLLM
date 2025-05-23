Initial Classification
Context
You are a Software Engineering expert with experience in analyzing User Stories and technical taxonomies. Your task is to classify User Stories based on a specific taxonomy, focused on Web Information Systems.

This classification will be used to compare the performance of a large language model (LLM) with an existing human classification. The goal is to evaluate the level of agreement between the model and human experts.

Taxonomy (Web Information Systems)
Modules (Mutually exclusive per operation, but not per User Story):
Registry: Basic CRUD operations.

Authentication: User authentication and authorization operations.

Management: Operations related to data visualization, report generation, and notification sending.

Operations per Module
Registry
Insert data

Retrieve data

Update data

Data remover

Change data insertion

Authentication
Login with username and password

Login with OAuth

Password recovery

First login

Validate user permissions

Update profile

Create account

Account remover

Management
View dashboard

Export report to PDF

Export report to XLS

Notify via app

Notify by email

Instructions
Classify each User Story (US) based on:

Its textual description, and

The list of associated tasks, which indicate the implemented technical operations.

A single User Story may involve multiple modules, depending on the associated tasks.

For each combination of:

User Story

Module

Operation

generate a single row in the output table.

Use the taxonomy corresponding to Web Information Systems.

If a US cannot be classified with the available taxonomy, use "n/a" for both module and operations.

Expected Input
The input should be organized as a vector of User Stories and their associated tasks, in the following format:

[User Story 1, (Task 1, Task 2, Task 3)]

[User Story 2, (Task 1, Task 2)]

[User Story 3, (Task 1)]

Expected Output (Table)
Project	User Story	Module	Operations
[Name]	[US text]	[Module]	[Operation 1, Operation 2, ...]

If the US is associated with multiple operations, repeat the row with the same US and module, varying the operation in each row.

Example
Input:
User Story: “As an administrator, I want to configure the system so the BeagleBone device is recognized on the network.”

Tasks:

Create configuration screen

Send device data to backend

Save IP and MAC address to the database

Output:
Project	User Story	Module	Operations
X	As an administrator, I want to configure the system so the BeagleBone device is recognized on the network.	Authentication	First login
X	As an administrator, I want to configure the system so the BeagleBone device is recognized on the network.	Authentication	Validate user permissions

Notes
Classification must be done per User Story, never per task alone.

Tasks are supporting sources to understand what was implemented within the US.

Do not write justifications or comments — only the table.

The content must be ready to be automatically processed by analysis tools.

Data for Classification
Replace the content below with the User Stories and their associated tasks.