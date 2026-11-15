# Experiment 9: Login System (Node.js, Express, MongoDB, JWT)

## Run on your computer
1. Copy `.env.example` to `.env` and fill in the two values
2. Run:
```
npm install
npm start
```
Open http://localhost:3000

## Environment variables
- `MONGO_URI`: your MongoDB link (database name: `logindb`)
- `JWT_SECRET`: any random text

## MongoDB Atlas (free database)
1. Create a free cluster at https://www.mongodb.com/atlas
2. Database Access: add a user with a simple password (letters and numbers only)
3. Network Access: add IP address `0.0.0.0/0`
4. Connect > Drivers > copy the link, replace `<password>`, and add the database name before the `?`
   Example: `mongodb+srv://user:password@cluster0.xxxxx.mongodb.net/DBNAME?retryWrites=true&w=majority`

## Deploy on Render (free)
1. Log in at https://render.com with GitHub
2. New > Web Service > choose this repo
3. Build Command: `npm install`
4. Start Command: `npm start`
5. Instance type: Free
6. Environment variables: add `MONGO_URI` and `JWT_SECRET`
7. Click **Create Web Service** and open the link when it says Live

The free plan sleeps when nobody uses it, so the first open can take about a minute.
