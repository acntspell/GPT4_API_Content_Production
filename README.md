Here's a README file for the described Python script:

# Donor Solicitation Script

This Python script is designed to automate the creation of personalized donor solicitation messages for a non-profit organization. It utilizes a preprocessed donor list where responses have been formatted to a first-person narrative style. The script generates custom messages using OpenAI's GPT-4 model, tailoring each message to individual donor profiles based on their historical donation behavior and demographic information.

## Features

- **API Key Integration**: Securely fetches the API key from environment variables.
- **Data Preprocessing**: Converts raw donor data into a narrative format.
- **Random Sampling**: Selects a random sample of donors to target for solicitations.
- **Personalized Message Generation**: Creates tailored solicitation messages using conversational AI.
- **Output**: Saves the generated messages in a CSV file for easy integration with mail merge applications.

## Installation

Ensure you have Python installed, and then install the required packages:

pip install pandas openai python-dotenv

## Configuration

1. Place your OpenAI API key and other sensitive information in a `.env` file at the root of your project directory.
2. Ensure your `.env` file contains the following variables:
   - `api_key`: Your OpenAI API key.
   - `writer`: A description of the writer's voice.
   - `client_org`: Information about the client organization.

## Usage

1. Load your preprocessed donor list into the `donors.csv` file.
2. Run the script to generate personalized solicitations:

python script_name.py

5. Check the `solicitations.csv` and `sample.csv` files for the output.

## Output Files

- `solicitations.csv`: Contains the solicitation messages paired with donor IDs.
- `sample.csv`: Contains a sample of 20 donors selected for solicitation.

## Security Notes

Do not commit your `.env` file to version control. Ensure it is listed in your `.gitignore` to avoid exposing sensitive information.

## Contributing

Contributions to this script are welcome. Please ensure to update tests as appropriate and follow the code of conduct for this project.

This README provides a concise yet comprehensive overview of the script's functionality, setup instructions, usage, and security practices. Adjustments can be made based on specific requirements or additional features of the script.
