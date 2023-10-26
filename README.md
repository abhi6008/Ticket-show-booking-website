# Ticket-show-booking-website

# Frontend

To run the frontend, follow these steps:

1. navigate to your project folder and run the development server using the following command:
   ```
   npm run dev
   ```

2. Once the development server is up and running, you will see a URL in the terminal. Copy this URL and paste it into any browser to access the frontend.

3. If frontend folder has index.html then run locally on any port.

# Backend

To run the backend, you'll need to perform the following steps:

1. Open your project folder containing the backend code.

2. To start the backend server, run the `app.py` file.

3. Open an Ubuntu terminal and navigate to the project folder. Activate the virtual environment using the following command:
   ```
   source env/bin/activate
   ```

4. After activating the environment, run the Redis server using the following command:
   ```
   redis-server
   ```

5. Open another Ubuntu terminal, navigate to the project folder, and activate the virtual environment as before.

6. To activate the Celery beat process, run the following command:
   ```
   celery -A main.celery beat --max-interval 1 -l info
   ```

7. Open a third Ubuntu terminal, navigate to the project folder, and activate the virtual environment.

8. To start the Celery worker process, run the following command:
   ```
   celery -A main.celery worker -l info
   ```

9. Finally, to run Mailhog, open an Ubuntu terminal and execute the following command:
   ```
   Mailhog
   ```

10. Once Mailhog is running, you can access it in your browser using the URL and port 8025.

Please make sure you have all the necessary dependencies and configurations set up before running these commands.
