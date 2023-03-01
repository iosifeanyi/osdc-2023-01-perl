# Open Sorce Development Course for Perl developers - 2023.01

https://osdc.code-maven.com/osdc-2023-01-perl/

* Start day: 2023.01.24

## TOC

* [Session 1 - Welcome - Version Control - Journal - Slack](#session-1---welcome---version-control---journal---slack)
* [Assignment 1](#assignment-1)
* [Session 2 - Create GitHub Pages using the git CLI; GitHub Actions](#session-2---create-github-pages-using-the-git-cli-github-actions)
* [Assignment 2](#assignment-2)
* [Session 3 - GitHub Actions, CPAN Digger](#session-3---github-actions-cpan-digger)
* [Assignment 3](#assignment-3)
* [Assignment 4](#assignment-4)

## Session 1 - Welcome - Version Control - Journal - Slack

* Welcome
    * overview of the [course](https://osdc.code-maven.com/)
        * git
        * GitHub
        * (GitLab)
        * Markdown
        * Docker
        * Testing
        * Static analysis
        * Communication
        * Slack
    * a little about myself
        * Self employed
        * Training
        * Introducing testing, CI etc.
    * If you'd like to send me an email reply to the one I sent you. Keep the subject line. Remove the irrelevant content.
      Without this it is **very** difficult for me to associate all the emails with the different courses I teach.
    * Assignments
        * Will be in some public GitHub or GitLab repositories
        * At the end of each assignment you'll write a report - a blog post / journal entry.
        * You will add it to your personal JSON file and send a Pull-Request with the change. (We'll learn these soon)
        * First few assignments will be to my projects or your own projects. This allows for quick feedback and integration.
        * Then we'll find you open source projects maintained by other people.
    * The more you participate, the more you learn in this course.
    * The more effort you put in this course, the more you will gain.
        * Ask questions!
        * Try to help others! The more you help others the more you will learn.
    * Grades: (if relevant) are based on the work done during the course. There is no end-project or exam at the end.

* Version Control
    * Why use version control?
    * Wikipedia and the verion control there. Recommended to watch:
        * [How to edit wikipedia](https://code-maven.com/edit-wikipedia)
        * [How to edit wikipedia (in Hebrew)](https://he.code-maven.com/edit-wikipedia)
        * [Como editar una página en Wikipedia](https://es.code-maven.com/editar-wikipedia)

* [GitHub](https://github.com/): process of contributing to an Open Source project using the GitHub web site. Editing and sending a Pull-Request. Use a the `cm-demo` user to make a change in the README of this repository and then to add the json file. Show how the CI fails when we add an incorrectly formatted file.
* What is [JSON](https://www.json.org/)?

* Show the Git repository of the project and the web site generated from it.

* Show blogging platform
    * [DEV](https://dev.to/) - See [my account](https://dev.to/szabgab/)

* We saw the drawing of the GitHub process in the cloud.

* We looked at [CPAN-Digger](https://cpan-digger.perlmaven.com/)
* We looked at the  [recent on MetaCPAN](https://metacpan.org/recent)
* We looked at some of the features of GitHub while looking at the [Dancer](https://github.com/PerlDancer/Dancer2/) project. (Insights, list of commits, forks, stars, watch)
* [The original Markdown](https://daringfireball.net/projects/markdown/syntax)
* [GitHub flavored Markdown](https://github.github.com/gfm/)
* [Markdown](https://en.wikipedia.org/wiki/Markdown).
    * Subtitle
    * Bullet points
    * Links
    * Bold

* [Video 1-1](https://youtu.be/HPUuiUBMbEE)
* [Video 1-2](https://youtu.be/qGAVORyZZrI)

### Assignment 1

* You will have to publish a journal of your process.
    * [DEV](https://dev.to/) - shared blogging platform. See [my account](https://dev.to/szabgab/)
* Create an account on the blogging platform you selected. (if you already have one, you can use that)
* Create an account on [GitHub](https://github.com/) (if you already have one, use that)
* Create an account on [GitLab](https://gitlab.com/) (if you already have one, use that)
* Add a picture to all these accounts. It is preferably a picture of you, but it can be a drawing of you, or some other avatar you might want to use.
* Send a pull-request to the GitHub repository of the course adding a JSON file. The name of the file should be your GitHub username and it should include key-value pairs as in the example. (The `posts` will be an empty list.) Check the result of GitHub Actions.
* Join the Slack workspace (I send invitations to everyone to their email address.) and say hi.
* Write a blog post about the course. In your post link to your GitHub and GitLab accounts and to your Pull-Request. If you encountered any issue, write about that and how you solved it. If you use an avatar instead of your own picture, describe how you created the avatar.
* In the blog post tell us a bit about your background.
    * What programming language(s) you use?
    * Which interesting 3rd-party libraries do you use? You can mention big ones, but it is probably more interesting if you mention more esoteric ones.
    * Include links to the home-page of each project and the GitHub/GitLab repository of each project.
    * What would you like to accomplish in the course?
    * Which open source projects would you like to contribute to.
* Update your Pull-request adding the URL to the blog post to the `posts` field in the json file.

* There are 3 GitHub repositories with lists of GitHub organization published by [higher education institutions](https://github.com/szabgab/open-source-by-higher-education), [governments](https://github.com/szabgab/open-source-by-government), and [corporations](https://github.com/szabgab/open-source-by-corporations). Find at least 5 more organizations that share some of their code using an open source license in GitHub or GitLab. An organization can be a corporation, a university, a college, a research institute, or a government. (e.g. find a list of universities and use the search feature of GitHub to find **GitHub organizations** that belong to the institute).

A couple of suggestions for the blog posts
* Use a title that can sound interesting to others as well eg. **How to contribute to an open source project** or  **How to Send a pull request on GitHub**.
* Add `osdc` tag and other relevant tags.
* Add the `series:` field to the `Jekyll front matter` (the header of each post on DEV.to)
* Use Markdown in the post.
* Include links to the relevant sites and pages such as the web site of the [Open Source Development Course](https://osdc.code-maven.com/) and the web site of our course: [Open Source Development Course for Perl developers](https://osdc.code-maven.com/c/osdc-2023-01-perl).

## Session 2 - Create GitHub Pages using the git CLI; GitHub Actions


* [HTML - Hyper Text Markup Language](https://en.wikipedia.org/wiki/HTML)
    * just view source in a browser

* GitHub pages https://cm-demo.github.io/
    * Plain Markdown files in the `docs/` folder
    * Configuring GitHub Actions with Jekyll in the `.github/workflows/` folder.  Then we changed the source to be `docs`.

* Git configuration


```
git config --global --add user.name "Foo Bar"
git config --global --add user.email foo@bar.com
```

These commands created the `~/.gitconfig` file.


```
ssh-keygen  Add public key to GitHub in User setting area
```


```
git clone

git status
git diff
git add
git commit
git show SHA
git push
git remote -v

git blame

git pull    # both with merge and rebase
```

In `~/.gitconfig` set the default action for `pull`:

```
[pull]
    rebase = true
```

We also saw:

```
gitk --all
```

* [Video 2-1](https://youtu.be/hQCaeUEKXTo)
* [Video 2-2](https://youtu.be/BgPN3XcdCBk)

### Assignment 2

* Set up your own website on github pages

Once it is done add the follwing entry to your JSON file:
```
    "github_page": "true",
```

See the `mentors/szabgab.json` for an example.


* Collect the git repositories of the projects you depend on. If CPAN modules then [MetaCPAN](https://metacpan.org/) might have the link.
* Add them as a list to your JSON file.  See the `mentors/szabgab.json` for an example.
* Blog about what we learned. Add links. (See my suggestions above how to improve your blog post.) If you feel something is missing from my notes (this file). Feel free to add them with a PR.


## Session 3 - GitHub Actions, CPAN Digger

* GitHub Actions
* [GitHub Actions slides](https://code-maven.com/slides/github-ci/actions)
* [GitHub Actions examles](https://code-maven.com/github-actions)

Specifically we looked at
* [Bash](https://github.com/szabgab/github-actions-bash)
* [PostgreSQL](https://github.com/szabgab/github-actions-postgresql/)
* [Perl with Makefile.PL](https://github.com/szabgab/github-actions-perl-makefile/)
* [OSDC Site generator](https://github.com/OSDC-Code-Maven/osdc-site-generator)

* [The checkout action](https://github.com/actions/checkout)

* We sent [this Pull Request](https://github.com/richterger/Perl-LanguageServer/pull/168) to the [Perl-LanguageServer](https://github.com/richterger/Perl-LanguageServer)
* We looked for the GitHub repository of [SPVM-FindBin](https://metacpan.org/dist/SPVM-FindBin), checked out another CPAN module of the same author and found the repo [here](https://github.com/yuki-kimoto/SPVM-FindBin/)

* [Docker Hub](https://hub.docker.com/)


* [CPAN Digger](https://cpan-digger.perlmaven.com/)

* We had a short intro to clone/branch/push/pr/pull but we'll cover it again.

* [Video 3-1](https://youtu.be/AmLAHWbvo5I)
* [Video 3-2](https://youtu.be/tzy9Me3S_jc)


### Assignment 3

* Find at least 2 Perl modules on CPAN Digger that has "something missing". Send a pull-request to each one of them.
    * Look at [CPAN Digger](https://cpan-digger.perlmaven.com/)
    * Some distributions have a link to their GitHub repositorybut not to the "issues".
    * Some distributions don't have a link to their GitHub. In some cases it isn't hard to track down the repository and then you can change it to make it include the links to the GitHub repository and to the issues.
* Blog about them!

## Session 4 Docker

(2023.02.28)

We set out working on one of the Perl modules listed in the JSON files in the participants/ folder, but then ended up covering Docker.

We used many examples from the [Docker slides](https://code-maven.com/slides/docker/) to introduce Docker.

We saw the [Docker image](https://github.com/szabgab/mydocker) I use to deal with various open source projects.

We added Dist::Zilla to this image.

* [Video 4-1](https://youtu.be/jegwGfSC5rs)
* [Video 4-2](https://youtu.be/N8ht-UDMqWQ)


### Assignment 4

* Create a Docker image for yourself.
* Run the tests of one of your favorite modules inside the container.
* Write a blog post linking to the issues you opened and the Pull-Request you sent. Even if they have not been accepted. Then add the link of that blog post to your JSON file in the participants folder.


## Session 5 plans for 2023.03.14

* Show how to connect the GitHub repository to Docker hub.
* Show one of my real-world projects using Docker compose
* Show editing a project while it is running in Docker compose

Take one of the projecs from the list of projects of the participants, run the tests locally using the Docker container (dr).
Open issue when necessary. Set up GitHub Actions if needed. Create test coverage report.


