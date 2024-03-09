# Ask Magic 8 Ball Workflow

The **Ask Magic 8 Ball** workflow automates interactions with pull requests (PRs) based on the commit messages that contain a special trigger `/magic8ball`. This GitHub Action is designed to randomly interact with PRs when triggered.

## How It Works

Whenever a commit is pushed to any branch and the commit message includes `/magic8ball`, the workflow is triggered. For each PR that is impacted by the push, the workflow will randomly choose one of the following actions to take:

- Close the PR with a message indicating the decision (e.g., "Not a chance! ❌")
- Merge the PR with a positive message (e.g., "Definitely go for it! 🎉")
- Leave a neutral comment indicating indecision (e.g., "Can't predict now, try later! 🤔")
- Request a review from another collaborator (e.g., "Let's get some eyes on this! 👀")

## Steps to Use

1. **Trigger the Workflow:** Include `/magic8ball` in the commit message of a push to trigger the workflow.

## Key Features

- **Engagement and Fun:** Adds an element of surprise to the PR review process.

## Configuration

Ensure you have the GitHub Actions permissions configured to allow repository interactions such as closing, merging, and commenting on PRs.
