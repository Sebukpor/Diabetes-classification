# Diabetes-classification


```markdown
# Diabetes Detection Web Application

This web application allows users to predict the likelihood of diabetes based on several input parameters using a pre-trained TensorFlow.js model. The prediction is made by loading a TensorFlow model in the browser and processing user inputs from a simple HTML form.

## Features
- **Gender Selection**: Choose between Male and Female.
- **Age Input**: Enter your age.
- **Hypertension Input**: Indicate whether you have hypertension (1 for yes, 0 for no).
- **Heart Disease Input**: Indicate whether you have heart disease (1 for yes, 0 for no).
- **Smoking History**: Select your smoking history from the options provided.
- **BMI Input**: Enter your Body Mass Index (BMI).
- **HbA1c Level Input**: Enter your HbA1c level.
- **Blood Glucose Level Input**: Enter your blood glucose level.
- **Predict Button**: After entering all required information, click the "Predict Diabetes" button to get a prediction.

## Project Structure
The project contains the following files and directories:
- **index.html**: The main HTML file that contains the form and loads the TensorFlow.js model.
- **model/**: A directory containing the TensorFlow.js model files (`model.json` and associated weight files).

## Setup Instructions
### Prerequisites
- **Web Server**: To serve the HTML file correctly, it’s recommended to use a local web server. You can use any basic web server like Python's built-in HTTP server.

### Running the Application Locally
1. **Download or Clone the Repository**: 
   ```
   git clone https://github.com/sebukpor/diabetes-classification.git
   cd diabetes-classification
   ```

2. **Ensure the Model Files are in Place**: 
   - Place the `model.json` file and associated weight files in the `model/` directory. The structure should look like this:
     ```
      
     └── model/
         ├── model.json
         └── group1-shard1of1 (and other shard files)
          ├── index.html
     ```

3. **Start a Local Web Server**:
   - If you’re using Python, run the following command in the project directory:
     ```sh
     python3 -m http.server
     ```
   - This will start a local server, usually accessible at `http://localhost:8000`.

4. **Access the Application**:
   - Open your web browser and navigate to `http://localhost:8000` (or the address provided by your web server).
   - The form should be visible, and you can enter your details and click "Predict Diabetes" to see the result.

### Troubleshooting
- **Form Not Displaying**: Ensure that all required files are in place and the paths are correct. Also, check your browser's Developer Tools for any errors.
- **Model Not Loading**: If the model fails to load, ensure that the model files are correctly placed in the `model/` directory and that there are no issues with the file paths.

## Dependencies
- **TensorFlow.js**: This library is loaded via CDN in the HTML file and is required for running the model in the browser.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements
- TensorFlow.js for enabling machine learning in the browser.
- Any other libraries or resources used in the project.
```

