# GenreSync: AI-Powered Spotify Analytics & Recommendations

An interactive web application built with Streamlit that integrates the Spotify Web API and OpenAI's GPT-4 models to analyze user music preferences and generate personalized AI insights.

## Core Features
* **Music Preference Visualization:** Fetches user data and audio features via the Spotify Web API to visualize listening habits and identify gaps across 20+ distinct genres.
* **AI-Powered Insights:** Leverages OpenAI GPT-4 and GPT-4o models to provide deep, personalized genre analysis and rare song suggestions tailored to the user's historical data.
* **Conversational Music Bot:** Features an embedded, context-aware chat interface for interactive music recommendations and discovery.
* **Secure Authentication:** Implements standard OAuth flows to authenticate users securely, ensuring private Spotify data remains protected.

## Technology Stack
| Component | Technology |
| :--- | :--- |
| **Frontend / Framework** | Streamlit, Python |
| **Music Data Integration** | Spotify Web API (via Spotipy) |
| **Artificial Intelligence** | OpenAI API (GPT-4 / GPT-4o) |

## Local Installation & Setup

1. **Clone the repository**
```bash
git clone [https://github.com/yycapalot/GenreSync-AI_Application.git](https://github.com/yycapalot/GenreSync-AI_Application.git)
cd GenreSync-AI_Application

2. **Create a virtual environment (Recommended)**
```bash
python -m venv env
# On Mac/Linux:
source env/bin/activate  
# On Windows:
env\Scripts\activate

3. **Install dependencies**
```bash
pip install -r requirements.txt

4. Environment Variables Configuration
For security reasons, API keys are not included in this repository. You must create a .env file in the root directory and add your specific credentials for both Spotify and OpenAI to run the application:
```bash
# Spotify API Credentials (Get these from developer.spotify.com)
SPOTIPY_CLIENT_ID="your_spotify_client_id_here"
SPOTIPY_CLIENT_SECRET="your_spotify_client_secret_here"
SPOTIPY_REDIRECT_URI="http://localhost:8501"

# OpenAI API Credentials (Get this from platform.openai.com)
OPENAI_API_KEY="your_openai_api_key_here"
