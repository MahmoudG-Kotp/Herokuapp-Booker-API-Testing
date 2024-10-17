# Test Herokuapp Booking API

This repository contains a Postman collection for testing the Booking API. The collection includes various requests to perform operations related to booking management, along with automated test cases to verify the API's functionality.

## Collection Overview

### Requests

1. **Booking Request**
   - Method: `POST`
   - Endpoint: `{{BaseURL}}/booking`
   - Description: Sends a booking request and retrieves a booking ID.

2. **All Booking IDs**
   - Method: `GET`
   - Endpoint: `{{BaseURL}}/booking`
   - Description: Retrieves all booking IDs.

3. **Booking ID**
   - Method: `GET`
   - Endpoint: `{{BaseURL}}/booking/:id`
   - Description: Retrieves a specific booking by ID.

4. **Authentication Request**
   - Method: `POST`
   - Endpoint: `{{BaseURL}}/auth`
   - Description: Authenticates a user and retrieves an authentication token.

5. **Update Booking ID**
   - Method: `PUT`
   - Endpoint: `{{BaseURL}}/booking/:id`
   - Description: Updates an existing booking by ID.

6. **Delete Booking ID**
   - Method: `DELETE`
   - Endpoint: `{{BaseURL}}/booking/:id`
   - Description: Deletes a booking by ID.

### Automated Test Cases

The collection includes automated test cases for each request, verifying the following:

1. **Booking Request**
   - Asserts that the booking request succeeds with a status code of 200.

2. **All Booking IDs**
   - Asserts that all booking IDs are retrieved successfully with a status code of 200.

3. **Booking ID Retrieval**
   - Asserts that the booking ID is retrieved successfully with a status code of 200.
   - Validates that the first name in the retrieved response matches the expected value.

4. **Authentication Request**
   - Asserts that the authentication request succeeds with a status code of 200.
   - Validates that the retrieved token is not empty.

5. **Update Booking ID**
   - Asserts that the booking update request succeeds with a status code of 200.

6. **Delete Booking ID**
   - Asserts that the booking deletion request succeeds with a status code of 201.

### Getting Started

1. Clone the repository to your local machine.
2. Import the Postman collection into Postman.
3. Set your `BaseURL` environment variable to point to the API you want to test.
4. Run the collection to execute the requests and automated tests.

### Contributing

Feel free to submit issues or pull requests if you want to contribute to the project!

### License

This project is licensed under the MIT License.

### Output

![apis](https://github.com/user-attachments/assets/2e539d5f-7fb0-481b-b5a9-478ccca63e37)
