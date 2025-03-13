# UI Component Library with Code Quality Checks

This project extends the UI component library from Assignment 12 by adding code quality checks and automated testing.

## Setup Instructions

### Prerequisites

- Node.js (v16 or higher)
- npm (v7 or higher)
- Docker

### Development Setup

1. Clone the repository:
   \`\`\`
   git clone [your-repository-url]
   cd zhu_haiqiao_ui_garden_build_checks
   \`\`\`

2. Install dependencies:
   \`\`\`
   npm install
   \`\`\`

3. Run development server:
   \`\`\`
   npm start
   \`\`\`

4. Run Storybook:
   \`\`\`
   npm run storybook
   \`\`\`

5. Run tests:
   \`\`\`
   npm test
   \`\`\`

### Code Quality Tools

This project uses the following code quality tools:

- ESLint for code linting
- Prettier for code formatting
- Husky for Git hooks
- lint-staged for running linters on staged files

Pre-commit hooks automatically run to ensure code quality before committing:

- Prettier formats code
- ESLint checks for issues
- Tests run to verify functionality

### CI/CD Pipeline

GitHub Actions are configured to run the same checks on every push and pull request to ensure code quality is maintained even if local pre-commit hooks are bypassed.

### Docker Setup

To run the application in a Docker container:

1. Build the Docker image:
   \`\`\`
   docker build -t zhu_haiqiao_coding_assignment13 .
   \`\`\`

2. Run the Docker container:
   \`\`\`
   docker run -p 8018:8018 --name zhu_haiqiao_coding_assignment13 zhu_haiqiao_coding_assignment13
   \`\`\`

3. Access the application at [http://localhost:8018](http://localhost:8018)
