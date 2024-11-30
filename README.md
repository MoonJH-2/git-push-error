If the secret was already committed, you need to remove it from the Git history.
git rm --cached .env
git commit --amend -CHEAD

Install BFG Repo-Cleaner:
brew install bfg

Run BFG to clean the .env file:
bfg --delete-files .env

Force push the cleaned repository:
git push --force
