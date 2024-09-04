
---

# Build a Full-Stack React Application with AWS Amplify

This project demonstrates how to build and deploy a full-stack React application using AWS Amplify. Integrate your React frontend with a serverless backend and leverage Amplify's hosting capabilities to create a scalable, globally available web application.

![React Application](/src/assets/5.png)

## Key Features

- **React Application:** Develop a single-page application (SPA) using React and Vite for optimized performance.
- **AWS Amplify Integration:** Utilize Amplify for hosting, backend setup (authentication, data, storage), and other cloud services.
- **Full-Stack Capabilities:** Implement user authentication, data storage, and media uploads within your React app.

## Prerequisites

Ensure you have the following:

- A GitHub account
- An AWS account with permissions to access Amplify and related services (Cognito, AppSync, S3)
- Basic understanding of React and AWS services

## Setup Instructions

### 1. Create a React Application

Initialize a new React application with Vite:

![Build Your App in Amplify: ](/src/assets//1.png)

```bash
npm create vite@latest my-react-app --template react
cd my-react-app
npm install
```

### 2. Push to GitHub

Set up a Git repository and push your code:

```bash
git init
git remote add origin <your-github-repo-url>
git add .
git commit -m "Initial commit"
git push -u origin main
```

### 3. Deploy and Customize Your App with AWS Amplify

1. Sign in to your AWS account and open the [Amplify console](https://console.aws.amazon.com/amplify).
2. Connect your GitHub repository to Amplify by following the setup wizard.
3. Configure build settings and deploy your app to a domain provided by Amplify (e.g., `<your-app>.amplifyapp.com`).

![Deploy with AWS Amplify](/src/assets/2.png)

### 4. Implement Amplify Authenticator Feature
Set up the Amplify Authenticator to handle user authentication:

1. Install Amplify libraries:
   ```bash
   npm install aws-amplify @aws-amplify/ui-react
   ```
2. Initialize and configure Amplify in your React app:
   - Follow the [AWS Amplify documentation](https://docs.amplify.aws/) to set up Amplify for authentication, data, and storage.

![Deploy Amplify Sandbox](/src/assets/3.png)


### 5. Configure Backend Features in Amplify
Set up backend features like authentication, data storage, and file management:

1. Initialize and configure backend resources using Amplify CLI

```
amplify init
amplify add auth
amplify add api
amplify add storage
amplify push
```
2. Integrate these features into your React app using Amplify libraries.
![Implement Amplify Authenticator Feature](/src/assets/4.png)

### 6. Clean Up Resources

To avoid incurring unwanted charges:

1. Remove the Amplify app from the Amplify console.
2. Delete any associated resources, such as S3 buckets and Cognito user pools.

## Additional Configuration

For optimal development, use Vite's React plugins:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc)

### Documentation

- [React Documentation](https://reactjs.org/docs/getting-started.html)
- [AWS Amplify Documentation](https://docs.amplify.aws/)
- [Vite Documentation](https://vitejs.dev/guide/)
- [AWS Amplify GitHub](https://github.com/aws-amplify/amplify-js)

## Important Notes

- Ensure you have the necessary AWS permissions to access and manage Amplify and related services.
- Regularly monitor your AWS resources to prevent unexpected costs.

---

