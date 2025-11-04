# Film Manager Service

## Overview
This server was generated using the [swagger-codegen](https://github.com/swagger-api/swagger-codegen) project.
The project uses an OpenAPI specification (openapi.yaml or openapi.json) as a blueprint to generate the server stub.


## Generating the Server Stub

You can generate the Node.js server stub from their OpenAPI specification using either of the following methods:

### Using Swagger Editor (recommended)

- Download the project [repository](https://github.com/swagger-api/swagger-editor/archive/refs/tags/v4.14.7.zip) and unzip it.

- Open index.html (double-click) to lounch Swagger Editor in your browser.

- Paste your OpenAPI document (openapi.yaml or openapi.json).

- Generate Server → nodejs-server → Download.

### Using Swagger Codegen CLI (Java required)

- Download the Swagger Codegen CLI jar [here](https://repo1.maven.org/maven2/io/swagger/codegen/v3/swagger-codegen-cli/3.0.72/swagger-codegen-cli-3.0.72.jar).

- Run the following command:

```
java -jar swagger-codegen-cli-3.0.72.jar generate -i openapi.json -l nodejs-server -o output-folder/
```

## Note

When extracting the compressed archive containing the generated server stub, the default Windows decompression tool may display security warnings and block the operation. To avoid these issues, consider using alternative archiving tools such as WinRar or 7-Zip. Alternatively, generating the stub directly using the Swagger Codegen CLI jar does not typically cause these problems.

## Integration

Once you have generated the server stub, integrate this repository into it:

Copy all files and folders from this repo into the generated server stub and replace duplicates in the stub with the ones from this repo (`package.json`, `index.js`, `utils/` folder, `service/` folder).

After integrating this repository into the generated server stub, you should complete the remaining parts of the implementation:

1) `index.js` – implement the API routes and set up the JSON validator according to the instructions in the TODO comments.

2) `components/` – replace all occurrences of the placeholder "/change/me" with the correct API URLs.

3) `controllers/` – implement your controller logic and connect it to the routes in index.js.


## Running the Server

Install dependencies and start the server:

```
npm install
npm start
```
Open Swagger UI to view the API documentation:
http://localhost:3001/docs


## Testing the App

Use the following credentials for testing:

Username: user.dsp@polito.it

Password: password

In the database folder you can find a [list](/database/passwords_databases.txt) of the users with relative password.

## Pagination

To set the number of items per page in API pagination, modify the ELEMENTS_IN_PAGE variable in utils/constants.js.
