### Backend Setup

1. Navigate to the backend directory:
    ```bash
    cd fruit-ai-backend
    ```

2. Create and activate a virtual environment:
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows: venv\Scripts\activate
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

4. Configure the Flask application:

   Update the `config.py` file with your MongoDB Atlas URI:
    ```python
    class Config:
        MONGO_URI = 'mongodb+srv://<username>:<password>@cluster0.mongodb.net/faqs?retryWrites=true&w=majority'
    ```

5. Run the Flask application:
    ```bash
    python app.py
    ```

6. Open your browser and navigate to `http://localhost:5000` to access the backend API.
