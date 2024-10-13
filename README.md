# 🎶 Emotion-Based Background Music Selector

This project is a deep learning-based web application that detects user emotions in real-time and selects background music tailored to their mood. Using facial emotion recognition and music recommendations, it brings a personalized, interactive music experience to users. Ideal for improving focus, relaxation, and enjoyment based on the user's emotional state.

---

## 🔗 Features
- **Real-Time Emotion Detection**: Uses a webcam to capture facial expressions, which are analyzed by a deep learning model.
- **Music Recommendations**: Suggests background music that aligns with the detected emotions.
- **Seamless Integration**: Automatically updates music suggestions based on changing emotions.
- **Simple User Interface**: Easy-to-use design that makes real-time feedback and control intuitive.

---

## 📋 Technologies

- **Frontend**:
  - **React.js**: For a dynamic, responsive UI to capture and display emotions in real time.
  - **JavaScript/HTML/CSS**: Core web technologies for handling webcam input, interactions, and layout.
  
- **Backend**:
  - **Flask/FastAPI**: Serves as an API backend to handle emotion detection and music recommendation logic.
  - **TensorFlow/Keras**: For building and running the emotion recognition model.
  - **Spotify API**: Fetches playlists and songs based on mood tags, providing the music selection.

- **Data & Model**:
  - **FER-2013 Dataset**: Used for training the emotion detection model.
  - **Emotion Detection Model**: A Convolutional Neural Network (CNN) trained on the FER-2013 dataset for classifying facial emotions.

---

## 📦 Setup

### Prerequisites
- Python 3.7+
- Node.js & npm
- Spotify Developer Account

### Installation Steps

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/emotion-music-selector.git
   cd emotion-music-selector
   ```

2. **Backend Setup**:
   - **Install Dependencies**:
     ```bash
     pip install -r requirements.txt
     ```
   - **Train/Load the Model**:
     - Either train the model using the FER-2013 dataset or load a pre-trained model.
     - Place the model file in the `models` directory.

3. **Spotify API Setup**:
   - Register on [Spotify Developer Dashboard](https://developer.spotify.com/dashboard/applications) and create an app to get your API keys.
   - Create a `.env` file in the root directory with:
     ```
     SPOTIFY_CLIENT_ID=your_client_id
     SPOTIFY_CLIENT_SECRET=your_client_secret
     ```

4. **Frontend Setup**:
   - **Navigate to Frontend**:
     ```bash
     cd frontend
     ```
   - **Install Dependencies**:
     ```bash
     npm install
     ```
   - **Run Frontend**:
     ```bash
     npm start
     ```

5. **Start the Backend Server**:
   - Navigate back to the main directory and run:
     ```bash
     python app.py
     ```

6. **Open in Browser**:
   - Go to `http://localhost:3000` to interact with the application.

---

## 🎮 Usage Guide

1. **Access Webcam**: Grant permission to access the webcam, which will capture facial expressions in real-time.
2. **Emotion Detection**: The app detects your current emotion based on facial analysis and displays it.
3. **Music Selection**: Depending on your mood, the app fetches a playlist from Spotify and begins playback.

---

## 🎨 Emotion to Music Mapping

| Emotion       | Music Category     |
|---------------|--------------------|
| Happy         | Upbeat, Pop, Dance |
| Sad           | Acoustic, Slow     |
| Angry         | Heavy Rock         |
| Neutral       | Chill, Lo-Fi       |
| Surprised     | Random/Experimental|

---

## 🛠️ Future Improvements

- **Additional Emotions**: Support a wider range of emotions.
- **Improved Model**: Fine-tune the model with a larger, diverse dataset.
- **Enhanced Music Mapping**: Allow users to customize their music preferences for each emotion.

---

## 🤝 Contributing

1. Fork the repository.
2. Create a new branch for your feature (`git checkout -b feature-branch`).
3. Commit your changes (`git commit -m 'Add new feature'`).
4. Push to the branch (`git push origin feature-branch`).
5. Open a Pull Request.

---

## 📄 License
This project is licensed under the MIT License.

---

## 🌐 Acknowledgements

- [FER-2013 Dataset](https://www.kaggle.com/datasets/msambare/fer2013)
- [Spotify API](https://developer.spotify.com/documentation/web-api/)
- Inspiration from various emotion-based music recommendation research papers
