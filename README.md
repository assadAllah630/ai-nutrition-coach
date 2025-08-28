# AI Nutrition Coach

An intelligent nutrition analysis application that uses IBM Watson AI to analyze food images and provide detailed nutritional information, calorie estimates, and health assessments.

## Features

- **Image-based Food Recognition**: Upload food images for instant analysis
- **Detailed Nutritional Breakdown**: Get comprehensive information about calories, proteins, carbohydrates, fats, vitamins, and minerals
- **Portion Size Estimation**: Accurate portion size detection and calorie calculation
- **Health Assessment**: Professional nutritional evaluation of your meals
- **User-friendly Interface**: Clean, modern web interface with real-time image preview

## Technology Stack

- **Backend**: Flask (Python)
- **AI/ML**: IBM Watson AI (Llama 4 Model)
- **Image Processing**: PIL (Python Imaging Library)
- **Frontend**: HTML5, CSS3, JavaScript
- **Styling**: Modern responsive design with glassmorphism effects

## Prerequisites

- Python 3.8+
- IBM Watson AI account and API credentials
- Modern web browser

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/assadAllah630/ai-nutrition-coach.git
   cd ai-nutrition-coach
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**
   ```bash
   cp .env.example .env
   ```
   
   Edit `.env` file and add your credentials:
   ```
   IBM_WATSON_API_KEY=your_ibm_watson_api_key_here
   IBM_WATSON_PROJECT_ID=your_project_id_here
   FLASK_SECRET_KEY=your_secure_secret_key_here
   ```

## Usage

1. **Start the application**
   ```bash
   python app.py
   ```

2. **Open your browser** and navigate to `http://localhost:5000`

3. **Upload a food image** and ask questions about its nutritional content

4. **Get instant analysis** with detailed nutritional breakdown and calorie estimates

## API Configuration

### IBM Watson AI Setup

1. Create an IBM Cloud account at [https://cloud.ibm.com](https://cloud.ibm.com)
2. Create a Watson Machine Learning service instance
3. Get your API key and project ID from the service credentials
4. Update the `.env` file with your credentials

## Project Structure

```
ai-nutrition-coach/
├── app.py                 # Main Flask application
├── requirements.txt       # Python dependencies
├── .env.example          # Environment variables template
├── .gitignore           # Git ignore rules
├── README.md            # Project documentation
├── static/
│   └── style.css        # CSS styling
└── template/
    └── index.html       # Main HTML template
```

## Key Functions

- **`input_image_setup()`**: Processes uploaded images and converts them to base64 encoding
- **`format_response()`**: Formats AI responses with proper HTML structure
- **`generate_model_response()`**: Handles communication with IBM Watson AI model

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Disclaimer

The nutritional information and calorie estimates provided are approximate and based on general food data. Actual values may vary depending on factors such as portion size, specific ingredients, preparation methods, and individual variations. For precise dietary advice or medical guidance, consult a qualified nutritionist or healthcare provider.

## Author

**Assad allah Alebrahim** - AI Engineer & Business Intelligence Analyst  
- GitHub: [@assadAllah630](https://github.com/assadAllah630)
- Company: Cogent Softech
- Location: Beirut, Lebanon

---

*Built with ❤️ using IBM Watson AI and Flask*