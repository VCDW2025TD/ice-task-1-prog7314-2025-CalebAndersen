# MemeStream RESTful API

This is the backend RESTful API for the MemeStream application, built with Node.js, Express, and MongoDB.

## Setup

1.  **Navigate to the API directory:**

    ```bash
    cd 01-RestfulAPI
    ```

2.  **Install dependencies:**

    ```bash
    npm install
    ```

3.  **Create a `.env` file:**

    Create a file named `.env` in the `01-RestfulAPI` directory with the following content:

    ```
    PORT=3000
    MONGODB_URI=your_mongodb_connection_string
    ```

    **Replace `your_mongodb_connection_string` with your actual MongoDB Atlas or local MongoDB connection string.**

## Running the API

To start the server, run:

```bash
npm start
```

(Note: You might need to add `"start": "node index.js"` to the `scripts` section of your `package.json` file if it's not already there.)

## API Endpoints

*   **`GET /memes`**: Fetches all memes.
*   **`GET /memes?userId=...`**: Fetches memes by a specific user.
*   **`POST /memes`**: Saves new meme data. Requires a JSON body with `userId`, `imageUrl`, `caption`, `lat`, and `lng`.