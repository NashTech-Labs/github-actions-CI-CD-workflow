# GitHub Actions CI/CD Template for Python Application

This repository contains a generic GitHub Actions CI/CD template for a Python application. It includes continuous integration (CI) and continuous deployment (CD) workflows.

## Usage

1. **Clone the repository**:
    ```bash
    git clone https://github.com/NashTech-Labs/github-actions-CI-CD-workflow.git
    ```

2. **Update the workflows**:

   - **CI Workflow (`.github/workflows/ci.yaml`)**: Customize the CI workflow as needed. Ensure that the Python version, dependencies, and test commands match your application.

   - **CD Workflow (`.github/workflows/cd.yaml`)**: Customize the CD workflow with your deployment platform. For AWS Elastic Beanstalk, set the `application-name`, `environment-name`, `region`, and `deployment-package` to match your setup. Update the deployment platform and configurations as needed.

3. **Add secrets**:

   - For CD workflow, add the necessary secrets (e.g., `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY`) to your GitHub repository.

4. **Push your changes**:
    ```bash
    git add .
    git commit -m "Update workflows"
    git push origin main
    ```

5. **Monitor the workflows**:

   - Monitor the CI/CD workflows in the GitHub Actions tab of your repository to ensure successful execution.
