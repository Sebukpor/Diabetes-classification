Here's a clearer and more organized version of your README file for the project:

---

# Diabetes Detection Web Application

This web application allows users to predict the likelihood of diabetes based on various health parameters using a pre-trained TensorFlow.js model. The prediction is made directly in the browser by processing user inputs through a simple HTML form.

## Features
- **Gender Selection**: Choose between Male or Female.
- **Age Input**: Enter your age.
- **Hypertension Status**: Indicate whether you have hypertension (1 for Yes, 0 for No).
- **Heart Disease Status**: Indicate whether you have heart disease (1 for Yes, 0 for No).
- **Smoking History**: Select your smoking history from the provided options.
- **BMI Input**: Enter your Body Mass Index (BMI).
- **HbA1c Level Input**: Enter your HbA1c level (average blood glucose level over the past 3 months).
- **Blood Glucose Level Input**: Enter your current blood glucose level.
- **Predict Button**: After entering all required information, click the "Predict Diabetes" button to receive a prediction.

## Project Structure
The project includes the following files and directories:
- **index.html**: The main HTML file containing the form and loading the TensorFlow.js model.
- **model/**: A directory containing the TensorFlow.js model files (`model.json` and weight shards).

## Setup Instructions

### Prerequisites
- **Local Web Server**: Use a web server to serve the HTML file correctly. You can use Python's built-in HTTP server or any other basic web server.

### Steps to Run the Application Locally
1. **Download or Clone the Repository**: 
   ```sh
   git clone https://github.com/sebukpor/diabetes-classification.git
   cd diabetes-classification
   ```

2. **Ensure Model Files Are in Place**: 
   - Place the `model.json` file and its corresponding weight shards inside the `model/` directory. The directory structure should look like this:
     ```
     └── diabetes-classification/
         ├── index.html
         └── model/
             ├── model.json
             └── group1-shard1of1 (and other shard files)
     ```

3. **Start a Local Web Server**:
   - If using Python, navigate to the project directory and run:
     ```sh
     python3 -m http.server
     ```
   - This will start a web server, usually accessible at `http://localhost:8000`.

4. **Access the Application**:
   - Open your web browser and navigate to `http://localhost:8000`.
   - You should see the form where you can enter your details and predict the likelihood of diabetes.

### Troubleshooting
- **Form Not Displaying**: Ensure that all files are correctly placed and the paths are properly referenced. Check your browser's Developer Tools for errors.
- **Model Not Loading**: If the model fails to load, ensure that the `model.json` file and weight shards are correctly placed in the `model/` directory.

## Dependencies
- **TensorFlow.js**: The library is loaded via CDN in the HTML file, allowing the model to run in the browser.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgements
- **TensorFlow.js**: For enabling machine learning in the browser.
- Any other libraries or resources used in this project.

---

For any questions or suggestions, feel free to contact the project maintainer at **dasmedhub@gmail.com**.
