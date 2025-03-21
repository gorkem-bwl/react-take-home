# React Coding Assignemnt

## Getting Started

1. Fork the repository and clone it to your local machine.
2. CD to `client` directory and run `npm install`
3. Run `npm run dev` to start the development server.
4. CD to the `server` directory and run `npm install`
5. Run `npm run dev` to start the server. It listens on port 9800 by default.
6. Open the browser and navigate to `http://localhost:5173` to see the Client.
7. Complete the assignment.

## Assignment Instructions

### Frontend 

Your goal is to build a fully interactive, reusable, and modular component that displays data fetched from a server with added functionalities.

1. Data Fetching & Error Handling
- Fetch data from the backend API and handle loading, error states, and retries.

2. Multiple Display Modes 
- Implement two variants: horizontal and vertical display modes.
- Add a toggle button to switch between the display modes dynamically.

3. Sorting & Filtering 
- Allow sorting by at least one column (e.g., alphabetically or numerically).
- Provide a basic filtering feature that lets users search within the displayed data.

4. Pagination 
- If the fetched dataset is large, paginate results with a “Next” and “Previous” button.
- Allow setting page size (e.g., 5, 10, 20 items per page).

5. Testing
- Write unit tests for at least one React hook and one core function in the component using Jest and React Testing Library.

Your goal is to write a reusable, modular component that displays some data that is fetched from a server.

This `DisplayComponent` should have two variants, one that displays data horizontally, one that displays data vertically. How you display the data is entirely up to you.

Please follow React best practices, use hooks where it makes sense, handle errors gracefully, comment liberally, etc. Commits are free so commit early and often!


### DevOps/CI-CD 

In addition to developing the React component, you'll implement a simple CI/CD pipeline to automate testing and deployment.

Requirements:
1. Set Up a GitHub Actions Workflow
- Create a .github/workflows/ci.yml file in the repository.
- The workflow should: 1. Install dependencies for both client/ and server/, 2. Run linting and unit tests for both frontend and backend, and 3. Build the frontend and backend if tests pass.

2. Dockerize the Application

- Write a Dockerfile for both the frontend and backend.
- Create a docker-compose.yml file that runs both services together.

3. Deploy to a Cloud Platform

- Configure a GitHub Actions workflow to deploy the application to a cloud service of your choice (Vercel, Netlify, Render, or a free-tier AWS/Azure instance).
- Alternatively, deploy the app on a personal VPS using Docker Compose.

4. Provide Documentation

- In the README.md, add a section explaining how to: 1. Run the application locally with Docker and 2. Deploy using the GitHub Actions workflow.
