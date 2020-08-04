# Nezago git bestpractices

As Git is the most popular version control system worldwide, we chose it to be our first version control system to use, but we are open to use any other one depending on the requirements of a specific project or client.

## Git namings

Since here at nezago, we believe that working as team will not only help us to go faster, but also it will help us to reach the peak possible, for that we want to go in harmony, with reliability, consitently. That is why we are concerned on how we name our things: repository, branch, pull request, ...

In this document, I am describing the naming convetions that we use here at nezago.

### Repository naming
While naming git repo, you should use lowercase letters, separted by dashes if your repository is a compound name.

Examples: 

1. Valid git repo name:
nezamedia-backed

2. Invalid repo names:
    * ~~Nezamedia-backend~~
    * ~~NEZAMEDIA-BACKEND~~
    * ~~nezaMedia-backend~~
    * ~~NezaMedia-Backend~~
    * ~~nezamedia_backend~~

#### What a valid repo name should and shouldn't have?
1. It should have a descriptive name, this means if I read a name of your git repo, I should have a big picture of what your repo has inside.

1. No general names allowed, like test, dev, project, ...

1. There shouldn't be any underscore, numbers, capital letters.

1. Your github repository name should not have more than 20 characters

1. It should be memorable, (Easy to be remembered)

### Branch naming
A branch name should be started by {ft, bg, ch} depending on the type of the task it implements, followed by a dash, followed by name of the branch in lowercases

 * ft : Feature
 * bg : bug fix
 * ch : chore

Examples: 

1. Valid branch name

    ft-user-signup

2. Invalid branch names
    * ~~user-signup~~
    * ~~ft-User-signup~~
    * ~~ft-user-Signup~~
    * ~~FT-USER-SIGNUP~~
    * ~~ft-user_signup~~

#### What a valid branch name should and shouldn't have?
1. It should have a descriptive name, this means if I read a name of your branch, I should understand which task are you are implementing on that branch.

1. No general names allowed, like test, dev, branch, ...

1. There shouldn't be any underscore, numbers, capital letters.

1. Your github branch name should not have more than 20 characters

1. It should be memorable, (Easy to be remembered)

### Pull request naming
We want you to name your pull request the title of the first commit message in that pull request.

Example:
feat: User signup

*Note:* Please read [this document](https://github.com/nezago/nezago-guidelines/wiki/Commit-message-template-used-at-nezago) on how you should formulate your commit messages, because if your commit message is invalid, then the name of your pull request will be invalid too.

#### What a valid pull request name should and shouldn't have?
1. It should have a descriptive name, this means if I read a name of your pull request, I should understand which task you are implementing in that pull request.

1. No general names allowed, like test, dev, branch, ...

1. There shouldn't be any underscore, numbers, dashes, hashes, ...

1. Your pull rquest name should not have more than 50 characters

1. It should be memorable, (Easy to be remembered)


## Other git conventions to use at nezago

### 1. Pull request
1. Whenever you get assigned a new task, and whenever you start working on that task, you must raise a pull request as soon as possible after your first commit.

1. If you are working on a task, from your solo project, which is for nezago controls, you are not allowed to merge your pull request before getting a review and at least one approval from Nezago Software Support Engineer (NSSE)

1. If you have raised a pull request, and you are still working on that pull request, you should add a badge to it, showing that is still in progress, when you are done and waiting for review, you have to remove the `work in progress` badge and add `ready for review` badge, and once it is approved, you have to remove the `ready for review` badge, and add `merge` badge

1. If you are working on a solo project, after getting your Pull Request approved, both you or NSSE, one of you, can merge the pull request to the base branch

1. If you are working on a pull request as a team, you should have a Technical Team Lead (TTL), which you will be provided by nezago, no team member is allowed to merge a PR, that is a task of TTL, for rebasing simplicity, we encourage teams to keep their PRs have one commit. You can use some techniques to achieve that, such as `git ammend --no-edit` or `git squash` but that is optional

1. In a team work project, a pull request will be ready for TTL review after getting two approvals from peer review

1. In a team work project, if your pull request is ready for peers review, you should send them review request by selecting them in your pull request reviewer section, remember that no team member is allowed to merge a pull request, that is a job of a TTL.

1. As a Technical Team Lead (TTL) of a team a certain team, you should make sure that your team members have tasks to work on, help them whenever they meet a blocker (technical or personal), maintain team harmony such as team convetions, folder structure, ..., review all `ready for TTL review` pull requests and approve and merge them if they deserve it.

### 2. Pull request badges
1. `work in progress` => in pink background color and white text
1. `ready for peer review` => in right blue background color and white text
1. `ready for TTL review` => in dark blue background color and white text
1. `merge` => in purple background color and white text
1. `rebase` => in yellow background color and black text

### 3. Commit
1. nezago strongly encourages you this: Whenever you are working on a task, make sure to commit and push your code on github, before: 

 * Shutting down your computer
 * Going to breakfast, brunch, lunch, supper, dinner
 * Taking a short break
 * Going to sleep

2. We strongly encourage you to keep practicing writing a good commit message which follows [this template](https://github.com/nezago/nezago-guidelines/wiki/Commit-message-template-used-at-nezago)

### 4. Project
1. A valid project at nezago, should have a professional readme file which is following our readme file template, get the template from [here](https://raw.githubusercontent.com/nezago/nezago-guidelines/development/nezago-templates/nezago-readme-file-template.md)

1. At least a link to documentation should be available for any project
