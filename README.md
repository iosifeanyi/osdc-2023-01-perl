# Open Source Development Course for Perl developers - 2023.01

https://osdc.code-maven.com/osdc-2023-01-perl/

* Start day: 2023.01.24

## TOC

* [Session 1: Welcome, Version Control, Journal, Slack](#session-1-welcome-version-control-journal-slack)
* [Assignment 1](#assignment-1)
* [Session 2: Create GitHub Pages using the git CLI; GitHub Actions](#session-2-create-github-pages-using-the-git-cli-github-actions)
* [Assignment 2](#assignment-2)
* [Session 3: GitHub Actions, CPAN Digger](#session-3-github-actions-cpan-digger)
* [Assignment 3](#assignment-3)
* [Session 4: Docker](#session-4-docker)
* [Assignment 4](#assignment-4)
* [Session 5: Docher HUB; Docker Compose](#session-5-docker-hub-docker-compose)
* [Session 6: GitHub Actions for Types::RENEEB](#session-6-github-actions-for-typesreneeb)
* [Session 7: GitHub Action for DBIx-Class, ack](#session-7-github-action-for-dbix-class-ack)
* [Session 8: DBD::Pg, test coverage with Devel::Cover](#session-8-dbdpg-test-coverage-with-develcover)
* [Session 9: git stash, detached head](#session-9-git-stash-detached-head)
* [Session 10: git stash and bisect, adding test to RSRU](#session-10-git-stash-and-bisect-adding-test-to-rsru)
* [Session 11: Git Flow; GitHub Actions for Test::Class](#session-11-git-flow-github-actions-for-testclass)
* [Next](#next)

## Session 1: Welcome, Version Control, Journal, Slack

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
    * Wikipedia and the version control there. Recommended to watch:
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

## Session 2: Create GitHub Pages using the git CLI; GitHub Actions


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

Once it is done add the following entry to your JSON file:
```
    "github_page": true,
```

See the `mentors/szabgab.json` for an example.


* Collect the git repositories of the projects you depend on. If CPAN modules then [MetaCPAN](https://metacpan.org/) might have the link.
* Add them as a list to your JSON file.  See the `mentors/szabgab.json` for an example.
* Blog about what we learned. Add links. (See my suggestions above how to improve your blog post.) If you feel something is missing from my notes (this file). Feel free to add them with a PR.


## Session 3: GitHub Actions, CPAN Digger

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
    * Some distributions have a link to their GitHub repository but not to the "issues".
    * Some distributions don't have a link to their GitHub. In some cases it isn't hard to track down the repository and then you can change it to make it include the links to the GitHub repository and to the issues.
* Blog about them!

## Session 4: Docker

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


## Session 5: Docker HUB; Docker Compose

* Show how to connect the GitHub repository to Docker hub.
    * [Docker HUB](https://hub.docker.com/repository/docker/szabgab/playground/general)
    * [GitHub](https://github.com/szabgab/playground)

The configuration file of docker to map all the data (all the volumes, images, containers) to a disk which is not the default.

```
$ cat /etc/docker/daemon.json
{
    "data-root": "/home/data/docker"
}
```


* Show one of my real-world projects using Docker compose
* Show editing a project while it is running in Docker compose
       * [PyDigger](https://pydigger.com/)
       * [GitHub](https://github.com/szabgab/pydigger.com)

Take one of the projects from the list of projects of the participants, run the tests locally using the Docker container (dr).
Open issue when necessary. Set up GitHub Actions if needed. Create test coverage report.

* We looked at https://github.com/reneeb/Types-RENEEB and found out that Steve already had a fork and that his changes were already applied to the original repo. (The best course of action at this point might be is to remove the fork and create it again.)
    * We found that the project had clear instructions on how to set up the development environment and how to run the tests. Nice.
    * We also found that some of the tests fail. Not so good. Steve will check why. He will probably open an issue with the failure. Even if later he finds out the reason, it is a good idea to have it documented on GitHub.

* [Video 5-1](https://youtu.be/OtSv-abMCmg)
* [Video 5-2](https://youtu.be/nYvXhBvMBSU)

### Assignment 5

* Pick one or more projects
* Try to setup the local development environment.
    * If you cannot, open an issue asking the author how. (Feel free to mention me by including @szabgab and mentioning the course by including a link to to https://osdc.code-maven.com/
    * If you can setup verify that there are clear instructions how to do this in the README file or in some other file (e.g. CONTRIBUTING).
        * If there are not, send a PR with the instructions so the next person will have less trouble.
    * Run the tests locally.
        * If there are failures report them.
    * Check if GitHub Actions is configured. If not, then configure it. (or open an issue asking the author if s/he wants it).
    * Create test coverage report. Add more tests if possible.


## Session 6: GitHub Actions for Types::RENEEB

* We sent several pull-requests to [Types-RENEEB](https://github.com/reneeb/Types-RENEEB)
    * [updated files generated by `dist zilla`](https://github.com/reneeb/Types-RENEEB/pull/7)
    * [fixing a test failure](https://github.com/reneeb/Types-RENEEB/pull/8)
    * [Adding Github Actions](https://github.com/reneeb/Types-RENEEB/pull/9). We started with the [GitHub Action skeleton](https://code-maven.com/github-actions) for Dist::Zilla.
    * Renee, the author of this project accepted our Pull-Requests within a few minutes. Then we sent another PR
    * [enabling more OSes and versions of Perl in GitHub Actions](https://github.com/reneeb/Types-RENEEB/pull/10)

* Clone the original repository

```
git clone git@github.com:reneeb/Types-RENEEB.git
```

* Create a fork of the repository via GitHub UI.

* Setup a new git remote to point to the forked repository:

```
git remote add fork git@github.com:yewtc/Types-RENEEB.git
```

* Create a branch to prepare a pull-request

```
git checkout -b BRANCH
  make changes
git add .
git commit -m "..."
git push --set-upstream fork BRANCH
```

* Send the pull-request from the GitHub UI

* Integrate the progress of original repository to our local clone

```
git checkout master
git pull origin master
```

* Once the Pull-request was accepted we could delete the branch locally and remotely

```
git branch -d BRANCH
git push -d origin BRANCH
```

* We created Test coverage report of the Types-RENEEB pacakge. It was not too interesting as everything was 100%.

```
cpanm Dist::Zilla::App::Command::cover

dzil cover
```

* We also sent a [pull-request](https://github.com/pjcj/Devel--Cover/pull/319) to [Devel::Cover](https://github.com/pjcj/Devel--Cover) with this information.

* [Video 6-1](https://youtu.be/EuXjJNMlF7U)
* [Video 6-2](https://youtu.be/j3fydLZ9cjU)

## Session 7: GitHub Action for DBIx-Class, ack

In this session we tried to add GitHub Actions (CI) to [DBIx::Class](https://metacpan.org/dist/DBIx-Class).

It already had an extensive configuration of [Travis-CI](https://www.travis-ci.com/), but unfortunately Travis stopped its free service.

I briefly explained how my [slides](https://code-maven.com/slides/) used to be generated using a Webhook.

We used the [playground Docker image](https://github.com/szabgab/playground) we covered in a previous session.

We still had to install [Module::Install](https://metacpan.org/pod/Module::Install) as it was a developer dependency.

```
cpanm --notest Module::Install
```


Then we could install all the other dependencies:

```
cpanm --installdeps --notest .
```

However when we ran `perl Makefile.PL` it still complained about a lot of missing modules. So we created a temporary file just to install those:

```
cpanm --notest Class::DBI::Plugin::DeepAbstractSearch
cpanm --notest Class::MethodCache
cpanm --notest Class::Unload
cpanm --notest Date::Simple
cpanm --notest DateTime::Format::MySQL
cpanm --notest DateTime::Format::Pg
cpanm --notest DateTime::Format::SQLite
cpanm --notest DateTime::Format::Strptime
cpanm --notest JSON
cpanm --notest JSON::Any
cpanm --notest JSON::DWIW
cpanm --notest JSON::XS
cpanm --notest Math::Base36
cpanm --notest MooseX::Types::JSON
cpanm --notest MooseX::Types::LoadableClass
cpanm --notest MooseX::Types::Path::Class
cpanm --notest PadWalker
cpanm --notest Pod::Coverage
cpanm --notest SQL::Translator
cpanm --notest Test::EOL
cpanm --notest Test::NoTabs
cpanm --notest Test::Pod
cpanm --notest Test::Pod::Coverage
cpanm --notest Test::Strict
cpanm --notest Text::CSV
cpanm --notest Time::Piece::MySQL
```

There must be a better way to install all of these, but we could not find the instructions.
So one addition to the project could be an easy way to find insttruction on how to set up
the local development environment.

After this we managed to run the tests though many were skipped for various reasons. For example some needed access to real databases.

Then we set up CI based on one of the [GitHub Actions examples](https://code-maven.com/github-actions).

We pushed it out, but it did not start to work. Yesterday GitHub had a big outage, so we looked at the [GitHub status](https://www.githubstatus.com/) and indeed, GitHub Actions was yellow. It did not work properly. Eventually it started our job, but it took several minutes to do so.

To our (or at least my) surprise, once GitHub Actions started to run the tests passed on the first attempt.


However we wanted to see how to run the tests with PostgreSQL as well.

For that we had to install [DBD::Pg](https://metacpan.org/pod/DBD::Pg), another module that does not have a CI. (neither to [DBD::mysql](https://metacpan.org/pod/DBD::mysql) nor [DBD::Oracle](https://metacpan.org/pod/DBD::Oracle) for that matter.

To install DBD::Pg locally we found in the readme of DBD::Pg which is linked from the [DBD-Pg](https://metacpan.org/dist/DBD-Pg) page. (I did not remember that during our session.)


```
apt-get install libpq-dev
cpanm --notest DBD::Pg
```

Then we added another YAML file for the GitHub Action, this time running insied a Docker container, based on the [PostgreSQL GitHub Action example](https://code-maven.com/github-actions).

It needed some parameters to pass the hostname of the Postgres server, the name of the database, the username and the password.

I briefly used and mentioned [ack](https://metacpan.org/dist/ack/view/ack) aka. [beyondgrep](https://beyondgrep.com/) an excellent grep-like tool in Perl.

To our surprise this too worked on the first try. I was so surprised I had to see a more detailed report and thus we split the GitHub Action job up and had a separate section where we used [prove](https://metacpan.org/dist/Test-Harness/view/bin/prove) to run the tests in verbose mode.


At the end we sent a [pull-request](https://github.com/Perl5/DBIx-Class/pull/147) with what we accomplished.

* [Video 7-1](https://youtu.be/imB85UpzZVY)
* [Video 7-2](https://youtu.be/bSx4Wxul8iM)


## Session 8: DBD::Pg, test coverage with Devel::Cover

* [Video 8-1](https://youtu.be/hqdeOy354QU)
* [Video 8-2](https://youtu.be/ZmmWUE2etNo)

* We saw how to setup a development environment for [https://metacpan.org/pod/DBD::Pg](https://metacpan.org/pod/DBD::Pg) using Docker and Docker Compose.
* Then we looked at the coverage report of this module using [Devel::Cover](https://metacpan.org/pod/Devel::Cover)
* We looked at [CPANcover](http://cpancover.com/)

* We looked at the [CPAN River list of distribution](http://neilb.org/2016/01/26/river-head-quality.html)
* We looked at the test coverage report of [DateTime::Format::Pg](https://metacpan.org/pod/DateTime::Format::Pg)
* We tried to reproduce [this issue](https://github.com/lestrrat-p5/DateTime-Format-Pg/issues/23) but got to the conclusion that it looks like an incorrect expectaton from the user.
* [DateTime::Format::Pg](https://metacpan.org/pod/DateTime::Format::Pg)
* [DateTime::TimeZone](https://metacpan.org/pod/DateTime::TimeZone)
* [Docker compose with PostgreSQL](https://code-maven.com/slides/docker/docker-compose-postgresql-server)
* We talked about [Test-Exception](https://metacpan.org/pod/Test::Exception) and [SKIP](https://code-maven.com/slides/test-automation-using-perl/test-more-skip).
* I mentioned the [Pay It Forward](https://osdc.code-maven.com/pif) project. Apparently it is an American expression.
* It would be nice to add the test coverage numbers to [CPAN-Digger](https://cpan-digger.perlmaven.com/)



## Session 9: git stash, detached head

* git

git add -i
git stash -u
git stash list
git stash show
git stash show -p


* [Video 9-1](https://youtu.be/RR0tQbOhzzU)
* [Video 9-2](https://youtu.be/rY3nTmJ4iRw)


## Session 10: git stash and bisect, adding test to RSRU

Date: 2023.04.25

git
    detached head
    merge / rebase
    reset
    stash
    bisect
    revert

* [Math::RPN](https://metacpan.org/pod/Math::RPN)
* In the 2nd video we added a test to [RSRU](https://github.com/lordfeck/rsru) see the [Pull-request](https://github.com/lordfeck/rsru/pull/62)

* [Video 10-1](https://youtu.be/TheqgwWH0MI)
* [Video 10-2](https://youtu.be/qT8SK7OkVAs)

## Session 11: Git Flow; GitHub Actions for Test::Class

Date: 2023.05.02

* We talked about Git Flow vs. having a single main branch. The latter would need a good (acceptance/integration) test coverage
so you can trust the test for a release without requiring manual QA. (The manual QA can still work as exploratory testing
that also feeds ideas to the people who then convert the test-cases into automated tests.

* We looked at the CI system of [Test::Class](https://metacpan.org/pod/Test::Class) that first creates a release and then uses that release on various versions of Perl to test it. It also tests a number of downstream distributions to verify that the new version does not break them.
* We looked at the GitHub Actions and the source code of [CPAN Dashboard](https://cpandashboard.com/)
* We looked at the [MetaCPAN tools](https://metacpan.org/tools) and the experimental dashboard there.
* We looked at the [stats page of PyDigger](https://pydigger.com/stats) and the mess of the [licenses](https://pydigger.com/licenses).
* [CPAN Rocks](https://cpan.rocks/)

* [Video 11-1](https://youtu.be/wC9GADfNI_o)
* [Video 11-2](https://youtu.be/SPN6gHWkizs)

## Session 12

* Date: 2023.05.16

* [GitHub Action when files change](https://github.com/szabgab/github-actions-run-code-if-files-change/)

* We talked about frequency of Pull-Requests or code-reviews.

* Docker caching - changing the Makefile.PL outside will make the `COPY Makefile.PL .` command run again
and that will trigger all the steps that follow it.

* [Video 12-1](https://youtu.be/jrQYrqHQrq4)
* Unfortunately I've forgotten to record the 2nd part.

## Next

* GitHub actions for a project that needs database access
* Test coverage report for other projects

* CPAN-Digger

Take one of the projects from the list of projects of the participants, run the tests locally using the Docker container (dr).
Open issue when necessary. Set up GitHub Actions if needed. Create test coverage report.

## Session 13 plans for 2023.05.16

