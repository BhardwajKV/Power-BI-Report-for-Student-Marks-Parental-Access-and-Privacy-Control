Power BI Report for Student Marks: Parental Access and Privacy Control

Dashboard Link - https://bit.ly/4eYVNqL


Project Overview:
The goal of this project is to create a Power BI report that allows parents to view their child's marks securely. Each parent should be able to see only their student's data. The final dashboard will be published publicly, but access to specific data will be restricted based on the user's credentials.

Objectives:
1.	Create a live Power BI report that displays student marks.
2.	Ensure parents can only view data specific to their own children.
3.	Publish the dashboard publicly while maintaining privacy and security controls.


Tools and Technologies:

•	Microsoft Power BI: 

To create the dashboard.

•	MYSQL Database: 

To store the student marks data and Clean Data.

•	Power BI Service: To publish and share the report.

Project Scope and Requirements:
1.	Data Source Preparation:
o	Collect student data, including columns like Student ID, Student Name, Parent ID, Marks, Subject, and Class.
o	Store the data in a format compatible with Power BI, such as Excel or SQL Server.
o	Ensure data accuracy and completeness for analysis.

2.	Dashboard Development:
o	Import the student data into Power BI Desktop.
o	Create visuals that represent student performance, such as bar charts, line charts, and tables.
o	Design filters to allow data exploration (e.g., by subject, class, and term).

3.	Privacy and Security:
o	Implement appropriate security measures to ensure that parents can only view data related to their own children. You may need to apply specific configurations or settings to achieve this.

4.	Publishing the Report:
o	Publish the report to the Power BI Service.
o	Configure security settings as needed to ensure privacy.
o	Generate a public link to share the dashboard, while ensuring that security settings remain in effect.

Detailed Steps:

1.	Data Collection and Preparation:
Gather student marks data, including information about each student's parent. An example dataset structure is as follows:
Publish the report to the Power BI Service.
![Screenshot 2024-10-26 190319](https://github.com/user-attachments/assets/b5347909-ff10-4e04-abda-2527b1f34db1)

2.  The missing values were identified and those who were attended the exam and still absent were made present using the folllowing code: 

![Screenshot 2024-10-26 201502](https://github.com/user-attachments/assets/3e59fecb-b0fb-434c-bde8-0f94d371537b)

3. Then the name were concated:
![Screenshot 2024-10-26 201529](https://github.com/user-attachments/assets/eba601bc-0a91-4675-bdda-b66c4e134b23)

4. The values which were missing in the maths column were retrived by the following query:
![Screenshot 2024-10-26 202009](https://github.com/user-attachments/assets/81e2717f-8081-405f-b00b-b6dae467f9fa)

5. The new column was added to show the sum value of maths,physics, and chemistry as new_total

![Screenshot 2024-10-26 202357](https://github.com/user-attachments/assets/cc281339-d3b1-4bf2-9425-5081bedd5291)

6. Then used the CTE to find the difference between the new_total and userscore:
![Screenshot 2024-10-26 202556](https://github.com/user-attachments/assets/68ae333f-cc45-417f-8f32-7d6abd1a6ca6)

7. Then joined the parents table with the students table:
![Screenshot 2024-10-26 202740](https://github.com/user-attachments/assets/0d17bb52-1b9d-462f-93c9-df96c8704df3)


8. Next finally the new table was created and included all the above changes into one table as final_new_data:
![Screenshot 2024-10-26 203015](https://github.com/user-attachments/assets/0a093f3e-2be7-45b3-859f-2b8b5ba4c55b)


9. Then the csv was imported into the power BI.

10. Then the log in page was created:
![Screenshot 2024-10-26 203209](https://github.com/user-attachments/assets/482e6e7b-f4d2-4b68-965f-61f64a060fbb)

11. The result report was created using the:
o	Card

o	Slicer

o	Stacked column chart

o	Table

o	Then button also added to log in and return action feature.

![Screenshot 2024-10-26 203526](https://github.com/user-attachments/assets/2da97f2e-b198-4c70-8b8f-f688c398c934)

12. Finally the power BI dashboard was published and given the public access:



Publishing the Dashboard


![Screenshot 2024-10-26 204859](https://github.com/user-attachments/assets/3726742c-6afc-4985-84ce-2f432fc478df)


Giving Access 
![Screenshot 2024-10-26 205057](https://github.com/user-attachments/assets/c3b3db31-0da8-4a5a-8acb-21f36c3a281a)




Challenges and Solutions:
1.	Data Privacy:
o	Challenge: Ensuring that each parent only views their own child's data.

o	Solution: Implement the appropriate security settings to restrict data based on the user's credentials.


2.	Public Sharing of Dashboard:
o	Challenge: Sharing the report publicly while maintaining data security.

o	Solution: The public link will be shared, but data access will be controlled through the necessary security settings applied during the report configuration.

Conclusion:

This project successfully creates a Power BI report where parents can view their child's marks while ensuring data privacy. This approach ensures a user-friendly experience, providing parents with valuable insights into their child's academic performance without compromising confidentiality.

CSV file of students and parents - 

https://docs.google.com/spreadsheets/d/1NBS1dGZwNjviXkMnNIpaiGHCPjiov8LE6jCA3zKb-e0/edit?gid=0#gid=0

Power BI Dashboard Link: 

https://bit.ly/4eYVNqL


