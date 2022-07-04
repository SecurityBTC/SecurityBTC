### Hi there 👋

<!--
**SecurityBTC/SecurityBTC** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->



Server Seed (hash)

Client Seed

Nonce

New seeds

Server Seed (hash)

Client Seed

Nonce

Use New Seeds

e9f85e849a647ecbd428c6001ed013a5fca714da02e2b419c8a67b99ca1fd5bf


<!--
**SecurityBTC/SecurityBTC** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
--># Welcome to Bitcoin.org's Codebase

Current Build Status: ![Build Status](https://travis-ci.org/bitcoin-dot-org/bitcoin.org.svg?branch=master)

Live site: [Bitcoin.org](https://bitcoin.org)

Report problems or help improve the site by opening a [new issue](https://github.com/bitcoin-dot-org/bitcoin.org/issues/new) or [pull request](https://github.com/bitcoin-dot-org/bitcoin.org/compare).

## Earn Bitcoin for Contributing
Open issues [labeled with "Bounty"](https://github.com/bitcoin-dot-org/bitcoin.org/labels/Bounty)
have bounties on them. Viewing the issue will reveal the value of the bounty.
Submit a pull request resolving the issue along with an accompanying note or
comment containing a bitcoin address and automatically receive a payment in the
amount of the bounty if it gets merged.

## How to Participate
The following quick guides will help you get started:

+ [Becoming a Contributor](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/become-a-contributor.md)
+ [Working with GitHub](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/working-with-github.md)
+ [Setting Up Your Environment](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/setting-up-your-environment.md)
+ [Improving Developer Documentation](https://github.com/bitcoin-dot-org/developer.bitcoin.org/)
+ [Assisting with Translations](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/assisting-with-translations.md)
+ [Adding Exchanges](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/adding-exchanges.md)
+ [Managing Wallets](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/managing-wallets.md)
+ [Adding Events, Release Notes and Alerts](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/adding-events-release-notes-and-alerts.md)
+ [Adding Blog Posts](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/adding-blog-posts.md)
+ [Miscellaneous / Other](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/miscellaneous.md)

### Code of Conduct

Participation in this project is subject to a [Code of Conduct](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/CODE_OF_CONDUCT.md).


# bitcoin
Navegações
Could not load web page at http://bitcoin.io/bitcoin.org because:

 net::ERR_INTERNET_DISCONNECTED

README.md
CI Scripts
This directory contains scripts for each build step in each build stage.

Running a Stage Locally
Be aware that the tests will be built and run in-place, so please run at your own risk. If the repository is not a fresh git clone, you might have to clean files from previous builds or test runs first.

The ci needs to perform various sysadmin tasks such as installing packages or writing to the user's home directory. While most of the actions are done inside a docker container, this is not possible for all. Thus, cache directories, such as the depends cache, previous release binaries, or ccache, are mounted as read-write into the docker container. While it should be fine to run the ci system locally on you development box, the ci scripts can generally be assumed to have received less review and testing compared to other parts of the codebase. If you want to keep the work tree clean, you might want to run the ci system in a virtual machine with a Linux operating system of your choice.

To allow for a wide range of tested environments, but also ensure reproducibility to some extent, the test stage requires docker to be installed. To install all requirements on Ubuntu, run

sudo apt install docker.io bash
To run the default test stage,

./ci/test_run_all.sh
To run the test stage with a specific configuration,

FILE_ENV="./ci/test/00_setup_env_arm.sh" ./ci/test_run_all.sh
Configurations
The test files (FILE_ENV) are constructed to test a wide range of configurations, rather than a single pass/fail. This helps to catch build failures and logic errors that present on platforms other than the ones the author has tested.

Some builders use the dependency-generator in ./depends, rather than using the system package manager to install build dependencies. This guarantees that the tester is using the same versions as the release builds, which also use ./depends.

If no FILE_ENV has been specified or values are left out, 00_setup_env.sh is used as the default configuration with fallback values.

It is also possible to force a specific configuration without modifying the file. For example,

MAKEJOBS="-j1" FILE_ENV="./ci/test/00_setup_env_arm.sh" ./ci/test_run_all.sh
The files starting with 0n (n greater than 0) are the scripts that are run in order.

Cache
In order to avoid rebuilding all dependencies for each build, the binaries are cached and re-used when possible. Changes in the dependency-generator will trigger cache-invalidation and rebuilds as necessary.
# Welcome to Bitcoin.org's Codebase

Current Build Status: ![Build Status](https://travis-ci.org/bitcoin-dot-org/bitcoin.org.svg?branch=master)

Live site: [Bitcoin.org](https://bitcoin.org)

Report problems or help improve the site by opening a [new issue](https://github.com/bitcoin-dot-org/bitcoin.org/issues/new) or [pull request](https://github.com/bitcoin-dot-org/bitcoin.org/compare).

## Earn Bitcoin for Contributing
Open issues [labeled with "Bounty"](https://github.com/bitcoin-dot-org/bitcoin.org/labels/Bounty)
have bounties on them. Viewing the issue will reveal the value of the bounty.
Submit a pull request resolving the issue along with an accompanying note or
comment containing a bitcoin address and automatically receive a payment in the
amount of the bounty if it gets merged.

## How to Participate
The following quick guides will help you get started:

+ [Becoming a Contributor](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/become-a-contributor.md)
+ [Working with GitHub](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/working-with-github.md)
+ [Setting Up Your Environment](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/setting-up-your-environment.md)
+ [Improving Developer Documentation](https://github.com/bitcoin-dot-org/developer.bitcoin.org/)
+ [Assisting with Translations](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/assisting-with-translations.md)
+ [Adding Exchanges](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/adding-exchanges.md)
+ [Managing Wallets](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/managing-wallets.md)
+ [Adding Events, Release Notes and Alerts](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/adding-events-release-notes-and-alerts.md)
+ [Adding Blog Posts](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/adding-blog-posts.md)
+ [Miscellaneous / Other](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/docs/miscellaneous.md)

### Code of Conduct

Participation in this project is subject to a [Code of Conduct](https://github.com/bitcoin-dot-org/bitcoin.org/blob/master/CODE_OF_CONDUCT.md).
# Google Research

This repository contains code released by
[Google Research](https://research.google).

All datasets in this repository are released under the CC BY 4.0 International
license, which can be found here:
https://creativecommons.org/licenses/by/4.0/legalcode.  All source files in this
repository are released under the Apache 2.0 license, the text of which can be
found in the LICENSE file.

---

Because the repo is large, we recommend you download only the subdirectory of
interest:

```
SUBDIR=foo
svn export https://github.com/google-research/google-research/trunk/$SUBDIR
```

If you'd like to submit a pull request, you'll need to clone the repository;
we recommend making a shallow clone (without history).

```
git clone git@github.com:google-research/google-research.git --depth=1
```

---

*Disclaimer: This is not an official Google product.*


