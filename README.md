### Error : To push, remove secret from commit(s) or follow this URL to allow the secret.

### If the secret was already committed, you need to remove it from the Git history.

```python
git rm --cached .env
git commit --amend -CHEAD
```

### Install BFG Repo-Cleaner:

```python
brew install bfg
```

### Run BFG to clean the .env file:

```python
bfg --delete-files .env
```

### Force push the cleaned repository:

```python
git push --force
```
