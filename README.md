# Film Affinity - Film Critique Generator

## Overview:
The Film Critique Generator is an application designed to generate personalised film critiques based on a user's film ratings from Letterboxd. It utilises web scraping to retrieve film ratings, OpenAI's GPT-3.5 model for critique generation, and offers a graphical user interface (GUI) for user interaction.

## About:
- **Functionality**: The script fetches film ratings from Letterboxd, generates personalised film critiques using GPT-3.5, and presents the generated critique to the user. It also generates HTML content for the critique.
- **Input**: Requires a Letterboxd username, and a ChatGPT API key
- **Output**: Generates a personalised film critique saved in a text file and an HTML file. It also presents the generated critique to the user through a GUI.

## How To:
1. Obtain an API key from OpenAI for accessing GPT-3.5.
2. Run the application "Film_Affinity.exe"
3. Input a Letterboxd username and ChatGPT API key through the GUI.
4. Click the "Generate Critique" button to initiate the process.
5. The script will scrape film ratings, generate a critique, save it as a text file, convert it to HTML, and open the HTML file for viewing.

Note: The GUI may look like it has "crashed", but it has not. Keep an eye on the command prompt for any errors and check the dist folder to ensure the files are being generated. 

## In-Depth:
- **Function Breakdown**:
  - `fetch_page`: Fetches a page of film ratings from a Letterboxd user's account.
  - `scrape_letterboxd`: Scrapes all rated films from a Letterboxd user's account and saves them as a text file.
  - `read_txt_ratings`: Reads the user's film ratings from the generated text file.
  - `generate_film_critique`: Generates a personalised film critique for the user based on their film ratings using GPT-3.5.
  - `generate_html_critique`: Generates HTML content for the film critique using ChatGPT.
  - `setup_gui`: Sets up the GUI components for user interaction.
  - `read_critique`: Reads the film critique from a text file.
  - `save_html_file`: Saves the generated HTML content as an HTML file.
  - `open_html_file`: Opens the HTML file in the default web browser.
  - **Error Handling**: The script includes error handling for file operations, network requests, and user inputs.
  - **API Integration**: Utilises OpenAI's GPT-3.5 model for generating film critiques based on user input prompts.
  - **Modular Design**: Functions are modularized for reusability and maintainability.
  - **User Interaction**: Provides a user-friendly GUI for inputting necessary information and viewing generated critiques.

## Disclaimer:
This script is provided for educational and demonstration purposes only. The use of this script to access and scrape data from third-party services such as Letterboxd may be subject to their terms of service. Use caution and ensure compliance with all applicable laws and regulations when utilising this script.
