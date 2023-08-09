# To-Do List Django Project with Social Authentication

Welcome to the To-Do List Django project with social authentication! This project showcases a simple to-do list application with the added functionality of logging in using popular social media platforms such as Facebook and Google. This README file will guide you through the process of setting up and running the project on your local machine using Django.

## Prerequisites

Before you begin, ensure you have the following:

- **Python:** Make sure you have Python installed. You can download it from the official [Python website](https://www.python.org/).
- **pip:** This package manager usually comes with Python. You'll need it to install project dependencies.
- **Virtual Environment (optional but recommended):** It's a good practice to set up a virtual environment for your project to keep dependencies isolated. You can create one using the `venv` module that comes with Python.

## Getting Started

Follow these steps to set up and run the project on your local machine:

1. **Clone the Repository:**
   ```
   git clone https://github.com/salman-221b/To-do-list-with-social-authentication.git
   cd To-do-list-with-social-authentication
   ```

2. **Install Dependencies:**
   Install the required Python packages by running the following command inside the project directory:
   ```
   pip install -r requirements.txt
   ```

3. **Database Configuration:**
   Configure your database settings in `settings.py`. By default, the project is set up to use SQLite. If you prefer a different database, you can modify the `DATABASES` section in the same file.

4. **Run Migrations:**
   Apply the database migrations to set up the database schema by running:
   ```
   python manage.py migrate
   ```

5. **Create Superuser (Admin):**
   Create an admin superuser using the following command and follow the prompts:
   ```
   python manage.py createsuperuser
   ```

6. **Run the Development Server:**
   Start the Django development server:
   ```
   python manage.py runserver
   ```

7. **Access the Admin Panel:**
   Open your web browser and navigate to `http://127.0.0.1:8000/admin` to access the Django admin panel. Log in using the superuser credentials created earlier.

8. **Add Social App Credentials:**
   In the admin panel, navigate to **Social Applications** under the **Social Accounts** section. To enable social authentication through Facebook and Google, you'll need to create apps on their respective developer platforms and obtain client ID and client secret.

   - **Facebook:**
     1. Go to the [Facebook for Developers](https://developers.facebook.com/) website.
     2. Create a new app and configure the app settings.
     3. Obtain the **App ID** and **App Secret** from the Facebook developer dashboard.
     4. In the Django admin panel, add a new Social Application:
        - Provider: Facebook
        - Name: Your choice (e.g., Facebook)
        - Client ID: Your Facebook App ID
        - Secret Key: Your Facebook App Secret
        - Sites: Select the appropriate site

   - **Google:**
     1. Go to the [Google Cloud Console](https://console.cloud.google.com/) website.
     2. Create a new project and configure the OAuth 2.0 credentials.
     3. Obtain the **Client ID** and **Client Secret** from the Google Cloud Console.
     4. In the Django admin panel, add a new Social Application:
        - Provider: Google
        - Name: Your choice (e.g., Google)
        - Client ID: Your Google Client ID
        - Secret Key: Your Google Client Secret
        - Sites: Select the appropriate site

9. **Access the Application:**
   After adding the social app credentials, navigate to `http://127.0.0.1:8000` in your web browser to access the application. You can sign up and log in using conventional email/password, as well as through your Facebook or Google account.

## Contributing

Contributions are welcome! If you'd like to improve the project, fix any bugs, or add new features, feel free to submit a pull request.



## Contact

If you have any questions or need further assistance, you can contact the project owner at salmanmehboob610@gmail.com

Enjoy using the To-Do List Django project with social authentication!
