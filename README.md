# Dream11 Genie

Dream11 Genie is a small project that explores how AI can help with fantasy cricket. It looks at information about a match and its players, then suggests a fantasy playing XI, including a captain and vice-captain. Each selection comes with a short explanation.

The goal is to make it easier to think through a fantasy team by bringing player and match information together and turning it into a clear set of suggestions.

This project currently uses example cricket data, so its recommendations are for demonstration and learning purposes. It is not connected to live match information and does not guarantee results.

## Quick start

1. Open a terminal in this project folder.
2. Create and activate a virtual environment:

   Windows:
   ```bash
   python -m venv .venv
   .\.venv\Scripts\activate
   ```

   macOS/Linux:
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Add your Groq API key:
   ```bash
   copy .env.example .env
   ```
   If `.env.example` is not present, create a `.env` file with:
   ```bash
   GROQ_API_KEY=your_api_key_here
   ```
   Get a free key from: https://console.groq.com/keys

5. Run the project:


   CLI run:
   ```bash
   python run.py
   python run.py "CSK vs MI"
   ```

   Web UI:
   ```bash
   streamlit run app.py
   ```

## Notes

- The app uses sample cricket data from `data.py`, so it works offline for demo/testing.
- The CLI is the easiest way to quickly test the agent.
- The Streamlit app is useful for a browser-based demo.
