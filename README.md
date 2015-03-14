<pre> 
 ____            _           _     ____             _          
|  _ \ _ __ ___ (_) ___  ___| |_  |  _ \  ___ _ __ (_)___  ___ 
| |_) | '__/ _ \| |/ _ \/ __| __| | | | |/ _ \ '_ \| / __|/ _ \
|  __/| | | (_) | |  __/ (__| |_  | |_| |  __/ | | | \__ \  __/
|_|   |_|  \___// |\___|\___|\__| |____/ \___|_| |_|_|___/\___|
              |__/                                             
		
</pre>		


## Overview
ProjectD (Working Title) - Special gift for someone special.

## Dependencies

## Quick Start

    git clone https://Tykco@bitbucket.org/Tykco/projectd-web.git
    cd projectd-web
    cp config/database.yml.sample config/database.yml
    cp .env.sample .env
    bundle install
    rake db:setup
    rails s

## Deployment

    *to be confirmed*

## Testing

    guard

## Branching

This project is running on [GitHub Flow](https://guides.github.com/introduction/flow/) with a modified [Git Flow](http://nvie.com/posts/a-successful-git-branching-model/) workflow.

* `master` is the active development branch

All local development should be done in the appropriately named branches:

* `feature/<branch_name>` for substantial new features or functions
* `enhance/<branch_name>` for minor feature or function enhancement
* `bugfix/<branch_name>` for bug fixes

**WARNING: Do not merge your changes directly into your local master
branch and push to GitHub!!!**

If you are done developing the component you are working on, push your
branch to GitHub by doing:

`git push -u origin <branch_name>`

After that, visit the
[BitBucket repository page](//bitbucket.org/Tykco/projectd-web) and open a
pull request to the `master` branch.

**TIP: "head branch" is the branch you want to merge, "base branch" is
the branch you want to merge your new commits into.**

Give your pull request a title and describe what you are trying to
achieve with your code. The branch or release manager will review your
code and take the next appropriate actions.

**Even if you are working alone, it is a must to follow this GitHub
workflow**

### For branch/release managers

This project is using [Git Tagging](http://git-scm.com/book/en/Git-Basics-Tagging) to manage production releases.

Add a version number to a commit in `master` by doing:

    git tag -a v1.2.3 -m '<your_message_goes_here>'

Then run

    git push --tags
