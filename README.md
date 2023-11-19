# **Documentation for Express API with MySQL**

## **Background of the Project**

This project serves as a hands-on exercise following the Express.js RESTful API tutorial provided by [Santri Koding](https://santrikoding.com/tutorial-set/tutorial-expressjs-restful-api). Utilizing Express.js as the backend framework and MySQL as the database, the project focuses on data management through RESTful API operations, covering everything from database configuration to CRUD operations.

## **Installation and Initial Configuration**

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/username/projectname.git
   cd projectname
   ```

2. **Install Dependencies:**
   ```bash
   npm install
   ```

## **Run Apache and MySQL in XAMPP**

1. **Install XAMPP:**
   - Download and install XAMPP from [https://www.apachefriends.org/index.html](https://www.apachefriends.org/index.html).

2. **Start XAMPP:**
   - Launch Apache and MySQL from the XAMPP control panel.

## **Configure MySQL Database**

1. **Open Configuration File:**
   - Open the `config/db.config.js` file.
   - Adjust the MySQL database configuration with the appropriate connection information.

## **Run the Project in the Text Editor**

1. **Run the Application:**
   - Open your text editor, open the `index.js` file.
   - Run the application by pressing the run button or using the command `node index.js`.

## **Using Postman for API Interaction**

1. **Display All Data:**
   - Open the Postman application.
   - URL: `http://localhost:3000/api/posts`.
   - Method: `GET`.
   - Click Send.

2. **Insert Data into the Database:**
   - URL: `http://localhost:3000/1/posts/store`.
   - Method: `POST`.
   - Choose the Body tab, select `x-www-form-urlencoded`.
   - Add Key and Value:
     - Key: `title`, Value: as desired.
     - Key: `content`, Value: as desired.
   - Click Send.
   - Response:
     ```json
     {
       "success": true,
       "message": "Insert Data Successfully"
     }
     ```

3. **Display Detail Data:**
   - URL: `http://localhost:3000/api/posts/1`.
   - Method: `GET`.
   - Click Send.

4. **Update Data in the Database:**
   - URL: `http://localhost:3000/api/posts/update/1`.
   - Method: `PATCH`.
   - Choose the Body tab, select `x-www-form-urlencoded`.
   - Add Key and Value for the update:
     - Key: `title`, Value: as desired.
     - Key: `content`, Value: as desired.
   - Click Send.
   - Response:
     ```json
     {
       "success": true,
       "message": "Update Data Successfully"
     }
     ```

5. **Delete Data from the Database:**
   - URL: `http://localhost:3000/api/posts/delete/1`.
   - Method: `DELETE`.
   - Click Send.
   - Response:
     ```json
     {
       "success": true,
       "message": "Delete Data Successfully"
     }
     ```

## **Note on Installing XAMPP**

- Ensure XAMPP is installed and running before starting the application.
