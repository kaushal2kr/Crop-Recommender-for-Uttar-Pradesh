Crop Recommender for Uttar Pradesh
A machine learning-based crop recommendation system for farmers in Uttar Pradesh, India. This tool uses environmental factors like temperature, humidity, rainfall, soil type, and season to suggest the best crops to grow in specific cities. It provides detailed recommendations, including nutrient requirements, water needs, expected yield, market price, and crop rotation suggestions, along with visualizations and downloadable reports.
Features

Crop Recommendations: Predicts the top 5 crops based on city, temperature, humidity, rainfall, soil type, and season using a Random Forest model.
Visualizations: Generates bar graphs, pie charts, scatter plots, feature importance heatmaps, and historical yield trends.
Interactive Map: Displays recommended crops on a map of Uttar Pradesh using Folium.
Reports: Exports recommendations as PDF, Excel, and CSV files.
Audio Output: Provides a speech summary of recommendations using gTTS.
User Interface: Built with Gradio for an easy-to-use web interface.

Installation

Clone the repository:git clone https://github.com/your-mental2devil/crop-recommender.git
cd crop-recommender


Install dependencies:pip install pandas numpy scikit-learn gradio matplotlib seaborn gTTS folium reportlab pyngrok requests openpyxl


(Optional) Set up ngrok for public access:
Sign up at ngrok.com and get your auth token.
Replace YOUR_NGROK_AUTH_TOKEN and YOUR_NGROK_API_KEY in the code with your credentials.



Usage

Run the script in a Python environment (preferably Google Colab for file downloads):python crop_recommender.py


Access the Gradio interface via the provided URL (local or ngrok).
Input the following:
City: Select a city in Uttar Pradesh (e.g., Lucknow).
Temperature: Enter a value (0-50°C) or leave blank for city default.
Humidity: Enter a value (0-100%) or leave blank.
Rainfall: Enter a value (≥0 mm) or leave blank.
Soil Type: Choose from clay, sandy, loamy, black, or red.
Season: Select kharif, rabi, or summer.


View the recommendations, visualizations, and download reports (PDF, Excel, CSV, audio, and map).

Requirements

Python 3.8+
Libraries: pandas, numpy, scikit-learn, gradio, matplotlib, seaborn, gTTS, folium, reportlab, pyngrok, requests, openpyxl
Google Colab (recommended for full functionality, especially file downloads)
Ngrok account (optional, for public access)

Notes

The system is optimized for Uttar Pradesh, with data for 30 cities and various crops, including cereals, fruits, vegetables, pulses, and herbs.
Visualizations and reports are saved in the /content/crop_recommender directory.
If Gradio's share=True fails, the script falls back to ngrok. Ensure you have a valid ngrok auth token.
Replace placeholder ngrok tokens in the code before running.

Contributing
Feel free to open issues or submit pull requests for improvements or bug fixes.
License
This project is licensed under the MIT License.
Acknowledgments

Built using open-source libraries like scikit-learn, Gradio, and Folium.
Inspired by the need to support farmers with data-driven crop choices.
