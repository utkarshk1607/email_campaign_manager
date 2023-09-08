# Django Email Campaign Manager

**Description:**

The Django Email Campaign Manager is a web application that allows you to manage email subscribers, create email campaigns, and send out email campaigns to your subscribers. This app uses an SQLite3 database for data storage.

**Features:**

- Add and remove subscribers from your email list.
- Create and manage email campaigns.
- Start and send email campaigns to your subscribers.
- Track the status and results of your email campaigns.

**Installation:**

1. Clone the repository to your local machine: <br>
`git clone https://github.com/your-username/email-campaign-manager.git` <br>

2. Change into the project directory: <br>
`cd email-campaign-manager` <br>

3. Create a virtual environment and activate it: <br>
`python -m venv venv` <br>
`source venv/bin/activate` <br>

4. Install the required packages: <br>
`pip install -r requirements.txt` <br>

5. Apply database migrations: <br>
`python3 manage.py makemigrations` <br>
`python3 manage.py migrate` <br>

6. Create a superuser to access the admin panel: <br>
`python3 manage.py createsuperuser` <br>

7. Start the development server: <br>
`python manage.py runserver` <br>


8. Access the app at `http://l27.0.0.1:8000/` and the admin panel at `http://127.0.0.1:8000/admin/`.

**Usage:**

1. **Admin Panel:**

- Access the admin panel using the superuser credentials created during installation.
- Add subscribers and manage your email list.
- Create and manage email campaigns.

2. **Endpoints:**

The app provides endpoints for managing subscribers and campaigns programmatically.

- `/add_subscribe/`: List and create subscribers.
- `/unsubscribe`: Retrieve, update, or delete a specific subscriber.
- `/add_campaign/`: Create email campaigns.
- `/send_email`: Send email of a specific campaign to all the "active users"

**Configuration:**

- The default database used is SQLite3. You can change the database settings in `settings.py` if needed.
