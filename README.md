# Skin Sight
Skin Skight is an AI skin health assistant which helps to identify your possible skin condition with just few clicks, before things get worse.

## Requirements
- [Node.js](https://nodejs.org/en/)
- [MongoDB](https://www.mongodb.com/try/download/community)
- [Python 3.6 or above](https://www.python.org/downloads/)

## Usage
1. Clone the repository
```
git clone https://github.com/Akash-Nadigepu/SkinSight.git
```

2. Navigate to the repository :open_file_folder:
```
cd SkinSight
```

3. Install the dependencies
```
cd frontend
npm install
cd ../backend
npm install
```
This might take a while to complete.

4. Create a `.env` file inside the backend folder and set the following credentials:
```
#.env
JWT_SECRET_KEY=
CLOUDINARY_CLOUD_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=
```
Get the Cloudinary credentials from your [Cloudinary Dashboard](https://cloudinary.com/console/)

5. Start the backend development server
```
npm run dev
```

6. Open a new terminal from `frontend` folder and run the frontend development server
```
npm run start
```

You can view the application at http://localhost:3000/.

## DOM
Project Directory Structure:

**SkinSight/**
- **AI/** (Directory for machine learning model and analysis)
    - `FinalModal.ipnyb` (Jupyter notebook with final model)
- **backend/** (Server-side logic and database handling)
    - `build/**` (Compiled files for production)
        - `index.html` (Server-side rendered entry point)
    - `controllers/**` (Code for handling API requests)
        - `login.js` (Handles user login)
        - `skin-results.js` (Manages skin disease prediction results)
        - `users.js` (User management functionality)
    - `middlewares/**` (Functions to intercept and process requests)
        - `upload.js` (Handles file uploads)
    - `models/**` (Data models for database interaction)
        - `skin-results.js` (Defines the skin result data structure)
        - `users.js` (Defines the user data structure)
    - `utils/**` (Reusable helper functions)
        - `config.js` (Application configuration settings)
        - `logger.js` (Logging functionality)
        - `middleware.js` (Common middleware functions)
        - `skins.js` (Skin disease-related utility functions)
- **frontend/** (Client-side user interface)
    - `build/**` (Compiled React application files)
        - `manifest.json` (Web app manifest details)
    - `public/**` (Static assets served directly)
        - `index.html` (Client-side entry point)
        - `manifest.json` (Web app manifest details again)
        - `robots.txt` (Robot exclusion instructions)
    - `src/**` (React component code and Redux logic)
        - `assets/**` (Static images and fonts)
        - `components/**` (Reusable UI components)
            - `BulmaSignupForm.js` (Signup form using Bulma CSS)
            - `Footer.js` (Website footer component)
            - ... (Other UI components)
        - `reducers/**` (Redux state management reducers)
            - `loggedUserReducers.js` (Maintains logged-in user data)
            - `notificationReducers.js` (Handles user notifications)
        - `services/**` (API interaction and data fetching logic)
            - `login.js` (Login API calls)
            - `signup.js` (Signup API calls)
            - `skin-result.js` (Skin disease prediction API calls)
            - `user.js` (User data management API calls)
        - `App.js` (Top-level React component)
        - `index.css` (Global CSS styles)
        - `index.js` (React app entry point)
        - `store.js` (Redux store configuration)
- `package.json` (Project dependencies and scripts)
- `.gitignore` (Files to exclude from version control)
- `README.md` (This file you're reading)

