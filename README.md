# **AI Personal Trainer App**  

## **Overview**  
The AI Personal Trainer App is a mobile application designed to revolutionize the way individuals track their fitness progress and workouts. It leverages AI technology for exercise form recognition, tracks repetitions and sets, and provides personalized workout plans. The app also integrates gamification features such as badges and leaderboards to keep users motivated.

The target audience includes beginners to casual users aged 18–40, with the app initially developed for Android and iOS smartphones, with plans for future integration with wearable devices.  

---

## **Features**  
### **Core Features**  
- **Exercise Tracking**:  
  - Tracks repetitions and sets.  
  - Optional AI-based form recognition using MediaPipe.  
- **Workout Routines**:  
  - Predefined plans for beginners, intermediates, and advanced users.  
  - Personalized workout plans based on fitness goals.  
  - Ability to create custom workout programs.  
- **Progress Tracking**:  
  - Weekly and monthly performance summaries.  
  - Visual charts and analytics using Chart.js.  
- **User Profile Management**:  
  - User profiles with health metrics (height, weight, BMI, fitness level).  
  - Syncing with wearables and APIs for real-time data.  
- **Gamification**:  
  - Badges for milestone achievements.  
  - Leaderboards for community engagement.  

### **Future Enhancements**  
- Wearable device integration.  
- Advanced AI for detecting complex workout forms.  
- Advanced analytics and tailored recommendations.  

---

## **Project Structure**  

The project is divided into three main components: **Frontend**, **Backend**, and **AI Models**.  

```plaintext
ai_trainer_project/
├── frontend/                  # Flutter-based mobile app
│   ├── lib/
│   │   ├── screens/           # UI screens (e.g., Home, Workout, Progress, Profile)
│   │   ├── widgets/           # Reusable UI components
│   │   ├── services/          # API calls and Firebase interactions
│   │   └── main.dart          # App entry point
│   └── assets/                # Images, icons, and other assets
├── backend/                   # Django backend
│   ├── ai_trainer_backend/
│   │   ├── settings.py        # Django configuration
│   │   ├── urls.py            # API routing
│   │   └── wsgi.py            # Backend entry point
│   ├── users/                 # User management app
│   │   ├── models.py          # Database models
│   │   ├── views.py           # API views
│   │   ├── serializers.py     # Data serializers
│   │   └── urls.py            # Endpoints for user management
│   └── requirements.txt       # Backend dependencies
├── ai-models/                 # AI/ML scripts or integrations
│   └── mediapipe/             # MediaPipe scripts for form recognition
├── docs/                      # Documentation and resources
│   ├── architecture_diagrams/ # App architecture diagrams
│   └── wireframes/            # UI/UX wireframes and mockups
├── .gitignore                 # Files to ignore in Git
└── README.md                  # Project documentation (this file)
```

---

## **Technologies Used**  
### **Frontend**:  
- Flutter (Dart): For building cross-platform mobile applications.  
- Chart.js: For progress visualization charts.  

### **Backend**:  
- Django REST Framework (Python): For APIs and data processing.  
- Firebase: For real-time database and authentication.  

### **AI Models**:  
- MediaPipe: For AI-based form recognition.  
- Pre-trained Model: COCO for pose detection.  

---

## **Getting Started**  

### **1. Clone the Repository**  
```bash
git clone https://github.com/yourusername/ai_trainer_project.git
cd ai_trainer_project
```

### **2. Setup Frontend**  
- Install Flutter: [Flutter Installation Guide](https://flutter.dev/docs/get-started/install).  
- Run the app:  
  ```bash
  cd frontend
  flutter pub get
  flutter run
  ```

### **3. Setup Backend**  
- Install Python and dependencies:  
  ```bash
  cd backend
  pip install -r requirements.txt
  python manage.py runserver
  ```

### **4. Firebase Configuration**  
- Add `google-services.json` (Android) or `GoogleService-Info.plist` (iOS) to the `frontend` project.  
- Configure Firebase in the backend for authentication and database.  

---

## **Contributing**  
Contributions are welcome! Feel free to submit a pull request or open an issue for suggestions or bug fixes.  

---

## **License**  
This project is licensed under the [MIT License](LICENSE).  

---

