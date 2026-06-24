# JWT Authentication

## Definition

JWT Authentication is an authentication mechanism where the backend issues signed JSON Web Tokens that clients send with requests to prove identity.

## Key Ideas

- Identity is encoded into a signed token.
- Backend creates and validates tokens.
- Frontend carries access tokens.
- Tokens are stateless from the backend's perspective.

## Relationships

### Related Concepts

- [[Access Token]]
- [[Refresh Token]]
- [[Authentication]]
- [[Authorization]]
- [[JSON Web Token (JWT)]]

### Depends On

- [[Token Signing]]
- [[User Authentication]]

### Enables

- [[Protected API]]
- [[Session Management]]

## Notes

JWT authentication commonly combines short-lived access tokens with longer-lived refresh tokens.