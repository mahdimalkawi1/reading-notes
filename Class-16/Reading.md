# Read: Class 16

## Serverless Functions:

### Q1. What are the key characteristics of serverless computing, and how does it differ from traditional server-based architectures?

- Serverless computing:

1- No server management: Cloud provider handles infrastructure tasks.

2- Event-driven and stateless: Functions triggered by events, no persistent state.

3- Automatic scaling: Infrastructure scales based on demand.

4- Pay-per-use billing: Cost based on actual execution time.

5- Backend services integration: Managed services reduce operational overhead.

6- Rapid development and deployment: Streamlined workflows and deployment mechanisms.

7- Limited execution time and resource constraints.

- Traditional server-based architectures:

1- Require server management and provisioning.

2- Lack event-driven and stateless nature.

3- Manual scaling and capacity planning.

4- Continuous server costs, regardless of demand.

5- Manual configuration and management tasks.

6- Longer development and deployment process.

7- No built-in execution time or resource constraints.

### Q2. ow can one get started with Vercel, and what are the main steps involved in deploying a serverless function using Vercel?

#### To get started with Vercel and deploy a serverless function:


1- Sign up for a Vercel account.

2- Install the Vercel CLI.

3- Set up your project using vercel init.

4- Write your serverless function in a supported language.

5- Test the function locally with the Vercel CLI.

6- Deploy the function with vercel.

7- Test and monitor the deployed function.


### Q3. What are APIs, and how can they be utilized in Python applications to access and manipulate data from external sources?

- APIs (Application Programming Interfaces) are sets of rules and protocols that allow different software applications to communicate and interact with each other. 


We you can utilize APIs in your application using these steps:

1- Identify and understand the API.

2-Choose an HTTP library like requests.

3- Make HTTP requests to API endpoints.

4- Handle the response and extract relevant data.

5- Implement error handling.

6- Manipulate and process the data.

7- Handle pagination if necessary.


### Q4. What is the Requests library in Python, and how can it be used to interact with APIs by sending HTTP requests? Can you provide an example of a basic GET request using the Requests library? 


<br> The Requests library used to send HTTP requests in Python.It provides a simple and intuitive API that makes it easy to interact with APIs by sending HTTP requests and handling the responses.

- Example: 

``` python 
import requests

response = requests.get('https://api.example.com/data')

if response.status_code == 200:
    data = response.json()
    print(data)
else:
    print('Error:', response.status_code)

```
