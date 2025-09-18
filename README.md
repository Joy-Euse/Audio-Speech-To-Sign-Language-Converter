# Audio Speech To Sign Language Converter

A Django web application that converts spoken audio or text input into sign language representations, helping bridge communication between hearing and non-hearing individuals.

## Features

- **Speech Recognition:** Convert spoken audio to text.
- **Text-to-Sign Language:** Translate text input into sign language using images, animations, or videos.
- **User Authentication:** Sign up and log in to access the service.
- **Natural Language Processing:** Uses NLTK for text processing.

## Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/Joy-Euse/Audio-Speech-To-Sign-Language-Converter.git
   cd Audio-Speech-To-Sign-Language-Converter-master
   ```

2. **Create and activate a virtual environment:**
   ```sh
   python -m venv venv
   venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

4. **Download required NLTK data:**
   ```sh
   python
   >>> import nltk
   >>> nltk.download('punkt')
   >>> nltk.download('averaged_perceptron_tagger')
   >>> nltk.download('wordnet')
   >>> nltk.download('omw-1.4')
   >>> exit()
   ```

5. **Apply migrations:**
   ```sh
   python manage.py migrate
   ```

6. **Run the development server:**
   ```sh
   python manage.py runserver
   ```

7. **Access the app:**
   Open your browser and go to [http://127.0.0.1:8000/](http://127.0.0.1:8000/)

## Usage

- **Sign Up:** Create an account to use the converter.
- **Convert Speech/Text:** Enter text or use the microphone to input speech. The app will display the corresponding sign language translation.

## Troubleshooting

- If you see `LookupError: Resource punkt not found`, make sure you have downloaded the required NLTK data as shown above.
- If the server does not start, check that your virtual environment is activated and all dependencies are installed.

## License

This project is for educational purposes. See `LICENSE` for more details.

## Credits

Developed by [Your Name/Team].  
Uses Django, NLTK, and other open-source libraries.