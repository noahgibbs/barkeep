Barkeep Changes
===============

This file summarizes changes between tagged Barkeep versions. It lists tags in reverse chronological order.
Each tag is followed by a description of the changes it represents. This is not in a typical Changelog format,
but rather general markdown text describing important notes about the versions and progress of Barkeep.

0.3.0
-----

### Major features

* Autocomplete in the commit search box.
* Emoji!
* Demo mode
* Gradual context expander for diff view.
* Management dashboard for adding/removing repositories and troubleshooting Barkeep.
* User permissions (admin/normal) and admin dashboard for managing users.
* Massive provisioning/deployment rewrite to make it easy to get up and running.
* Introduced a vagrant-based development workflow to make it easy to test deployment.

### Minor features and bugfixes

* Using unicorn as well as multiple resque workers in production.
* Ported our styles from less to scss.
* Allow for using multiple OpenID providers.
* Greatly improved developer workflow with foreman.
* Tests for client-side coffeescript code.
* Partial sha matching redirects.
* Introduced the Barkeep client gem.
* [Fix corner cases in diff generation](https://github.com/ooyala/barkeep/issues/134)
* [Comment previews](https://github.com/ooyala/barkeep/issues/70)
* [Commit view refreshes automatically.](https://github.com/ooyala/barkeep/issues/60)
* [Replace SHAs with links in commit messages.](https://github.com/ooyala/barkeep/commit/ede08a3cbe8ffb7eb959a3bdea5dd093ac43476f)
* Introduced our own grit fork and updated it to fix many bugs and incompatibilities with recent git versions.
* [Show a list of repos on the admin page.](https://github.com/ooyala/barkeep/issues/127)
* Tons of bugfixes and too many minor features to write about.

0.2.1
-----

### Major features
* [Review requests.](https://github.com/ooyala/barkeep/issues/41)
* [Framework for string filtering in comments and commit messages.](https://github.com/ooyala/barkeep/issues/114)

### Minor features and bugfixes
* [Side-by-Slide™ view performance enhancements.](https://github.com/ooyala/barkeep/issues/113)
* [Add a keyboard shortcut for focusing commit comment box (shift+c).](https://github.com/ooyala/barkeep/commit/5d1be41032ef63b47707d4f54b5145efde10cf5b)
* [Add a small +/- header to clarify commit summary.](https://github.com/ooyala/barkeep/commit/b698fc5914269da0d26b47c8951ba0ad6755d144)
* [Link commit messages to referenced Github issues.](https://github.com/ooyala/barkeep/commit/a4c5b138f5416151c8f38673e95c4f87986f52a1)
* [Link commit messages and comments to referenced JIRA issues.](https://github.com/ooyala/barkeep/commit/9f9cff3515cee13d739ebd0bccd248b463b8f608)
* [Automatically add link to images when embedded in comments.](https://github.com/ooyala/barkeep/commit/4e255de9cb83c67ea162cb2a4598ecf61c640574)
* [Truncate long file names in commit summary and diff views.](https://github.com/ooyala/barkeep/issues/108)
* [Add permalinks to comments and link from comment emails.](https://github.com/ooyala/barkeep/issues/119)
* [Warn the user if they attempt to navigate away with an unsaved comment on the page.](https://github.com/ooyala/barkeep/issues/118)
* [Improve markdown rendering in comments.](https://github.com/ooyala/barkeep/commit/33e3f8121ea8b2a63a54cc35b898eb3e3859eaa6)
* [Redirect unambigious partial SHAs to the correct commit route.](https://github.com/ooyala/barkeep/commit/a5177d919c7d193e1e90aa137dc9a19a13bacfa5)
* Other bug fixes and style improvements

0.2.0
-----

### Major features

* Side-by-side diff view.
* [Emails are now sent upon commit ingestion.](https://github.com/ooyala/barkeep/issues/10)
* [We now show a list of changes at the top of the commit view.](https://github.com/ooyala/barkeep/issues/61)
* [Commits are now editable (our first outside contribution!)](https://github.com/ooyala/barkeep/issues/23)

### Minor features and bugfixes

* [Two bug fixes for automatic commit links.](https://github.com/ooyala/barkeep/commit/f57255b9fc74007121874b5fe0e456e78cad6741)
* [File renames are now reflected in the commit view.](https://github.com/ooyala/barkeep/commit/c996e0ba20fe3040f4754284b2aa1f5444432bc3)
* [C++ source files are highlighted](https://github.com/ooyala/barkeep/issues/101).
* [There is now a dropdown menu for each saved search to toggle email and search preferences.](https://github.com/ooyala/barkeep/commit/cc1805dbfbf718f9f57518741ba2ff66cd9f2be0)
* Background jobs now run with Resque instead of our own background jobs logic.
* Periodic jobs are now scheduled with Clockwork.
* [Images in comment boxes are resized so they don't overflow.](https://github.com/ooyala/barkeep/issues/93)
* [There is now a keyboard shortcut for approving/disapproving commits (a)](https://github.com/ooyala/barkeep/issues/25)
* [Eliminated potentially confusing red borders around characters in diffs.](https://github.com/ooyala/barkeep/issues/77)
* Empty files and symbolic links are better handled in the diff view. ([14](https://github.com/ooyala/barkeep/issues/14), [71](https://github.com/ooyala/barkeep/issues/71)).
* [Rewrite of keyboard shortcuts for sanity.](https://github.com/ooyala/barkeep/commit/82c5f86305ab9ab53f41f13261e768cf49370cdd)
* [Side-by-side now persists between page views via a cookie.](https://github.com/ooyala/barkeep/issues/48)
* [Use MIT open-source license](https://github.com/ooyala/barkeep/issues/87)
* [Comments are now editable](https://github.com/ooyala/barkeep/issues/23) (our first outside contribution!)
* Many smaller fixes and improvements.

0.1.1
-----

### Minor features and bugfixes

* [Fixed a confusing saved search title bug where the branch name was omitted](https://github.com/ooyala/barkeep/issues/76)
* [Commenter names are bold in comment emails to make them easier to spot](https://github.com/ooyala/barkeep/commit/b90d5130ac0cc83e1bbfd3314ebe433a28367d49)
* Better instructions for running Barkeep locally
* [Exclude commits from the saved search view that are not yet in the DB](https://github.com/ooyala/barkeep/issues/73)
* [Fixed the seam on the background image](https://github.com/ooyala/barkeep/issues/45)
* [Java is now syntax-highlighted](https://github.com/ooyala/barkeep/commit/a32656a99b465108a0c43288654e4aa2e2013e8b)
* [Trailing newlines are no longer omitted from the diff view](https://github.com/ooyala/barkeep/issues/64)
* Nice tooltips for certain items on the page
* [Stats page style overhauled to be more consistent with saved search view](https://github.com/ooyala/barkeep/commit/1d3a23da9af5d4f1366bfb5042d77501ff1b51fe)
* [There is a checkmark indicator in the saved search view that shows which commits have been approved](https://github.com/ooyala/barkeep/issues/67)
* [The diff parser now correctly handles single line changes](https://github.com/ooyala/barkeep/issues/64)
* [Line numbers are now unselectable](https://github.com/ooyala/barkeep/commit/3e81c5634fada33b51e4289b0a12ba4255c4ef4f)
* [Switched to our own custom syntax theme, and dropped in multiple themes to allow for user-selected swapping in the future](https://github.com/ooyala/barkeep/commit/f683134ca6674efe9bc33e1e7488393c596520dd)
* [Fixed bug where added and deleted commit comments were not reflected in the UI](https://github.com/ooyala/barkeep/issues/56)
* Fixes for Google openid failures
* Comment emails now explain why the recipients are receiving mail
* Many page and code style tweaks and fixes

0.1.0
-----

### Major features

* [Emails notifications for comments are now sent to people who have saved searches that cover the commit](https://github.com/ooyala/barkeep/issues/7)
* [There is now a time range filter that applies to all saved searches](https://github.com/ooyala/barkeep/issues/12)
* [There is a 'show unapproved only' checkbox to filter each saved search](https://github.com/ooyala/barkeep/issues/8)
* [Each chunk of code (a change plus context) in the diff view is now separated by a break indicator](https://github.com/ooyala/barkeep/issues/42)
* [We now display a line at 110 characters to indicate line limit](https://github.com/ooyala/barkeep/issues/30)
* Secret dark feature that will be officially announced in the next release

### Minor features and bugfixes

* [Diffs with long lines now scroll instead of overflowing the view](https://github.com/ooyala/barkeep/issues/1)
* [Saved searches don't scroll left from the first page (it refreshes instead)](https://github.com/ooyala/barkeep/issues/2)
* [Fix "typing j/k in a comment box moves the selected line"](https://github.com/ooyala/barkeep/issues/3)
* [Fix email thread issues](https://github.com/ooyala/barkeep/issues/4)
* [Batching for comment emails](https://github.com/ooyala/barkeep/issues/6)
* [Retry sending an email when we get "connection if reset by peer"](https://github.com/ooyala/barkeep/issues/9)
* [Enter and 'o' open commits in a new tab](https://github.com/ooyala/barkeep/issues/11)
* [Fixed bug with fenced code blocks causing nested comment forms](https://github.com/ooyala/barkeep/issues/16)
* [Fixed bug where the page number doesn't change](https://github.com/ooyala/barkeep/issues/17)
* [Fixed bug where searching with branches:all returns no results](https://github.com/ooyala/barkeep/issues/19)
* [Added 'r' shortcut to refresh saved searches](https://github.com/ooyala/barkeep/commit/e1ec4a241e6b04628a8cd1d02278687ae0fe4593)
* [Added /statusz route to report deploy-time information](https://github.com/ooyala/barkeep/commit/c5cfedaf1bb00d6930260fabc339b9ef604dcfd8)
* Hundreds of styling tweaks
* Added some tests
* Code style fixes
* Much, much more
