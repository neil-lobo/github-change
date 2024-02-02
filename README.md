# Installation

1. Clone repo
```sh
git clone git@github.com:neil-lobo/github-change.git
```

2. Make script executable
```sh
cd github-change/src
chmod u+x github-change
```

3. Add `github-change` to your `PATH` variable

4. Create `src/accounts.json` file
    - Follow `src/example.accounts.json` file

5. Optionally, turn on auto signing for commits
```sh
git config --global commit.gpgsign true
```

6. Add to `.bashrc` file or equivalent
```sh
eval "$(ssh-agent -s)" > /dev/null
github-change 2> /dev/null
```

7. Optionally, create an alias in `.bashrc` file or equivalent
```sh
alias ghc='github-change'
```

# Usage
### Show currently loaded account
```sh
github-change -s
```
### Switch accounts
```sh
github-change -c [account-name]
```
