# Claiming Multiple Bounties: Multi-Bounty PRs

> **Note:**  
> If you need to include an image, place it in the curly brackets below as a Markdown image link.  
> Example:  
> `{ ![Multi-bounty PR example](path/to/image.png) }`  
> The image should visually show a PR description with multiple `close #issue-number` lines, or a workflow diagram illustrating the process of claiming multiple bounties.

---

## What Does "Multi-bounty PRs Must Claim Each Reward Separately" Mean?

When you work on a project with Lightning Bounties, you might solve more than one bounty issue at the same time.  
A **multi-bounty PR** is a pull request (PR) that addresses multiple issues, each with its own bounty attached.

**You must claim each bounty reward separately.**  
This means:  
- You cannot claim multiple bounties with a single PR description alone.
- Each bounty issue must be closed and claimed in a way the system can recognize and reward.

---

## Why Is This Important?

Lightning Bounties uses GitHub’s automation.  
When you add `close #issue-number` (or `closes #issue-number`) in a PR description, it triggers the bounty payout for that specific issue.

If you solve multiple bounty issues, the system needs a clear, separate closure for each one to process all rewards correctly.

---

## How To Claim Multiple Bounties

### 🟢 **Recommended: One PR Per Bounty Issue**

1. **Create a separate PR for each bounty issue you solve.**
2. In each PR description, include `close #X`, where `X` is the issue number for the bounty you are claiming.
3. Merge each PR after review.

**This is the simplest, most reliable way to ensure you get all your bounty rewards.**

---

### 🟡 **If You Combine Fixes in One PR (Not Recommended)**

If you must address multiple issues in a single PR:

1. Merge the combined PR as usual.
2. For each additional bounty issue:
    - Create a minimal follow-up PR (for example, update a comment or documentation).
    - In the PR description, include `close #X` for the remaining issue, and reference the original PR.
    - Example:
      ```
      close #42

      This PR references the work completed in #123 (original PR).
      ```
3. Merge each follow-up PR to trigger the bounty payout for each issue.

---

## Why Separate Claims?

- Lightning Bounties tracks and pays out rewards based on the closure of individual issues via PRs.
- If you do not claim each bounty separately, you may miss out on some rewards.
- The system may only process the first `close #X` it finds in a PR description.

---

## Example Workflow

| Step                      | Action                                                                 |
|---------------------------|------------------------------------------------------------------------|
| 1. Solve multiple issues  | Fix code for issues #10 and #12, each with a bounty.                   |
| 2. Create PR for #10      | PR description: `close #10`                                            |
| 3. Create PR for #12      | PR description: `close #12`                                            |
| 4. Both PRs merged        | Each bounty is automatically recognized and paid out by the system.    |

If you accidentally merged a PR that fixed multiple issues but only closed one bounty,  
create a new minimal PR for each remaining bounty, referencing the original PR as the source of the fix.

---

## 🧠 Expert Tips

- Keeping PRs atomic (one per issue) helps with clarity, review, and automation.
- If you’re ever unsure, default to one PR per bounty issue.
- Always use the `close #issue-number` syntax in the PR description, not just in comments.

---

## Summary

- **Always claim each bounty separately.**
- **Use one PR per bounty issue whenever possible.**
- **If you combine fixes, follow up with minimal PRs to close and claim each remaining bounty.**
- **Use `close #issue-number` in each PR description to trigger the payout.**

---

{  
  // Place an image here showing a PR description with multiple `close #issue-number` lines,  
  // or a workflow diagram illustrating the process of claiming multiple bounties.  
  // Example: ![Multi-bounty PR example](path/to/image.png)
}
