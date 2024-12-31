# Go Devcontainer

## Description

This project sets up a local environment for a Go project using VSCode devcontainer and Docker Compose to run multiple services.

## Steps

### Step 1: Create .env file

Create a `.env` file with the following content:

```properties
DB_USER=dev
DB_PASSWORD=secret
DB_NAME=dev_db
DB_HOST=db

PGADMIN_DEFAULT_EMAIL=anonymous@example.com
PGADMIN_DEFAULT_PASSWORD=secret
```

### Step 2: Install VSCode Remote - Containers Extension

Install the [VSCode Remote - Containers](https://marketplace.visualstudio.com/items?itemName=ms-vscode-remote.remote-containers) extension. Then, open the project in the devcontainer.

### Step 3: Verify the Connection to `postgres`

Run the following command to verify the connection to `postgres`:

```go
go run cmd/db/main.go
```

### Step 4: Access pgAdmin

Access pgAdmin at [http://localhost:5050](http://localhost:5050).
