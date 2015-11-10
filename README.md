# The FrostWire Monorepo

Welcome to the main FrostWire repository. 
Here you will find the sources necessary to build [FrostWire for Android](http://www.frostwire.com/android/?from=github) and [FrostWire for Desktop](http://www.frostwire.com/downloads/?from=github)

 * [/android](https://github.com/frostwire/frostwire/tree/master/android) Sources for FrostWire for Android
 * [/desktop](https://github.com/frostwire/frostwire/tree/master/desktop) Sources for FrostWire for Desktop (Windows, Mac, Linux)
 * [/common](https://github.com/frostwire/frostwire/tree/master/common) Common sources for the desktop and android client

In the past these sources were held at [frostwire-android](https://github.com/frostwire/frostwire-android), 
[frostwire-desktop](https://github.com/frostwire/frostwire-desktop) and [frostwire-common](https://github.com/frostwire/frostwire-common) and [https://github.com/frostwire/frostwire-common](frostwire-common) respectively.
**These repositories will no longer be used.**

# Coding Guidelines

[5 Object Oriented Programming Principles learned during the last 15 years][3]
[3]: <http://bit.ly/y0hdR4>

* Keep it simple. ([KISS](https://en.wikipedia.org/wiki/KISS_principle))
* Do not repeat yourself. ([DRY](https://en.wikipedia.org/wiki/Don%27t_repeat_yourself)) Re-use your own code and our code. It'll be faster to code, and easier to maintain.
* If you want to help, the [Issue tracker](https://github.com/frostwire/frostwire-desktop/issues) is a good place to take a look at.
* Try to follow our coding style and formatting before submitting a patch.
* **All pull requests should come from a feature branch created on your git fork**. We'll review your code and will only merge it to the master branch if it doesn't break the build. If you can include tests for your pull request you get extra bonus points ;)
* When you submit a pull request try to explain what issue you're fixing in detail and how you're fixing in detail it so it's easier for us to read your patches. If it's too hard to explain what you're doing, you're probably making things more complex than they already are. Look and test your code well before submitting patches.
* We prefer well named methods and code re-usability than a lot of comments. Code should be self-explanatory.


# Contribution Guidelines

Every countribution merged to the master branch will automatically receive a tip of 1% of whatever funds are available on the [tip4commit fund](https://tip4commit.com/github/frostwire/frostwire-android).

Tip for next commit: [![see here](http://tip4commit.com/projects/538.svg)](http://tip4commit.com/projects/538)

If you want to contribute code, start by looking at the [open issues on github.com](https://github.com/frostwire/frostwire-desktop/issues).

If you want to fix a new issue that's not listed there, create the issue, see if
we can discuss a solution.

Please follow the following procedure when creating features to avoid unnecessary rejections:

* Fork the source.
* Clone it locally
* Create a branch with a descriptive name of the issue you are solving.
* Make sure the name of your feature branch describes what you're trying to fix. If you don't know what to name it and there's an issue created for it, name your branch issue-233 (where 233 would be the number of the issue you're fixing).
* Focus on your patch, do not waste time re-formatting code too much as it makes it hard
  to review the actual fix. Good patches will be rejected if there's too much code formatting
  noise, we are a very small team and we can't waste too much time reviewing if something
  got lost or added in the middle of hundreds of lines that got shifted.
* Code, Commit, Push, Code, Commit, Push, until the feature is fully implemented.
* If you can add tests to demonstrate the issue and the fix, even better.
* Submit a pull request that's as descriptive as possible. Adding (issue #233) to the commit message or in PR comments automatically references them on the issue tracker.
* We'll code review you, maybe ask you for some more changes, and after we've tested it we'll merge your changes.

If your branch has taken a while to be accepted for merging into `master`, it's very likely that the `master` branch will have moved forward while you work. In this case, make sure to sync your `master`.

    git checkout master
    git pull upstream master

and then rebase your branch to bring it up to speed so it can be merged properly (do not merge `master` into your branch):

    git checkout my-branch
    git rebase master

As you do this you may have to fix any possible conflicts, just follow the instruction git gives you if this is your first time.

Make sure to squash any cosmetic commits into the body of your work so that we don't pollude the history and you don't get more bitcoins than you should from the rest of the collaborators for things like fixing a typo you just introduced on your branch.

_Repeat and rinse, if you send enough patches to demonstrate you have a good
coding skills, we'll just give you commit access on the real repo and you will
be part of the development team._

# Tip 4 commit

All merged contributions automatically get 1% of whatever is left on our tip4commit fund in bitcoins.

[![tip for next commit](https://tip4commit.com/projects/43144.svg)](https://tip4commit.com/github/frostwire/frostwire)

# How to build

Instructions on how to build are included inside each project, we're still making the migration into this monorepo structure, so we'll accept gladly any commits refering to the README.md files found here.

For now, `desktop/` has to be built from the root of the monorepo as simple as doing:
`gradle build`

For `android/`, go inside the directory and do:
`./gradlew assembleDebug`

### License

Frostwire Desktop is offered under the [GNU General Public License](http://www.gnu.org/copyleft/gpl.html). Available [here](LICENSE.txt).


### Official FrostWire sites

[Main Website Frostwire.com](http://www.frostwire.com) |
[Frostwire Forum](http://forum.frostwire.com) |
[Facebook](http://www.facebook.com/FrostWireOfficial) |
[Twitter @frostwire](https://twitter.com/frostwire) |
[Tumblr](http://tumblr.frostwire.com)
