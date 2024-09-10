# API Testing Overview
As I continue developing my API testing skills, I've worked on several projects focused on validating functionality, performance, and security through automated tests. 
Using Postman and its built-in JavaScript runtime, I’ve compiled a comprehensive set of tests covering both functional and integration scenarios. These focus on:

- **Endpoint validation**: Verifying response codes and payload structures.
- **Error handling**: Testing edge cases and failure scenarios.
- **Security**: Ensuring proper authentication and authorization.
These tests are designed for seamless integration with CI/CD pipelines, executable through a simple command-line interface. Detailed setup instructions are provided below.

# Projects
## Grocery Store API
* **Flow:** Tests cover a full user journey—finding a product, adding it to the cart, updating the cart, creating and modifying an order, and finally, deleting the order.
* **Additional Tests:** Include authentication checks and various invalid input cases.

## Trello API
* **Flow**: Simulates creating a board, adding multiple lists, creating and moving cards between lists, and deleting the board at the end.

# Running the Tests
1. Clone the repository.
2. Install dependencies:
* `brew install node` (to install npm)
* `brew install newman` (to run tests via the terminal)
3. Navigate to the project directory and run:
* `newman run <collectionName.json>`
* For GroceryStoreDemoCollection, specify the environment:
  * `newman run GroceryStoreDemo.postman_collection.json -e Testing.postman_environment.json` or
  * `newman run GroceryStoreDemo.postman_collection.json -e Production.postman_environment.json`

Alternatively:

Clone the repository and run the test suites directly within Postman.

##
For issues or queries, please contact me at liliya.vovk.17@gmail.com.
