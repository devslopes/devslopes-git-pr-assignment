# Git 102 Assignment

## 📣 Getting Started

1. clone the repository: `git clone https://github.com/devslopes/devslopes-git-pr-assignment`
2. Create a `.gitignore` file
3. Create a `.env.local` file and copy/paste the following into it:

```
**DUMMY DATA**

CONVERTKIT_API_URL=https://api.convertkit.com/v3/
CONVERTKIT_API_KEY=D4SkateFzVBORyLK98DIE4321
CONVERTKIT_API_SECRET_KEY=123lY2sshhh-456NoXOne7fvH6i2-knowesJ0

FORM_ID=1234567

CONTENTFUL_SPACE_ID=d3-space-crocodiles
CONTENTFUL_ACCESS_TOKEN=givejkW9NU_xGGTZxME-xUXTHE-XMgg711codesj4pN
```

## 🛠 Requirements

1. Your commits and Pull Request **MUST EXCLUDE** OS generated files/folders and files with sensitive data. (i.e: OS-specific and editor specific settings, debug logs, build tools, etc).

## 📝 Instructions

1. Update the `.gitignore` file to ignore OS generated files/folders and files with sensitive data
2. Add and commit your changes
3. As you make changes to this project, be mindful of the requirements **(Requirements state the Pulll Request MUST EXCLUDE files with sensitive data)**.
4. Create a remote repository for this project on Github
5. Push this repository from the command line to Github.
   **NOTE:**: When adding this repository to Github, you will need to replace the word `origin` with `destination` (or any other word you wish to use). This is because the remote repository you cloned is already using the name, `origin`

```
git remote add destination <your_github_repo_url>
git branch -M main
git push -u destination main
```

6. After making your initial push to your remote repository, create a new branch off your local `main` branch called, `feature/bug-tracking`
7. Create a new file, `.env.production.local`
8. Copy/paste the following sensitive data into, `.env.production.local`:
   `SENTRY_DSN=https://1eb0a2142.ingest.sentry.io/711007`
9. Create a new file, `app.js`
10. Add the following to `app.js`:

```
var loveToCode = true;
var BUG_TRACKING_DNS = process.env.production.local;
```

11. Add the following to `styles.css`:

```
h2 { color: blue; }
```
12. It's a good practice to check the changes in your project before adding them to the staging area. You want to make sure you are only tracking the files you intend to.
13. Commit your changes locally. Your commit message should have a subject line and body. It should follow the 7 commit message convention guidelines
14. Push this branch to your remote repository. (This will create a new remote branch). Remember, when you push your code, don't use "origin". Use `destination` (or the whatever word you chose to use when you set up the remote repo)
15. Create a Pull Request for this branch to be merged into `main`
16. To submit your assignment, put the URL of your GitHub repository in a `.txt` file, zip the file and then upload it through your student portal so we can verify the commit history is correct. DO NOT MERGE YOUR PR UNTIL IT'S BEEN APPROVED. A Devslopes mentor will review your PR (Pull Request), comment as necessary and reject or approve your PR


## Notes:
1. If you realize your PR includes files it's not supposed to, you can delete your local and remote repository and start over.
