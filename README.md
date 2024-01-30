# LAB - Class 16

**Project:** Capital Finder

**Author:** Latherio Kidd

## Links and Resources

- **Back-end Server URL:** 
- **Front-end Application:** 

### Setup

**.env requirements (where applicable):**

- No .env variables required for this serverless function as it interacts with the public REST Countries API.

#### How to Initialize/Run Your Application

- This is a serverless function deployed on Vercel, so no local initialization is typically required.
- To interact with the function, use HTTP GET requests with query parameters.
  - Example: `GET [your Vercel function URL]/capital-finder?country=Chile`
  - This should return "The capital of Chile is Santiago."

#### How to Use Your Library

- The serverless function can handle two types of queries:
  1. **Country to Capital**: Pass a country name as a query parameter to get its capital.
     - E.g., `?country=Chile` responds with "The capital of Chile is Santiago."
  2. **Capital to Country**: Pass a capital name as a query parameter to find out which country it belongs to.
     - E.g., `?capital=Santiago` responds with "Santiago is the capital of Chile."

#### Tests

**How do you run tests?**

- Tests can be implemented using a framework like pytest to mock HTTP requests and responses.
- Local testing can be done using the Vercel CLI, if installed.

**Any tests of note?**

- Test cases should include various countries and capitals, including edge cases like countries with multiple capitals.
