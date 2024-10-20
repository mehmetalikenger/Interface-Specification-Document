
# Interface Specifications

## Requirements
Users should be able to:
- Create a new user by filling out a form.
- See the user table.
- Hide the disabled users.

## UI Components

### 1. **User Table**
There should be a user table that the users can see. This table must contain the following columns:
- **ID**: The unique identifier for the user.
- **User Name**: The username of the user.
- **Email**: The email of the user.
- **Enabled**: A boolean column (`true/false`) indicating whether the user is enabled.

### 2. **New User Button**
There should be a button labeled "**+ New User**" to create a new user. This button should be on the table.

### 3. **New User Form**
To create a new user, the user must fill out a form. The form should contain the following input fields:
- **Username**
- **Display Name**
- **Phone**
- **Email**
- **User Roles**: A dropdown (`ComboBox`) to select a user role (`Guest`, `Admin`, `SuperAdmin`). The default text of the ComboBox must be **“Select user roles”**.
- **Enabled**: A checkbox to indicate whether the user is enabled.

### 4. **Hide Disabled Users Checkbox**
There should be a checkbox to hide disabled users. This checkbox should be next to the "New User" button.

### 5. **Save User Button**
This button will allow the user to save the data on the form.

---

## Behaviors

- To create a new user, the user must click on the "**+ New User**" button.
- The "New User Form" must be shown after the user presses the "**+ New User**" button.

### User Roles ComboBox
- When the user clicks on the ComboBox, it must list the following values:
  - Guest
  - Admin
  - SuperAdmin

### Save Button Activation
- The "Save User" button must be active after the user fills out the entire form.
- If the user clears any section of the form, the "Save User" button must be deactivated again.
- The color of the "Save User" button must be brighter than its actual color when it is deactivated.

### User Table Interaction
- The user must be able to change the order of the columns in the table using the buttons on each column header.

