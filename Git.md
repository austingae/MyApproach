# Git

## When you want to use git in your project: 
1. git init
2. create a remote repository on GitHub
3. git remote add origin GitHub-link
4. have some code, then git add and git commit
5. git push origin master

## If you want to create a new feature, then use the Feature Branch Workflow:
1. create a feature branch, which is a copy of your git history | git branch branch-name
2. upload feature branch to GitHub | git push origin branch-name
3. git checkout branch-name; work on the feature; and when done...git add, git commit, and git push
4. create a "pull request" on GitHub so that others can view and comment on your code
5. Once approved, then merge feature branch to master branch.
- merge changed feature branch to unchanged master branch --> merge!
- merge changed feature branch to changed master branch --> might lead to merge conflict, which must then be resolved manually

### Sources: 
- https://www.youtube.com/watch?v=hrTQipWp6co&t=1852s&ab_channel=SuperSimpleDev
- https://www.youtube.com/watch?v=1ibmWyt8hfw&t=2557s&ab_channel=SuperSimpleDev
- https://www.youtube.com/watch?v=Q1kHG842HoI&ab_channel=SuperSimpleDev



# GitHub Pages:
How to Deploy a React App to GitHub Pages: https://www.youtube.com/watch?v=Q9n2mLqXFpU&list=LL&index=1&ab_channel=PedroTech

Once React App has been Deployed to GitHub Pages, How to Fix 404 Error: https://www.youtube.com/watch?v=fuGu-Ponjf8&ab_channel=ToThePointCode