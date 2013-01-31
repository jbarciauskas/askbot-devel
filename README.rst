==========================
Askbot-Heroku - Q&A forum
==========================

This is Askbot project - open source Q&A system, like StackOverflow, Yahoo Answers and some others.
Askbot is based on code of CNPROG, originally created by Mike Chen 
and Sailing Cai and some code written for OSQA.

Demos and hosting are available at http://askbot.com.

Branch `0.7.x` - is the latest version supporting Django 1.5

Branch `0.8.x` - transitional version for the upgrade of the database to Django 1.7

Branch `0.9.x` - supports Django 1.7

Branch `master` supports Django 1.8

How to contribute
=================

Your pull requests are very welcome, **but please read the few paragraphs below**, it might save our combined efforts.

**Obvious bug fixes will be merged quickly**, however less obvious cases should include a clear description of how to reproduce the bug. Complex cases must be accompanied with the new unit tests.

Everyone likes good geatures, but **feature PR's may be not accepted, unless discussed beforehand in the "Issues" section or by email support@askbot.com or at the Askbot support forum**. Of course you can do anything you want in your fork, but please don't make an assumption that your giant glorious PR will be used, due to limited bandwidth for testing and to avoid "easter eggs" and the feature overload.

**Please always use feature branches for the PR's**, multiple feature/bugfix PR's are harder to understand and less likely to be accepted.

**Translators: DO NOT use git to contribute translations!!!** instead - translate at https://www.transifex.com/projects/p/askbot/.

All documentation is in the directory askbot/doc

Follow https://help.github.com/articles/fork-a-repo to to learn how to use
`fetch` and `push` as well as other help on using git.

License, copyright and trademarks
=================================
Askbot software is licensed under GPL, version 3.

Copyright Askbot S.p.A and the project contributors, 2010-2016.

"Askbot" is a trademark and service mark registered in the United States, number 4323777.

=======
Project for a web community to debate and intervene on matters of civic interest.
=======
This is Askbot project - open source Q&A system, like StackOverflow, Yahoo Answers and some others
=======
This is a fork of the Askbot project - open source Q&A system, like StackOverflow, Yahoo Answers and some others.

This fork consists of an initialized Askbot installation containing the necessary modifications to deploy in heroku with a PostgreSQL database.

To deploy in heroku:

1. Add the heroku repository as a git remote and push
2. ``syncdb`` and ``migrate``
3. Set environment variables in heroku::
   $ heroku config:set DJANGO_SETTINGS_MODULE=app.settings.prod
   $ heroku config:set SECRET_KEY="some_random_value"

To get a value for SECRET_KEY you can use the linux utility ``apg``.

I will try to keep this repository synced with https://github.com/ASKBOT/askbot-devel.git but this is not guaranteed.

The rest of this README comes from the original project.

Demo site is http://askbot.org

All documentation is in the directory askbot/doc

Askbot is based on code of CNPROG, originally created by Mike Chen 
and Sailing Cai and some code written for OSQA
