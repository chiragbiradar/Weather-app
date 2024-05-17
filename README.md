**Weather App - Leadzenai Assignment**

This Django web application retrieves real-time weather information for any city using the OpenWeatherMap API.

**Features:**

- User-friendly interface for entering city names
- Displays current weather conditions (temperature, humidity, description, etc.)
- Clean and responsive design (consider adding a screenshot if possible)

**Prerequisites:**

- Python 3.x ([https://www.python.org/downloads/](https://www.python.org/downloads/))
- pip package manager (usually comes with Python)
- Virtual environment tool (recommend `venv` or `virtualenv`)

**Setup:**

1. **Create a virtual environment:**

   ```bash
   python -m venv venv  # Using venv
   source venv/bin/activate  # Activate on Linux/macOS
   venv\Scripts\activate.bat  # Activate on Windows
   ```

2. **Clone this repository (if applicable):**

   ```bash
   git clone https://github.com/your-username/weather-app.git
   cd weather-app
   ```

3. **Install dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Obtain an OpenWeatherMap API key:**

   - Create a free account at [https://openweathermap.org/api](https://openweathermap.org/api).
   - Go to your profile and navigate to the API keys section.
   - Create a new API key and copy it for the next step.

5. **Configure API key:**

   - Create a file named `.env` in the project's root directory (**important: exclude this from version control**).
   - Add the following line, replacing `API_KRY` with your actual key:

     ```
     API_KEY=YOUR_API_KEY
     ```

6. **Run database migrations:**

   ```bash
   python manage.py migrate
   ```

7. **Start the development server:**

   ```bash
   python manage.py runserver
   ```

   Open http://127.0.0.1:8000/ in your web browser to access the app.

**Deployment:**

The provided deployment instructions ("hosted at weather-app-leadzenai-assignment.vercel.app") are specific to Vercel. However, here's a general outline that can be adapted to various hosting providers:

1. Consult your hosting provider's documentation on deploying Django applications.
2. Typically, you'll need to configure environment variables (including your API key) for the production environment.
3. Push your code to a version control system (e.g., Git).
4. Follow your provider's instructions on building and deploying your app.
