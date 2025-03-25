# CurioAPI

CurioAPI is an open-source RESTful API that provides fascinating curiosities from around the world, categorized into different topics such as nature, animals, space, and history. The API supports multilingual responses (English and Spanish) and is freely available without authentication requirements.

## Features

- Provides random and categorized curiosities.
- Supports multiple languages (`en` and `es`).
- Open-source and free to use.
- Extendable categories and subcategories.
- Built with **Node.js** and **Express.js**.
- Uses **MongoDB** with **Mongoose**.

## Endpoints

### Get a Random Curiosity

```http
GET /curiosity/random/{language}
```

- `{language}`: `en` or `es`

### Get Curiosities by Category

```http
GET /curiosity/{category}/{language}
```

- `{category}`: `nature`, `animals`, `space`, `history`, etc.
- `{language}`: `en` or `es`

### Get Curiosity by ID

```http
GET /curiosity/id/{id}
```

- `{id}`: Unique curiosity ID.

## Example Response

```json
{
  "title": "The Eiffel Tower grows in summer",
  "description": "Due to thermal expansion, the Eiffel Tower can grow up to 15 cm during hot summer days.",
  "category": "history",
  "language": "en"
}
```

## Installation & Setup

### Prerequisites

- [Node.js](https://nodejs.org/)
- [MongoDB](https://www.mongodb.com/)

### Clone the Repository

```sh
git clone https://github.com/your-username/CurioAPI.git
cd CurioAPI
```

### Install Dependencies

```sh
npm install
```

### Configure Environment Variables

Create a `.env` file in the root directory:

```
PORT=3000
MONGO_URI=your_mongodb_connection_string
```

### Run the Server

```sh
npm start
```

The API will be available at `http://localhost:3000`

## Deployment

You can deploy this API using services like **Vercel, Railway, Render**, or your own **VPS** with Docker or PM2.

## Contributing

We welcome contributions! Feel free to fork the repository, create a new branch, and submit a pull request.

1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m "Add feature-name"`.
4. Push to the branch: `git push origin feature-name`.
5. Open a pull request.

## License

CurioAPI is open-source and licensed under the [MIT License](LICENSE).s
