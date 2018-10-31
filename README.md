# SimpleRPackage

This R package was created for testing RStudio and git integration, as well other related packages.

Steps for create and deploy it in GitHub:

1. In RStudio: *Project -> Create New Project -> New Directory -> R Package*. Then, fill the informations about the package and check the box "Create a git repository" beore create it;
2. Change your package, add functions, documentation and build it, following: *Build -> Clean and Rebuild*;
3. Go to your GitHub account and create a new repository with the same name of your new package; 4. Open your terminal (inside RStudio) and:
   - If that is your first time using git, you will need to associate your GitHub account to the repository. Just change your e-mail and GitHub name by typing:
   ```
   git config --global user.email "your email associated to GitHub account"
   git config --global user.name "your GitHub user name"
   ```
   - Then, change the actual (empty) git origin to the one you created at GitHub:
   ```
   git remote add origin git remote add origin git@github.com:githubname/reponame.git
   ```
   - Finally, push the commited code to GitHub:
   ```
   git push -u origin master
   ```

After this procedure you should see the Pull and Push buttons at Git bar on RStudio and be able to do the next commits as usual. 

Related sources:
- [git-rstudio](http://r-pkgs.had.co.nz/git.html)
- [create-packages-r-cran-github](https://www.analyticsvidhya.com/blog/2017/03/create-packages-r-cran-github/)
- [rstudio-see-git](http://happygitwithr.com/rstudio-see-git.html)
- [rstudio-changing-origin-for-git-version-control-of-project](https://stackoverflow.com/questions/39435240/rstudio-changing-origin-for-git-version-control-of-project?rq=1)
