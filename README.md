Disclaimer: This project is for educational purposes only and is not affiliated with or endorsed by Spotify
Prerequisites
Node.js 18+
MongoDB (local or MongoDB Atlas)
A free Cloudinary account
Getting Started
1. Clone the repository
bash
git clone https://github.com/<your-username>/spotify-clone.git
cd spotify-clone
2. Backend setup
bash
cd server
npm install
cp .env.example .env

Edit .env:

env
PORT=5000
MONGO_URI=mongodb://localhost:27017/spotify-clone
JWT_SECRET=replace_with_a_long_random_string
CLIENT_URL=http://localhost:5173

CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret

Start the server:

bash
npm run dev
3. Frontend setup
bash
cd ../client
npm install

Create client/.env:

env
VITE_API_URL=http://localhost:5000/api

Run the app:

bash
npm run dev

Open http://localhost:5173.
