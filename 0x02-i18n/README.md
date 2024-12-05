# ALX 0x02. i18n - Internationalization (i18n) Project

## Project Overview

This project is part of the **ALX Software Engineering Program (Backend Specialization)**. The focus of this project is to implement **internationalization (i18n)** in a Flask web application. Through this project, you'll learn how to build a web application that supports multiple languages, regions, and time zones to provide a better user experience for a global audience.

In this project, you'll set up basic Flask routes, integrate the **Flask-Babel** extension, handle language and time zone selections, and provide a personalized user experience based on their locale and time zone preferences.

## Tasks Breakdown

### Task 0: Basic Flask App

- **Objective**: Set up a basic Flask app with a single route (`/`) that displays "Welcome to Holberton" as the page title and "Hello world!" as the header.
- **Files**:
  - `0-app.py`: Flask application.
  - `templates/0-index.html`: Basic HTML template.

### Task 1: Basic Babel Setup

- **Objective**: Install the **Flask-Babel** extension and configure it to support multiple languages (`en` and `fr`), setting the default locale to `en` and the default timezone to `UTC`.
- **Files**:
  - `1-app.py`: Flask app with Babel configuration.
  - `templates/1-index.html`: Template with dynamic content.
  
### Task 2: Get Locale from Request

- **Objective**: Implement a `get_locale` function that uses `request.accept_languages` to determine the best language match based on the user's browser preferences.
- **Files**:
  - `2-app.py`: Updated Flask app with language detection.
  - `templates/2-index.html`: Template that adjusts based on the locale.

### Task 3: Parametrize Templates

- **Objective**: Parametrize the templates using **gettext** for translation. Set up `.po` files for English and French translations and compile them.
- **Files**:
  - `3-app.py`: Flask app with parameterized templates.
  - `babel.cfg`: Babel configuration file.
  - `templates/3-index.html`: Template with translation keys.
  - `translations/en/LC_MESSAGES/messages.po`: English translation file.
  - `translations/fr/LC_MESSAGES/messages.po`: French translation file.
  - `translations/en/LC_MESSAGES/messages.mo`: Compiled English translation file.
  - `translations/fr/LC_MESSAGES/messages.mo`: Compiled French translation file.

### Task 4: Force Locale with URL Parameter

- **Objective**: Allow users to force a specific locale by passing a `locale` parameter in the URL (e.g., `locale=fr`).
- **Files**:
  - `4-app.py`: Flask app with locale parameter handling.
  - `templates/4-index.html`: Template with forced locale selection.

### Task 5: Mock Logging In

- **Objective**: Create a mock login system by simulating user data. Users can log in using a `login_as` URL parameter, and their locale will be used for content display.
- **Files**:
  - `5-app.py`: Flask app with user mock data and login simulation.
  - `templates/5-index.html`: Template displaying user-specific content.

### Task 6: Use User Locale

- **Objective**: Modify the `get_locale` function to prioritize the user’s preferred locale. The priority order is:
  1. Locale from URL parameters.
  2. Locale from user settings.
  3. Locale from request headers.
  4. Default to English.
- **Files**:
  - `6-app.py`: Updated Flask app with user locale handling.
  - `templates/6-index.html`: Template that displays user locale settings.

### Task 7: Infer Appropriate Time Zone

- **Objective**: Implement time zone handling by inferring the user's time zone from the URL or user settings. If neither is available, default to UTC. Validate the time zone using **pytz**.
- **Files**:
  - `7-app.py`: Flask app with time zone inference.
  - `templates/7-index.html`: Template displaying the user's current time based on their time zone.

### Task 8: Display the Current Time (Advanced)

- **Objective**: Display the current time in the correct format based on the user’s inferred time zone. Ensure the time is displayed in both English and French, depending on the selected language.
- **Files**:
  - `app.py`: Flask app displaying the current time.
  - `templates/index.html`: Template with dynamic current time.
  - `translations/en/LC_MESSAGES/messages.po`: English translation file for time.
  - `translations/fr/LC_MESSAGES/messages.po`: French translation file for time.

## Installation

To get started with this project, follow the instructions below to set up the necessary environment:

### 1. Clone the Repository

```bash
git clone https://github.com/harystyleseze/alx-backend.git
cd alx-backend/0x02-i18n
```

### 2. Set Up a Virtual Environment

```bash
python3 -m venv venv
source venv/bin/activate  # For macOS/Linux
venv\Scripts\activate  # For Windows
```

### 3. Install Dependencies

```bash
pip3 install -r requirements.txt
```

### 4. Run the Flask Application

```bash
python3 0-app.py
```

You can now open your browser and visit `http://127.0.0.1:5000/` to see the app in action.

## Testing

Test different translations and locales by using URL parameters:
- `http://127.0.0.1:5000/?locale=fr` for French.
- `http://127.0.0.1:5000/?locale=en` for English.
- `http://127.0.0.1:5000/?login_as=2` to log in as a user.

## Contributing

If you have suggestions or improvements for this project, feel free to fork the repository and create a pull request. For any issues, please open an issue on GitHub.

## License

This project is open source and available under the [MIT License](LICENSE).

## Author

**Harrison Eze**  
GitHub: [harystyleseze](https://github.com/harystyleseze)

