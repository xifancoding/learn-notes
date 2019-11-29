Bug: 
    Error: Commit failed -exit code 128 received, with output: '*** Please tell me who you are'.

Fix: 
    open [your git folder]/.git/config
    append:
    [user]
	    name = your github name
	    email = your github email

