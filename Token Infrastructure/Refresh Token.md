# Refresh Token

## Definition

A Refresh Token is a long-lived credential used to obtain new access tokens after expiration.

## Key Ideas

- Usually stored in HttpOnly cookies.
- Not sent through Authorization headers.
- Can be revoked independently.

## Relationships

### Related Concepts

- [[Access Token]]
- [[Refresh Flow]]
- [[Cookie Authentication]]

### Depends On

- [[Token Signing]]

### Enables

- [[Session Management]]