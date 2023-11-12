## Welcome to GitHub Collaboration Guide Instructions!

1. [Intro](#1-intro)
2. [Workflow for Individual Developers](#2-workflow-for-individual-developers)
   - [Fork the Repository](#21-forking-repositories)
   - [Clone Your Fork](#22-cloning-your-fork)
   - [Keep Your Fork Updated](#23-keeping-your-fork-updated)
   - [Create a Pull Request](#24-creating-a-pull-request)
3. [Workflow for Core Developers](#3-workflow-for-core-developers)
   - [Work with Branches](#31-working-with-branches)
   - [Create a Pull Request](#32-creating-a-pull-request)
4. [Workflow for Lead Developers](#4-workflow-for-lead-developers)
    - [Create Issues](#41-creating-issues)
    - [Review Pull Requests](#42-reviewing-pull-requests)
    - [Merge Pull Requests](#43-merging-pull-requests)
    - [Close Issues](#44-closing-issues)
5. [Outro](#5-outro)

### 1. Intro

Welcome to the team! We're excited to have you on board. This document will guide you through the setup process for working with GitHub in our organization. Depending on your role, you'll fall into one of these groups: "Individual Developers", "Core Developers" or "Lead Developers." Please follow the instructions relevant to your role.

### 2. Workflow for Individual Developers:
#### 2.1. Forking Repositories:
1. Navigate to the organization's GitHub page.

2. Find the repository you want to contribute to and click on it.

3. In the top right corner of the repository page, click the "Fork" button. This will create a copy of the repository in your GitHub account.

#### 2.2. Cloning Your Fork:
1. On your forked repository page, click the "Code" button, and copy the URL.

2. Open your terminal or command prompt and navigate to the directory where you want to store the project.

3. Run the following command to clone the repository to your local machine:

    ```bash
    git clone https://github.com/your-username/repository.git
    ```

#### 2.3. Keeping Your Fork Updated:
1. Add the original repository as a remote:

    ```bash
    git remote add upstream https://github.com/organization-name/repository.git
    ```
2. Fetch the latest changes from the original repository:

    ```bash
    git fetch upstream
    ```
3. Merge the changes into your local fork:

    ```bash
    git merge upstream/dev
    ```
4. Push the changes to your GitHub repository:

    ```bash
    git push origin dev
    ```

#### 2.4. Creating a Pull Request:

1. On your GitHub fork, navigate to the "Pull Requests" tab.

2. Click on the "New Pull Request" button.

3. Select the base repository (organization/repository) and the base branch (dev).

4. Select the head repository (your forked repository) and the compare branch (e.g., feature/your-feature-name).

5. Click on "Create Pull Request."

6. Add a title and description to explain your changes.

7. Request a review from relevant team members.

8. Apply appropriate labels to categorize your contribution, such as "feature," "bugfix," or other relevant labels.

9. Click on "Create Pull Request" again to submit your request.


### 3. Workflow for Core Developers:
#### 3.1. Working with Branches:

1. Clone the repository to your local machine (if not done already):

    ```bash
    git clone https://github.com/organization-name/repository.git
    ```

2. Navigate to the project directory:

    ```bash
    cd repository
    ```

3. Create a new branch for your feature or bug fix:
    - For features:

        ```bash
        git checkout -b feature/your-feature-name
        ```
    - For bug fixes:

        ```bash
        git checkout -b bugfix/your-bugfix-name
        ```
4. Make your changes and commit them:

    ```bash
    git add .
    git commit -m "Your commit message"
    ```

5. Push the branch to GitHub:
    ```bash
    git push origin feature/your-feature-name  # or bugfix/your-bugfix-name
    ```
#### 3.2. Creating a Pull Request:

1. On your GitHub repository, navigate to the "Pull Requests" tab.

2. Click on the "New Pull Request" button.

3. Select the base repository (organization/repository) and the base branch (dev).

4. Select the head repository (your forked repository) and the compare branch (e.g., feature/your-feature-name).

5. Click on "Create Pull Request."

6. Add a title and description to explain your changes.

7. Request a review from relevant team members.

8. Apply appropriate labels to categorize your contribution, such as "feature," "bugfix," or other relevant labels.

9. Click on "Create Pull Request" again to submit your request.

10. In the pull request description, link the related issue using the # symbol and issue number (e.g., #123). This helps in cross-referencing and provides context for the changes.

Congratulations! Your changes will be merged into the dev branch after the review process. If you have any questions or concerns, feel free to communicate with your team lead or colleagues. Happy hacking!

### 4. Workflow for Lead Developers
#### 4.1. Creating Issues

1. On the GitHub repository page, click the "Issues" tab.

2. Click the "New Issue" button.

3. Provide a clear title and description for the issue.

4. Assign labels, milestones, and assignees as needed.

#### 4.2. Reviewing Pull Requests

1. Navigate to the "Pull Requests" tab on GitHub.

2. Review code changes in the pull request.

3. Add comments, request changes, or approve the pull request.

#### 4.3. Merging Pull Requests

1. Ensure the pull request has been reviewed and approved.

2. Click the "Merge" button on the pull request page.

3. Choose the merge method (e.g., "Merge commit" or "Squash and merge").

**Notice**: All changes must be merged into the development branch. Then you should periodically, synchronize the development branch by merging it into the main branch to maintain the latest features and fixes.

#### 4.4. Closing Issues

1. Once the changes are merged, close the related issue.

2. Add any necessary comments or details regarding the resolution.

### 5. Outro
Thank you for taking the time to familiarize yourself with our collaboration guide. We wish you the best in your work and hope for great results! If you have any questions, feel free to reach out to your team or fellow developers.