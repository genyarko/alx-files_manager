# Files Manager

[![Coverage Status](https://coveralls.io/repos/github/genyarko/alx-files_manager/badge.svg?branch=main)](https://coveralls.io/github/genyarko/alx-files_manager?branch=main)

This is a straightforward file management API crafted with Express, MongoDB, Redis, Bull, and Node.js.

## Requirements

### Applications

- Node.js
- Yarn (the package manager/resource negotiator)

### APIs

- A Google API should be set up with at least an email sending scope, and a valid URL (e.g., `http://localhost:5000/`) should be one of the redirect URIs. Store the `credentials.json` file in the root directory of this project.

### Environment Variables

Store the required environment variables in a file named `.env`, where each line follows the format `Name=Value`. The table below lists the environment variables utilized by this server:

| Name                | Required | Description                                             |
| ------------------- | -------- | ------------------------------------------------------- |
| GOOGLE_MAIL_SENDER  | Yes      | The email address of the account responsible for sending emails to users. |
| PORT                | No (Default: `5000`) | The port at which the server should listen.        |
| DB_HOST             | No (Default: `localhost`) | The database host.                                  |
| DB_PORT             | No (Default: `27017`) | The database port.                                  |
| DB_DATABASE         | No (Default: `files_manager`) | The database name.                              |
| FOLDER_PATH         | No (Default: `/tmp/files_manager` (Linux, Mac OS X) & `%TEMP%/files_manager` (Windows)) | The local folder where files are saved. |

## Installation

- Clone this repository and navigate to the cloned repository's directory.
- Install the packages using `yarn install` or `npm install`.

## Usage

Start the Redis and MongoDB services on your system and execute `yarn start-server` or `npm run start-server`.

## Tests

- Create a separate `.env` file for the tests named `.env.test` and store the values of the environment variables for the testing environment in it.
- Run `yarn test` or `npm run test` to execute the end-to-end tests.

## Documentation

- TODO: Generate OpenAPI documentation with [**apidoc**](https://www.npmjs.com/package/apidoc).
+ Run `yarn test` or `npm run test` to execute the E2E tests.

## Documentation

+ TODO: Generate OpenAPI documentation with [**apidoc**](https://www.npmjs.com/package/apidoc).
