# Job Description Translator

A Flask web application that translates complex job descriptions into simpler, more understandable language for job applicants using OpenAI's GPT models.

## Features

- Paste any job description into the web interface
- Get a simplified, jargon-free translation that explains the role clearly
- Responsive design that works on desktop and mobile devices

## Setup

1. Clone this repository
2. Create a virtual environment:
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. Install dependencies:
   ```
   pip install -r requirements.txt
   ```
4. Set your OpenAI API key using the provided script:
   ```
   python set_api_key.py YOUR_API_KEY
   ```
   Or run the script without arguments to be prompted for the key:
   ```
   python set_api_key.py
   ```
5. Run the application:
   ```
   python app.py
   ```
   Or use the provided shell script:
   ```
   ./run.sh
   ```
6. Open your browser and navigate to `http://localhost:12000`

## Testing with Sample Data

A sample job description is included in the repository for testing purposes. To test the application with this sample:

1. Make sure the application is running in one terminal
2. In another terminal, run:
   ```
   python test_with_sample.py
   ```
   This will send the sample job description to the API and display the translated result.

## Technologies Used

- Flask: Web framework
- OpenAI API: For translating job descriptions
- Bootstrap: For responsive UI
- JavaScript: For handling form submissions and displaying results

## License

MIT