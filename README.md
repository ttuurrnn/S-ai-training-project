# Diet Recommendation App

This project is a Flask-based web application that provides personalized diet recommendations based on user inputs such as age, weight, height, gender, activity level, and dietary goals. The app utilizes the FatSecret API to fetch food and recipe data, ensuring that the diet plans are both accurate and diverse.

## Features

- **User Input:** Users can enter their personal information (age, weight, height, etc.) and dietary goals.
- **Calorie Calculation:** The app calculates the user's daily caloric needs based on the Harris-Benedict equation, adjusted for their activity level and goals.
- **Personalized Diet Plan:** The app provides a diet plan with specific meals and recipes, including a breakdown of calories, proteins, carbs, and fats.
- **API Integration:** The app integrates with the FatSecret API to search for foods and recipes, using real data to generate meal plans.

## Installation

### Prerequisites

Before you begin, ensure you have Python installed on your machine. You'll also need an API key from FatSecret.

### Steps

1. **Clone the repository:**

    ```bash
    git clone https://github.com/ttuurrnn/my-diet-app.git
    cd my-diet-app
    ```

2. **Create and activate a virtual environment:**

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. **Install the dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4. **Set up your environment variables:**

    Create a `.env` file in the project root and add your FatSecret API credentials:

    ```plaintext
    CLIENT_ID=your_fatsecret_client_id
    CLIENT_SECRET=your_fatsecret_client_secret
    ```

5. **Run the application:**

    ```bash
    python app.py
    ```

6. **Access the application:**

    Open your web browser and navigate to `http://localhost:5000`.

## Usage

1. **Input your details:** On the main page, enter your age, weight, height, gender, activity level, and dietary goal (e.g., weight loss, muscle gain).
2. **Get your diet plan:** Click "맞춤형 다이어트 식단 추천 받기" to generate a customized diet plan.
3. **Review your plan:** The app will display a diet plan with meals and recipes, along with a breakdown of calories and macronutrients.

## Project Structure

- **`app.py`:** The main Flask application file, containing all the routes and logic.
- **`templates/index.html`:** The main page where users input their information.
- **`templates/result.html`:** The results page displaying the recommended diet plan.
- **`requirements.txt`:** A list of all Python dependencies required to run the app.

## Technologies Used

- **Flask:** A lightweight web framework for Python used to build the application.
- **FatSecret API:** Used to retrieve food and recipe data for generating diet plans.
- **Tailwind CSS:** A utility-first CSS framework for styling the user interface.
- **Chart.js:** Used for visualizing BMI (Body Mass Index) on the front end.

## Future Enhancements

- **Enhanced Recipe Recommendations:** Improve the diversity of recommended recipes by integrating more advanced search criteria.
- **User Accounts:** Allow users to save their dietary plans and track their progress over time.
- **Multi-language Support:** Add support for multiple languages to cater to a broader audience.


## Acknowledgements

- Special thanks to the FatSecret API team for providing a comprehensive API that made this project possible.

