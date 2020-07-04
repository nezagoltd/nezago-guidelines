# Commit message template

A good commit message has three parts:
    1. Message title
    1. Message body
    1. Message footer

The message title starts by type of the task {feat, bug, chore} followed by colon and then a brief description of what changed in that commit, no more than 50 characters, the description must start with a capital letter, and use imperative model. No past, no future, just present tense as imperative model sounds.

You will describe all of changes you made in that commit in the body outlined as tasks, every task is started by a dash and a capital letter. Every task is in imperative mood. Remember that commit is like a small letter that you are communicating to other programmers, so that if they read it, they will undestand what you did in that commit, so try to express well what you have done. Don't hesitate to use techinal terms in it. Since it a message to other programmers, they understand what you want them to know.

The commit message footer, must be inside square bracket, and starts with {Finishes, Delivers}, followed by hash (#) followed by pivotal tracker ID

Note: The head is separated from the body with an empty space, and the body separated from the footer with empty space

## Example of the commit message
feat: User signup

- Write signup failing test
- Add signup controller
- Add signup endpoint

[Finishes#1111111]
