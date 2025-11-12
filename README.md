# Mixed_model

Link to the [Quarto web page](https://nmar722.github.io/Mixed_model/)

## Quick Guide: Switch an Existing Repo from HTTPS to SSH

1. Check current remote URL:
```r
git remote -v
```
If you see something like:

origin  https://github.com/user/repo.git (fetch)

origin  https://github.com/user/repo.git (push)

2. Change remote to SSH:
```r
git remote set-url origin git@github.com:user/repo.git
```

3. Verify the change:
```r
git remote -v
```
It should now show:

origin  git@github.com:user/repo.git (fetch)

origin  git@github.com:user/repo.git (push)

## SSH vs HTTPS for GitHub Workflows (Summary Table)

Feature |SSH |HTTPS|
--- |--- |--- |
Authentication |SSH keys (no password prompts) |Username + PAT (or credential helper) |
Setup Complexity |Requires key generation & GitHub setup |Simple (just use credentials) |
Firewall Friendly |May be blocked (port 22) |Works everywhere (port 443) |
Best ForFrequent pushes, automation, private repos |Quick clones, restricted networks |
Security |Strong (key-based) |Strong (token-based) |
Credential Rotation |Rare (keys last long) |Tokens expire or need rotation|

