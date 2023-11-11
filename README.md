## Welcome to GitHub Collaboration Guide Instructions!

1. [Intro](#intro)
2. [Workflow for Outside Developers](#workflow-for-outside-developers)
   - [Fork the Repository](#fork-the-repository)
   - [Clone Your Fork](#clone-your-fork)
   - [Keep Your Fork Updated](#keep-your-fork-updated)
   - [Create a Pull Request](#create-a-pull-request)
3. [Workflow for Core Developers](#workflow-for-core-developers)
   - [Create a Branch](#create-a-branch)
   - [Make Changes](#make-changes)
   - [Push Changes](#push-changes)
   - [Create a Pull Request](#create-a-pull-request-1)

### 1. Intro

Welcome to the team! We're excited to have you on board. This document will guide you through the setup process for working with GitHub in our organization. Depending on your role, you'll fall into one of two groups: "Outside Developers" or "Core Developers." Please follow the instructions relevant to your role.

### 2. Guide for Outside Developers:
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


### 3. Guide for Core Developers:
#### 3.1. Creating Branches:

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

#### 3.3. Reviewing and Merging:

1. Team members will review your pull request, suggest changes, and discuss the proposed changes.

2. Once the changes are approved, the reviewer can merge the pull request.

3. To merge, click on the "Merge" button, ensuring that the "Squash and Merge" option is selected if needed.

4. Confirm the merge.

Congratulations! Your changes will be merged into the dev branch after the review process. If you have any questions or concerns, feel free to communicate with your team lead or colleagues. Happy hacking!