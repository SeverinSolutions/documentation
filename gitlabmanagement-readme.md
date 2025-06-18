# B3 Production

## Description

The B3 Production server is a dynamic web application designed to enhance project management and issue tracking through real-time interactions. Leveraging the GitLab REST API and Webhooks, it offers an intuitive interface for viewing, commenting on, and updating the state of issues within your private GitLab repositories.

## Features

- GitLab OAuth2 integration for user authentication.
- Fetch and display projects and issues from GitLab.
- Real-time updates for issues using WebSockets.
- Issue management capabilities.

## Technologies

- Node.js and Express for the backend.
- EJS for templating.
- MongoDB for session storage.
- WebSocket for real-time communication.
- GitLab API for issue management.

## Prerequisites

- Node.js installed.
- GitLab account.
- MongoDB running locally or remotely.

## Environment Setup

Before running the application, ensure you have set up the following environment variables in a `.env` file:

- **GITLAB_PROJECT_ID**: The Client ID of your GitLab OAuth application.
- **GITLAB_PROJECT_SECRET**: The Client Secret of your GitLab OAuth application.
- **GITLAB_CALLBACK_URL**: The callback URL for OAuth flow, e.g. `https://yourdomain.com/auth/callback`. Must match one of the Redirect URIs in your GitLab applicatoin settings.
- **GITLAB_WEBHOOK_URL**: The URL for receiving webhook events from GitLab e.g. `https://yourdomain.com/webhook/issues`.

**Note**: You can set up the OAuth application on GitLab by navigating to `https://gitlab.lnu.se/oauth/applications/` to obtain the Client ID and Client Secret.


## Getting Started

To set up and run the B3 application, follow these steps. This assumes a server is already set up for its deployment, secured with your selected technologies. If not, ensure to set up and secure a server beforehand.

1. Clone the repository:
   ```bash
   git clone git@gitlab.lnu.se:1dv528/student/jl225ps/b3-production.git
   ```
2. Navigate to the project directory:
   ```bash
   cd b3-application
   ```
3. Install the dependencies (in production mode):
   ```bash
   npm install --production
   ```
4. To start the server use the following command:
   ```bash
   npm start
   ```
5. Access the application: Open your web browser and navigate to your domain name.

**Note**: The command in step 4 is the simplest way to start the server but may not be recommended for production environments. Adjust the command to fit your server configuration and setup requirements.
