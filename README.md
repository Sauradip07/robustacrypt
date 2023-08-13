![ogimage (1)](https://github.com/bishal7679/robustacrypt/assets/70086051/c933237c-f0c1-4809-a009-ef60b1afc178)

# What is RobustaCrypt 🛡️
RobustaCrypt is an innovative tool that combines the power of various cutting-edge technologies to create a robust and secure password-protected application to fortify Your Website's Defense with Robust Password Protection. This project utilizes Next.js, the most amazing React framework on the planet, to deliver a seamless and dynamic user experience. With the integration of Tailwind CSS, Geist UI, and React Hook Form. RobustaCrypt achieves stunning and responsive designs along with efficient form validation. The project also leverages the capabilities of HarperDB for its database needs, ensuring data integrity and scalability with Auth0 authentication.

# Project Scope 🧪
We always need some kind of secured environment in order to implement any project and give access to some specific developers while developing the application privately. So, our tool `RobustaCrypt` will enhance the security layer of an under developing project privately by providing **DATA-SITEID** and **PASSWORD** for a particular project and only some specific people can access it who got the password for admission control into that project. The world will get a new taste of authentication with more reliable and secure way.

# Technologies Used ✨
- **Next.js**: The most amazing React framework for building server-rendered React applications.
  
- **TailwindCSS**: A utility-first CSS framework for creating responsive and stylish user interfaces.
- **Geist UI**: A modern and minimalist React component library for clean and aesthetic designs.
- **HarperDB**: A distributed and scalable database for handling data storage and retrieval efficiently.
- **Nextra**: A static site generation tool tailored for documentation websites.
- **Auth0**: A robust authentication and authorization platform to secure user interactions.
- **Axios**: A promise-based HTTP client for making API requests from the client-side.
- **React Hook Form**: A library for flexible and performant form validation in React applications.
- **Zod**: A TypeScript-first schema validation for efficient runtime data validation.
- **Web3forms**: Empowering form submissions with blockchain technology for enhanced security.
- **SWR**: A React hook for remote data fetching, with built-in caching and revalidation.
- **Typescript**: A statically typed superset of JavaScript for improved code quality and maintainability.
- **UglifyJS**: A powerful JavaScript minifier for optimizing script performance.
- **Vercel**: A cloud platform for hosting and deploying web applications with ease.

![frameworks](https://github.com/bishal7679/robustacrypt/assets/70086051/f849b33a-215c-4031-991e-0a7a47cce4a7)



# Various Features 🤯
🔹  `Secure Authentication`: Utilize Auth0 to ensure robust user authentication and authorization mechanisms.

🔹 `Efficient API Handling`: Perform API requests seamlessly using Axios for smooth data exchange.

🔹 `Dynamic Form Validation`: Leverage React Hook Form and Zod for effective and real-time form validation.

🔹 `Blockchain-powered Submissions`: Employ Web3forms to enhance form submissions with the security of blockchain.

🔹 `Data Management`: HarperDB facilitates efficient storage, retrieval, and management of application data using serverless Technology.

🔹 `Responsive UI`: Craft stylish and responsive user interfaces using TailwindCSS and Geist UI components.

🔹 `Real-time Data Fetching`: SWR enables efficient remote data fetching with automatic caching.

🔹 `Type-Safe Development`: TypeScript ensures type checking for a more reliable and maintainable codebase.

# Tracks We are using
- Auth0
  ![auth0](https://github.com/bishal7679/robustacrypt/assets/70086051/af3686e1-d241-42e8-8d98-29ef6fd8d3a5)

- Web 3.0

# How to set up locally 💻
 1. Fork the repository and then clone it
 ```bash
 git clone https://github.com/bishal7679/robustacrypt.git
```
2. Make sure you are using the node version 16. If you are using greater than this then you might face some issues, So Recommended having installed `nvm` onto your machine
Check REF :- https://github.com/nvm-sh/nvm

3. Follow below steps
### **Authentication**
Create your Auth0 account and set the required ENV value by creating one file `.env.local` in your root project scope
```bash
AUTH0_SECRET=
AUTH0_BASE_URL=
AUTH0_ISSUER_BASE_URL=
AUTH0_CLIENT_ID=
AUTH0_CLIENT_SECRET=
```
### **Database**
Then Sign up to HarperDB and create an instance [on their Studio](https://studio.harperdb.io/sign-up).

- Choose the cloud provider of your preference 
- Give the instance a name and give its credentials
- Pick the specs for the instance - there's a free tier available
- Review the information and confirm the instance creation
- It can take minutes to create a HarperDB instance. Stretch your legs and drink some water while you wait for it.
```bash
HARPERDB_URL=
HARPERDB_KEY=
```
### **JWT Tokens**
RobustaCrypt uses [JSON Web Tokens (JWT)](jwt.io) and requires some environment variables to work with them. You can use the same generate-secret command for suitable and secure strings.
Command for generate secret:- 
```bash
node -e "console.log(crypto.randomBytes(32).toString('hex'))"
```
### **Base URL**
To generate the script and all the URLs correctly, pointing to your instance, add a new environment variable called `NEXT_PUBLIC_BASE_URL` pointing to the same domain as the `AUTH0_BASE_URL` variable.

We don't use the same environment variable because in providers like Vercel, the variable needs to be prefixed with `NEXT_PUBLIC_` to be exposed to the front-end.

### **Final Steps**
Confirm that you have all these environment variables configured on your preferred provider and that you run the build script during deployment.
```bash
AUTH0_SECRET=
AUTH0_BASE_URL=
AUTH0_ISSUER_BASE_URL=
AUTH0_CLIENT_ID=
AUTH0_CLIENT_SECRET=
HARPERDB_URL=
HARPERDB_KEY=
HASH_SECRET=
JWT_TOKEN=
TOKEN_SECRET=
NEXT_PUBLIC_BASE_URL=
```
After that, install all the dependencies
```bash
yarn
yarn run build
yarn run start
```
Now access your application on localhost:3000

# Demo Videos

 - ### Exploration

   

https://github.com/Sauradip07/robustacrypt/assets/82558066/df69ebc5-04db-463f-9c80-939e650a0c36


   
 - ### Working Demo

   

https://github.com/Sauradip07/robustacrypt/assets/82558066/10c700e5-8318-4bc2-8c58-e93d33ab9ff0




# Integrated PWA (Progressive Web App)
- PWA helps you to run our tool as a website on Desktop and also you can use our tool on Mobile as a web app with all responsiveness and persistance of data
  It will help you to not face any Installation Hussles and loading time etc.
  
  ![pwa](https://github.com/bishal7679/robustacrypt/assets/70086051/0ee4c7af-de79-4a79-82c6-ef39cbba9a0f)


# DevOps Integration to serve our product to End user
- We have created docker image of our application and pushed it to ECR repository
 ![docker](https://github.com/bishal7679/robustacrypt/assets/70086051/48049ccf-7374-4a92-81fc-9ff4587003b9)

- We have deployed our application to Amazon ECS cluster with ALB (Application load balancer) which will be used to access our tool by end user
  ![13-08-2023:12:36:06](https://github.com/bishal7679/robustacrypt/assets/70086051/2071d415-9ea0-418b-994b-60d53b3da103)

- Also added CI/CD pipeline with GitHub Action to automatic integrate our changes to github repo and deploy it automatically to ECS cluster so that it effect the changes to production
  
![cicd](https://github.com/bishal7679/robustacrypt/assets/70086051/b6a9c0d3-531e-4077-b382-f1b4a9b82cd5)



# How RobustaCrypt works?
For RobustaCrypt to work on your site, you will have to inject a small snippet that you can find in your [site's dashboard]().

It is a tiny script (a little more than a kilobyte), therefore it does not slow down your page at any costs. And other thing that it requires is just `staticshield-div` class (or class Name in react ecosystem) on the top level div of the page.

This script looks like below for password protecting an HTML page
```bash
<script src='https://robustacrypt.vercel.app/script.js' data-site-id='<SITE-ID>' data-cap='<CAPTION>'></script>
<noscript>
	<meta http-equiv='refresh' content='0; url=https://robustacrypt.vercel.app/errors/noscript'/>
</noscript>
```
The `<SITE-ID>` and `<CAPTION>` are the two fields you will find in dashboard itself. You will be able to find the complete snippet there, with prefiled `<SITE-ID>` and `<CAPTION>` fields. All you have to do, copy and paste it in the right place, and you can find that place here in the docs.

If you are not getting this, that's fine. You can directly jump into your favorite framework's documentation [blog]() and you will find everything needed there 😄
# Under the hood🔥
When the password-protected page with the snippet loads, the script looks for a valid token in the browser storage. If it does not find one, it will redirect you/the end user to a RobustaCrypt hosted login page where the user will be able to log in with password

If the script finds a `token`, it validates it by sending it to RobustaCrypt's servers. If the token is valid, the user is then allowed to view and interact with the webpage.

If the `token` happens to be invalid, the user is then redirected to the login page. The token does not become invalid usually unless it is edited/modified by anyone manually.

The `token` also becomes invalid if it has been expired. The expiration duration can be increased or decreased in the dashboard.

Now you can start integrating RobustaCrypt in your website now.

# Contribution Guidelines
Please refer to our contribution guide if you wish to contribute to the project 
# License🧾
RobustaCrypt is released under the MIT License.
# ❤️ Show your support
Give a ⭐ if this project helped you, Happy learning!
