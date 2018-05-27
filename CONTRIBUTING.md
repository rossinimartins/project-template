Everybody is welcome to make pull requests and open issues in this project, once following the rules available in this file.

# Issues

1. First, make sure that there isn't already an open issue which address the same problem. If there is one, give it a "[+1 reaction](https://github.com/blog/2119-add-reactions-to-pull-requests-issues-and-comments)" or a comment, if you believe that you have more information that can help us to solve the problem. 
2. After analysis, the issue will be classified as:
    - `INVALID`: the issue doesn't follow the rules available in this file.
    - `DUPLICATE`: there is another open issue who address the same problem.
    - `NOT A BUG`: the issue doesn't address a real bug, but relates the software working in a way it was designed to.
    - `NOT REPRODUCIBLE`: the developers cannot reproduce the problem described by the issue.
    - `WONT'T FIX`: the benefits on solving this issue are too small compared to the amount of work (or any other resource) required to do it.
    - `LOW PRIORITY`: there is no prediction of when this issue will be solved.
    - `MEDIUM PRIORITY`: this issue should be solved in one of the next releases.
    - `HIGH PRIORITY`: this issue should be solved ASAP.
3. If there is a need for more information, this will be solicited in the issue report. If the author of the issue doesn't answer in 7 days, the issue will be automatically closed;  
4. Once selected for the next release, the issue can be in one of the following status:
    - `RELEASE BACKLOG`: issue selected for the next release, but the work is not started yet.
    - `IN DEVELOPMENT`: there is a developer working on this issue.
    - `IN TEST`: the solution for the issue is beeing tested.
    - `READY FOR RELEASE`: the issue is solved and waiting for the next release.
    - `RELEASED`: the issue is solved and available in the current version of the software.

# Pull Requests

1. First, open an [issue](#issues) and assign it to yourself, to make sure there is no two people working on the same problem.
2. Then, create a new branch from the `develop` branch called `feature/{issue_code}` (without the curly brackets).
3. Write the tests and the corresponding code on the new branch. Make sure your commits messages follows the [convention](#commits). 
4. Push your branch and open a "squash merging" pull request to `develop`. Note that the pull request cannot be accepted under the following circumstances:
    - The source code submitted doesn't follow one of the coding conventions;
    - The message of one commit in the pull request doesn't follow the [convention](#commits);
    - The build fails on the CI server;
    - At least one of the tests fails;
    - Code coverage drops below 80%;
5. The pull request will be revised. Some comments can be added to it in way to improve the quality of the solution. On the other hand, if everything seems ok, the pull request will be accepted.

# Commits

This project uses [Conventional Commits messages](https://conventionalcommits.org/) with the following commit types:

* **meta**: SCM-only related changes, like adding a new file to `.gitignore`
* **docs**: Documentation only changes
* **observability**: Changes related to logs, metrics, monitoring, et cetera
* **hypothesis**: Commit used only for hypothesis testing
* **test**: Adding missing tests or correcting existing tests
* **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
* **refactor**: A code change that improves maintainability without changing external behavior
* **fix**: A bug fix
* **feat**: A new feature
* **arch**: High level changes in the project
* **lib**: Including or updating a third-party library
* **build**: Changes in the build-related files
* **infra**: Changes in configuration for third-party systems, like Docker images or CI tools
* **legal**: Changes related to licenses, copyright claims, et cetera
* **financial**: Changes related to funding or expenses of the project
