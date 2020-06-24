# test-git-squash
This repo is for testing git squash command.

## Scenario 1
I just created my master branch and pushed a new commit.

Now let’s create a feature branch.

Created a new branch called “scenario1”.

Now I checked out my scenario 1 branch. This is to test if I have multiple local commits on a feature branch, but I don’t push them to the remote feature branch, when I squash them, do I need to force push?

    - Now I made two commits. Let’s squash them and see what happens
	- Now I have squashed my commits and pushed
		- I was not required to do force push.
	- Conclusion: if I don’t push my commits to remote feature branch, I can squash them and do normal push (not the force push). 
	- This is because the new two commits do not exist in the history of my remote feature branch yet, so it is easy to rewrite their histories.
	
## Scenario 2

When I have multiple local commits in my feature branch, and I push them, when I want to squash them, do I need to force push?

    - Yes, force push.
    - This is because the new commits have historis on the remote branch, and squashing them means overwrite the original histories.
    
## Scenario 3
When I have some commits, and master has some later, and I merge my local branch with master, can I squash commits?

    - Now I have merged master to my local branch. 


