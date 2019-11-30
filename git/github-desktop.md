# About Github-Desktop

1. >Error: Commit failed -exit code 128 received, with output: '*** Please tell me who you are'.

    fix: open [your git folder]/.git/config, add:

    ```bash
    ...
    [user]
    name = your github name
    email = your github email  
    ...
    ```
