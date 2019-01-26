# fortress
Automation build system.

How it should work

1. Reads the .fortress.json JSON configuration file from the root directory of your repository.

2. Gets automated build execution command from it, for example bundle test.

3. Checks out your repository into a temporary directory on one of its servers.

4. Merges pull request into master branch.

5. Starts a new Docker container and runs bundle test in it.

6. If everything is fine, pushes modified master branch to GitHub.

7. Reports back to you, in the GitHub pull request.
