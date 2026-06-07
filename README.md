# HMS Backend

Contains all infrastructure and backend services for the Hospital Management System.

## Services

| Service            | Port   | Description                         |
|--------------------|--------|-------------------------------------|
| PostgreSQL (app)   | 5432   | Main application database           |
| Redis              | 6379   | Caching / session store             |
| PostgreSQL (KC)    | (none) | Dedicated DB for Keycloak           |
| Keycloak           | 8080   | OpenID Connect Identity Provider    |

## Quick Start

```bash
docker compose up -d
```

Keycloak admin console: http://localhost:8080  
Credentials: `admin` / `admin`

## Pre-configured Test Users

| Username  | Password    | Role   |
|-----------|-------------|--------|
| admin     | Admin123!   | admin  |
| dr.chen   | Doctor123!  | doctor |

## OTP Setup
All users are required to set up a 6-digit TOTP authenticator on first login.
Use Google Authenticator, Authy, or any TOTP-compatible app.
