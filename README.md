This script lists the users who have read access to a specified GitHub repository by querying the GitHub API.

# Requirements
- Git Bash for Windows.
- jq: Command-line JSON processor for parsing API responses
- GitHub Personal Access Token with necessary scopes to read the repository's collaborator information

# How it Works
The script takes two arguments:

1. The GitHub user or organization name who owns the repository.
2. The repository name to query the collaborators from.

It will then authenticate using the provided GitHub username and Personal Access Token, make a request to the GitHub API, and list all users who have read (pull) access to the repository.

## Usage

1. Clone or download this script to your machine.

2. Set the Required Environment Variables
- username: Your GitHub username.
- token: Your GitHub personal access token.

You can set these variables in the terminal session:
export username="your-github-username"
export token="your-github-token"


3. Run the script with the required arguments: ./list-github-collaborators.sh <repo_owner> <repo_name>
- repo_owner: The username or organization name that owns the GitHub repository.
- repo_name: The name of the GitHub repository you want to query.


# Prerequisites
- jq: To parse and filter JSON data.
Install jq (if not already installed): sudo apt-get install jq


# Error Handling
If the required command-line arguments are not provided, the script will prompt you to enter the correct arguments. 
For example: Please execute the script with the required arguments (user and repo name).



# Author: Ankit Singh

# License: This script is open-sourced and free to use.