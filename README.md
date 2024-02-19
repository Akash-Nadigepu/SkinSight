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
