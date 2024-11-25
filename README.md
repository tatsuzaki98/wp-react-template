# WordPress Local Development Environment
Start WordPress server

```sh
# Copy .env.example to .env
install .env.example .env

# Start WordPress server
docker-compose up
```

Enable Tailwind hot reload
Tailwind output file is `/greenleaf/global.css`.

```sh
# Install npm packages
npm ci

# Start Tailwind hot reload
npm run watch
```

# to-do
- check how to enable custom fields in the Gutenberg editor

# Branch Protection Rules
To ensure the integrity of the repository and maintain high code quality, we implement the following Branch Protection Rules for key branches like main:

### Require Pull Request Reviews:

- At least 1-2 reviews must be approved by the Project manager and/or the Lead developer before merging.

- Reviewers should be familiar with the impacted area of code.
  
- Each developer/team member should create pull requests after different commits which will be reviewed by the Project manager or Lead developer before merging to restricted branches.

### Status Checks:

- All required status checks like particular tests must pass before merging.

- Enable the option to Require status checks to pass before merging.

### Commit History:

- Disable force pushes to protected branches to prevent history rewrites.

- Require linear history to maintain a clean and straightforward commit history.

### Branch Restrictions:

- Limit who can push directly to protected branches, ensuring that only authorized personnel can make changes.

- In this case only the Lead Developer and the Project Manager are authorized to make changes in the main branch.

### Branch Naming Conventions

To ensure consistency and clarity, please follow these branch naming conventions:

- **Feature Branches**: `feature/<short-description>`  
  Example: `feature/user-authentication`

- **Bugfix Branches**: `bugfix/<short-description>`  
  Example: `bugfix/fix-login-error`

- **Hotfix Branches**: `hotfix/<short-description>`  
  Example: `hotfix/fix-typo-in-readme`

- **Release Branches**: `release/<version-number>`  
  Example: `release/v1.0`

## Commit Message Format
#### Commit messages should follow this format:

Type: A short type of change (e.g., feat, fix, docs, chore, style, refactor, test)

Description: A concise but clear message describing the change.

# Issue Creation Guidelines
To ensure efficient issue tracking and resolution, follow these guidelines when creating new issues:

### Use Templates:

- Always use the provided issue templates for consistency.

- If no template fits, provide a clear and concise description.

### Descriptive Titles:

- Use a specific, clear and concise title that summarizes the issue clearly.

### Detailed Descriptions:

Include the following information:

- Steps to Reproduce if the issue is a bug
- Expected Behavior
- Actual Behavior
- Any relevant screenshots, error logs, or examples.

### Labels:

- Apply relevant labels as specified by github to categorize the issue.

### Link Relevant Resources:

- Reference related issues, pull requests, or any helpful documentation where necessary.

### Assignment:

- Assign the issue to yourself or a relevant team member to handle the issue.
