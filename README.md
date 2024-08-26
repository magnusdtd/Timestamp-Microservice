# Timestamp Microservice

## Overview

The Timestamp Microservice is a simple API that returns the current timestamp in both Unix and UTC formats. It can also convert a given date string or Unix timestamp to both formats.

## Features

- **Current Timestamp**: Get the current timestamp in Unix and UTC formats.
- **Date Conversion**: Convert a given date string or Unix timestamp to Unix and UTC formats.

## Endpoints

### Get Current Timestamp

- **URL**: `/api/timestamp`
- **Method**: `GET`
- **Response**:
  ```json
  {
    "unix": 1633046400000,
    "utc": "Fri, 01 Oct 2021 00:00:00 GMT"
  }

### Convert Date String or Unix Timestamp

- **URL**: `/api/timestamp/:date_string`
- **Method**: `GET`
- **URL Parameters**:
    - ***date_string***: A date string (e.g., 2021-10-01) or Unix timestamp (e.g., 1633046400000).
- **Response**:
  ```json
  {
    "unix": 1633046400000,
    "utc": "Fri, 01 Oct 2021 00:00:00 GMT"
  }


## Usage

1. **Get Current Timestamp**:
    I haven't had a domain yet, therefore I use "<my-domain.com>" to demo this project.
   - Send a `GET` request to `/api/timestamp`.
   - Example:
     ```sh
     curl https://<my-domain.com>/api/timestamp
     ```

2. **Convert Date String or Unix Timestamp**:
   - Send a `GET` request to `/api/timestamp/:date_string`.
   - Example:
     ```sh
     curl https://<my-domain.com>/api/timestamp/2021-10-01
     ```

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/your-username/timestamp-microservice.git
   ```
2. Navigate to the project directory:
   ```sh
   cd timestamp-microservice
   ```
3. Install dependencies:
   ```sh
   npm install
   ```
4. Start the server:
   ```sh
   npm start
   ```

## Technologies Used

- Node.js
- Express.js

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## Contact

For any questions or feedback, please contact [tdat0306@gmail.com](mailto:tdat0306@gmail.com).
```
