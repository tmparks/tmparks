# Git Configuration

    # Ensure that every commit on the main branch represents stable code
	[branch "main"]
	    mergeOptions = --no-ff

	# Hide the multitude of sins from topic branches
    [branch "develop"]
	    mergeOptions = --squash

	# Often (or rarely) used commands
    [alias]
	    alias = config --get-regexp ^alias\\.
	    graph = log --graph --oneline
	    unstage = reset HEAD --
		revert-commit = reset HEAD~ --
		delete-local-branch = branch --delete
		delete-remote-branch = push origin --delete
