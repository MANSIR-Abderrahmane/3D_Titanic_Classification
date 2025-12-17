<!-- -->

# Titanic Classification and 3D Visualization Project

This project predicts passenger survival on the Titanic using a machine learning model and visualizes the ship with an interactive 3D model. Built Frem Scratch, it combines data science with web development to create an engaging user experience.

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Clapper%20Board.png" alt="Clapper Board" width="25" height="25" /> Project Showcase Video <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Movie%20Camera.png" alt="Movie Camera" width="25" height="25" />

<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Film%20Frames.png" alt="Film Frames" width="25" height="25" /> [Watch on LinkedIn](https://www.linkedin.com/feed/update/urn:li:activity:7330408127697207296/?commentUrn=urn%3Ali%3Acomment%3A(ugcPost%3A7330405178682032128%2C7330554997769687040)&dashCommentUrn=urn%3Ali%3Afsd_comment%3A(7330554997769687040%2Curn%3Ali%3AugcPost%3A7330405178682032128)&lipi=urn%3Ali%3Apage%3Ad_flagship3_profile_view_base%3BntAzI5rFTSy42Wma%2BvT2hQ%3D%3D)  
<img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Film%20Frames.png" alt="Film Frames" width="25" height="25" /> [Watch on YouTube](https://youtu.be/XhbllR8bzM0)


## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Light%20Bulb.png" alt="Light Bulb" width="25" height="25" /> Features

- **Survival Prediction**: A Random Forest model predicts survival based on passenger features (e.g., Age, Gender, Pclass, Embarked).
- **Interactive 3D Visualization**: A `.glb` model of the Titanic, rendered with Three.js, supports camera rotation.
- **Web Interface**: Users can input passenger details via a web form and view survival predictions in real-time.
- **Accuracy**: Achieves ~80% accuracy on the test dataset.

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Gear.png" alt="Gear" width="25" height="25" /> Tech Stack

<table align="center" style="width:100%; border-collapse: collapse; text-align: center;">
  <tr>
    <td align="center"><img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Window.png" alt="Window" width="25" height="25" /> FontEnd</td>
    <td align="center"><img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/X-Ray.png" alt="X-Ray" width="25" height="25" /> BackEnd</td>
    <td align="center"><img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Hand%20gestures/Mechanical%20Arm.png" alt="Mechanical Arm" width="25" height="25" /> Machine Learning</td>
    <td align="center"><img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/Bar%20Chart.png" alt="Bar Chart" width="25" height="25" /> Data Analysis</td>
  </tr>
  <tr>
    <td align="center"><img src="https://skillicons.dev/icons?i=html,css,js" align="center"><br/>+<br/><img src="https://skillicons.dev/icons?i=threejs" align="center"></td>
    <td align="center"><img src="https://skillicons.dev/icons?i=flask" align="center"></td>
    <td align="center">
      <img width="80" src="https://github.com/user-attachments/assets/3865d31c-9d7c-469f-a0d0-d85f40e56127" alt="XGBoost" title="XGBoost"/>
      <br/>
      <img src="https://skillicons.dev/icons?i=sklearn" align="center">
    </td>
    <td align="center">
       <img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/python.png" alt="Python" title="Python"/>
      <img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/numpy.png" alt="NumPy" title="NumPy"/>
      <img width="50" src="https://raw.githubusercontent.com/marwin1991/profile-technology-icons/refs/heads/main/icons/pandas.png" alt="Pandas" title="Pandas"/>
    </td>
  </tr>
</table>


- **Backend**: Flask (web server), scikit-learn (machine learning)
- **Frontend**: HTML, CSS, JavaScript, Three.js (3D rendering)
- **Machine Learning**: Random Forest Classifier (primary), Logistic Regression (baseline), explored XGBoost
- **Data**: Titanic dataset (`train.csv`, `test.csv`, `gender_submission.csv`)
- **Model Storage**: Pickle file (`titanic_model.pkl`)

## <img src="https://raw.githubusercontent.com/Tarikul-Islam-Anik/Animated-Fluent-Emojis/master/Emojis/Objects/File%20Folder.png" alt="File Folder" width="25" height="25" /> Project Structure

```
CodeAlpha_Titanic_Classification/
├── data/
│   ├── gender_submission.csv
│   ├── test.csv
│   └── train.csv
├── model/
│   └── titanic_model.pkl
├── backend/
│   ├── app.py              # Flask backend
│   ├── utils.py            # Prediction logic
│   ├── static/
│   │   ├── models/        # 3D model (.glb)
│   │   ├── style.css      # Frontend styling
│   │   └── script.js      # Frontend logic and Three.js
│   └── templates/
│       └── index.html     # Web interface
├── notebooks/
│   └── titanic_analysis.ipynb  # Data preprocessing and model training
├── README.md
├── requirements.txt
└── .gitignore
```

## Setup Instructions

1. **Clone the Repository**:
   ```bash
   git clone <repository-url>
   cd CodeAlpha_Titanic_Classification
   ```

2. **Install Dependencies**:
   Ensure Python 3.8+ is installed. Then, install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Prepare the Dataset**:
   Place `train.csv`, `test.csv`, and `gender_submission.csv` in the `data/` folder. These can be sourced from Kaggle's Titanic dataset.

4. **Train the Model** (optional):
   Run `titanic_analysis.ipynb` to preprocess data and train the Random Forest model. The trained model is saved as `model/titanic_model.pkl`.

5. **Run the Application**:
   Start the Flask server:
   ```bash
   python backend/app.py
   ```
   Access the web interface at `http://localhost:5000`.

6. **Interact with the App**:
   - Enter passenger details (e.g., Pclass, Sex, Age, SibSp, Parch, Fare, Embarked) in the web form.
   - View the survival prediction and probability.
   - Explore the interactive 3D Titanic model with camera rotation.

## Machine Learning Workflow

1. **Data Cleaning**:
   - Filled missing `Age` values with the median.
   - Filled missing `Embarked` values with the mode.
2. **Feature Encoding**:
   - `Sex`: male=1, female=0
   - `Embarked`: C=0, Q=1, S=2
3. **Model Training**:
   - Used Random Forest Classifier (`n_estimators=100`, `random_state=42`).
   - Features: Pclass, Sex, Age, SibSp, Parch, Fare, Embarked.
4. **Evaluation**:
   - Achieved ~80% accuracy on the test set.

## Usage

- **Prediction**: Submit passenger data via the web interface to get survival predictions.
- **Visualization**: Rotate and explore the 3D Titanic model using mouse controls.
- **Exploration**: Review `titanic_analysis.ipynb` for detailed data analysis and model training steps.

## Future Improvements

- Enhance preprocessing with feature engineering (e.g., family size).
- Tune model hyperparameters or compare additional algorithms (e.g., XGBoost).
- Improve the frontend UI with better styling and interactivity.
- Add input validation and detailed error messages.
- Deploy the app using Docker or a cloud platform like Heroku.

## Acknowledgments

- Built as part of the CodeAlpha Internship.
- Dataset sourced from Kaggle's Titanic competition.
- 3D model rendering powered by Three.js.

Feel free to explore the code, contribute, or reach out for questions!
