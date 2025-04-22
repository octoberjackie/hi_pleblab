# ClaimRewardv2 Criteria and Troubleshooting Guide for Lightning Bounties

## Introduction

This guide outlines the criteria for claiming rewards and provides troubleshooting steps for developers working on bounties on the Lightning Bounties Platform. 

## ClaimRewardv2 Criteria

To claim a reward for a bounty:

1. **Look for an Issue**: Find an issue on the  [app.lightningbounties.com](http://app.lightningbounties.com "app.lightningbounties.com"). feed that you want to work on.

2. **Fix the Issue**: Fork the repository, work on the issue, and ensure your changes meet the acceptance criteria.

3. **Create a Pull Request (PR)**:
   - Create a PR to the bounty poster's repository.
   - In the PR description, include the `close #issue-number` syntax to link the PR to the issue.

4. **Claim Reward**: 
   - **Important**: Before claiming the reward, you must click **Claim Reward** on  [app.lightningbounties.com](http://app.lightningbounties.com "app.lightningbounties.com").
   - Once the PR is approved and merged, and you maunually click `claim reward` + `check` the reward will be deposited directly into your balance.

## Troubleshooting

### Issue Not Linked to PR

- **Check PR Description**: Ensure the `close #issue-number` syntax is present in the PR description.
- **Ask for Help**: If you cannot edit the PR, ask the repository owner to add the `close` syntax for you.

### PR Merged but No Payment

- **Verify PR Description**: Confirm the `close #issue-number` syntax is in the PR description.
- **Create a New PR**: If the syntax was missing, create a new PR with minimal changes (e.g., a comment or documentation update) and include the `close #issue-number` syntax.
  - Go to the repository on GitHub.
  - Click "Compare & pull request".
  - Include `close #X` or `closes #X` in the PR description (where X is your issue number).
  - Explain that this PR is to properly close the issue for Lightning Bounty payment.
  - Reference your original PR: "This PR references the work completed in #Y".
  - The repository owner will need to review and approve this new PR.

### Payment Not Received

- **Check User Balance**: Ensure your account balance is updated on  [app.lightningbounties.com](http://app.lightningbounties.com "app.lightningbounties.com").
- **Contact Support**: If the balance is not updated, reach out to the Lightning Bounties  [Discord](https://discord.gg/zBxj4x4Cbq "Discord") for assistance.

### Other Issues
- **Lightning Network**: Ensure your Lightning Network wallet is set up correctly for receiving payments.

---

By following these steps and troubleshooting tips, developers can effectively claim rewards for their contributions. Remember, to claim the bounty, you must first click **Claim Reward** on [app.lightningbounties.com](http://app.lightningbounties.com "app.lightningbounties.com").
