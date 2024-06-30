# GitHub Account Statistics Service

Track and analyze your GitHub activities with ease. This service provides detailed insights into your GitHub account, including repository statistics, follower counts, stars, and contributions. You can also compare your performance with other GitHub users.

## Table of Contents
- [Features](#features)
- [How It Works](#how-it-works)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Data Model](#data-model)
- [User Stories](#user-stories)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

## Features

- **User Authentication with GitHub:** Securely log in using your GitHub account.
- **Detailed Statistics:** View comprehensive statistics of your repositories, followers, stars, and contributions.
- **Comparison Tool:** Compare your GitHub performance with other users.
- **Interactive Visualizations:** Enjoy interactive charts and graphs for data analysis.

## How It Works

1. **Sign Up:** Log in with your GitHub account to get started.
2. **Fetch Data:** Our system retrieves your GitHub statistics instantly.
3. **Analyze & Compare:** View your data and compare it with others to gain insights.

## Installation

To set up the project locally, follow these steps:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/Obrempong12/Portfolio_Project.git
    ```

2. **Navigate to the project directory:**
    ```bash
    cd Portfolio_Project
    ```

3. **Install dependencies:**
    ```bash
    npm install
    ```

4. **Set up environment variables:** Create a `.env` file and add your GitHub OAuth credentials.
    ```env
    GITHUB_CLIENT_ID=your_client_id
    GITHUB_CLIENT_SECRET=your_client_secret
    ```

5. **Run the project:**
    ```bash
    npm start
    ```

## Usage

1. **Log in:** Use your GitHub account to log in.
2. **View statistics:** Access your personalized dashboard to view detailed statistics.
3. **Compare with others:** Use the comparison tool to analyze your performance against other GitHub users.

## API Endpoints

### Authentication
- **`GET /auth/github`**: Redirects to GitHub for authentication.
- **`GET /auth/github/callback`**: Callback URL for GitHub authentication.

### User Data
- **`GET /api/user`**: Retrieves authenticated user data.
- **`GET /api/user/repos`**: Retrieves user repository data.
- **`GET /api/user/compare/:username`**: Compares authenticated user data with another GitHub user.

## Data Model

The data is stored in the following format:

- **User:**
  ```json
  {
    "id": "unique_user_id",
    "username": "github_username",
    "avatar_url": "profile_image_url",
    "repositories": [
      {
        "id": "repo_id",
        "name": "repo_name",
        "stars": "star_count",
        "forks": "fork_count",
        "issues": "issue_count"
      },
      ...
    ]
  }
---
## Contributors
PETER KWESI OBREMPONG STEPHENSON<https://github.com/Obrempong12>
