# Bisect's VSTS CI Runners

We've adapted Microsoft's runners on linux platforms.

## Linux (ubuntu 16.04)

- [Conan](https://conan.io) installed.
- [Ninja](https://ninja-build.org) installed.
- GCC updated to version 7.
- Conan remotes [added](https://github.com/bisect-pt/conan_config).

## Windows
Not yet available.

# How to Use

1. Go to linux folder
2. Edit `docker-compose.yml` file:
    1. Change `YOUR_ACCONT_HERE` to your account name (Hint: look at your VSTS url. Example: https://<account_name>.visualstudio.com/)
    2. Change `YOUR_TOKEN_HERE` to a real access token ([HowTo](https://docs.microsoft.com/en-us/vsts/git/_shared/personal-access-tokens?view=vsts)).
3. Start the agent with `docker-compose up --build`!
