# Vehicle Service Management System - 'Multiple' Privilege Escalation Leads to CRUD Operations
Vehicle Service Management System - 'Multiple' Privilege Escalation Leads to CRUD Operations

### Exploit Title: Vehicle Service Management System - 'Multiple' Privilege Escalation Leads to CRUD Operations
### Date: 28/12/2021
### Exploit Author: P.L.Sanu
### Exploit Author Website: https://www.plsanu.com
### Vendor Homepage: https://www.sourcecodester.com
### Software Link: https://www.sourcecodester.com/php/14972/vehicle-service-management-system-php-free-source-code.html
### Version: <= 1.0
### Tested on: Windows 10
### CVE : 
### Google Dork: N/A
### Reference: 
- https://www.plsanu.com/vehicle-service-management-system-multiple-privilege-escalation-leads-to-crud-operations/
- https://github.com/plsanu/Vehicle-Service-Management-System-Multiple-Privilege-Escalation-Leads-to-CRUD-Operations

### 1. Vehicle Service Management System - 'User List' (/admin/?page=user/list) (/admin/?page=user/manage_user)

### Steps to Reproduce:
1. Visit the admin panel http://localhost/vehicle_service/admin
2. Login the Admin account in Browser A (Chrome)
3. Login the Staff account in Browser B (Firefox)
4. In Admin account(Chrome) navigate to the User List section and click on Create New button.
5. Copy the link of Create New User http://localhost/vehicle_service/admin/?page=user/manage_user
6. In Staff account (Firefox) there is no User List section because Staff Account didn't have the rights to create a user. 
7. Paste the copied link in Browser B (Firefox)
8. Now we are able to access the Create User Page.
9. Enter the required details and click on Save button.
10. In Admin account(Chrome) navigate to the User List section http://localhost/vehicle_service/admin/?page=user/list
11. The new user have been created successfully.
12. Staff account can able to access the User List page and Create User page.
13. Staff account can able to Create, Read, Update & Delete the users.

### 2. Vehicle Service Management System - 'Category List' (/admin/?page=maintenance/category) (/admin/?page=maintenance/manage_category)

### Steps to Reproduce:
1. Visit the admin panel http://localhost/vehicle_service/admin
2. Login the Admin account in Browser A (Chrome)
3. Login the Staff account in Browser B (Firefox)
4. In Admin account(Chrome) navigate to the Category List section and click on Create New button.
5. Copy the link of Create New Category http://localhost/vehicle_service/admin/?page=maintenance/manage_category
6. In Staff account (Firefox) there is no Category List section because Staff Account didn't have the rights to create a Category. 
7. Paste the copied link in Browser B (Firefox)
8. Now we are able to access the Create Category Page.
9. Enter the required details and click on Save button.
10. In Admin account(Chrome) navigate to the Category List section http://localhost/vehicle_service/admin/?page=maintenance/category
11. The new category have been created successfully.
12. Staff account can able to access the Category List page and Create Category page.
13. Staff account can able to Create, Read, Update & Delete the Category.

### 3. Vehicle Service Management System - 'Service List' (/admin/?page=maintenance/services) (/admin/?page=maintenance/manage_service)

### Steps to Reproduce:
1. Visit the admin panel http://localhost/vehicle_service/admin
2. Login the Admin account in Browser A (Chrome)
3. Login the Staff account in Browser B (Firefox)
4. In Admin account(Chrome) navigate to the Service List section and click on Create New button.
5. Copy the link of Create New Service http://localhost/vehicle_service/admin/?page=maintenance/manage_service
6. In Staff account (Firefox) there is no Service List section because Staff Account didn't have the rights to create a Service. 
7. Paste the copied link in Browser B (Firefox)
8. Now we are able to access the Create Service Page.
9. Enter the required details and click on Save button.
10. In Admin account(Chrome) navigate to the Service List section http://localhost/vehicle_service/admin/?page=maintenance/services
11. The new Serive have been created successfully.
12. Staff account can able to access the Service List page and Create Service page.
13. Staff account can able to Create, Read, Update & Delete the Service.

### 4. Vehicle Service Management System - 'Settings' (/admin/?page=system_info)

### Steps to Reproduce:
1. Visit the admin panel http://localhost/vehicle_service/admin
2. Login the Admin account in Browser A (Chrome)
3. Login the Staff account in Browser B (Firefox)
4. In Admin account(Chrome) navigate to the Settings section.
5. Copy the link of Settings Section http://localhost/vehicle_service/admin/?page=system_info
6. In Staff account (Firefox) there is no Settings section because Staff Account didn't have the rights to access the Settings. 
7. Paste the copied link in Browser B (Firefox)
8. Now we are able to access the Settings page.
9. Enter the required details and click on Save button.
10. In Admin account(Chrome) navigate to the Settings section http://localhost/vehicle_service/admin/?page=system_info
11. The details have been updated successfully.
12. Staff account can able to access the Settings page.
13. Staff account can able to Update the Settings.
