# Pokemon API

## Endpoints

### Authentication

- `POST /register`: Register a new user
- `POST /login`: Login and receive a token

### Pokemon

- `POST /pokemon`: Create a new Pokemon (requires authentication)
- `GET /pokemon`: Get all Pokemons (supports pagination)
- `GET /pokemon/:id`: Get a Pokemon by ID
- `PUT /pokemon/:id`: Update a Pokemon by ID
- `DELETE /pokemon/:id`: Delete a Pokemon by ID

## Authentication

- Use the token received from the login endpoint as a Bearer token in the Authorization header for protected endpoints.

## Error Handling

- All endpoints return appropriate HTTP status codes and error messages.

## Rate Limiting

- The API is rate-limited to 100 requests per 15 minutes per IP address.

