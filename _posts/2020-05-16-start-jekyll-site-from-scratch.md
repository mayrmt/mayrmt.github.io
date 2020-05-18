---
layout: post
title:  "Starting a GitHub Pages site from scratch"
date:   2020-05-16 21:53:12 +0200
categories: jekyll update
---

I wanted to start my own GitHub Pages site from scratch.
In particular, I really want to be able to develop and test the site locally and push to GitHub only,
if new contributions have been tested on my local machine.

To start a [jekyll](www.jekyllrb.org)-based site on GitHub pages from scratch,
I have oriented myself along the [instructions in the GitHub documentstion](https://help.github.com/en/github/working-with-github-pages/creating-a-github-pages-site-with-jekyll).
Yet, some details were missing or confusing (at least to me).

Here are the steps, that work for me:

1. Navigate to the parent directory, in which you want to create the folder to store the website repository

    ```bash
    cd <parentDirectory>
    ```

1. Create an empty `git` repository for the website:

    ```bash
    git init <GitHubUserName>.github.io
    ```

1. Create an emtpy jekyll-based site  via `jekyll new .`.
1. Open the auto-generated Gemfile
    1. Follow the instructions in the Gemfile's comments to use GitHub Pages.
    1. Update the `gem "github-pages"`line so that the line looks like this,
    replacing `<version>` with the current dependency version for `github-pages`.

    ```
    gem "github-pages", "~> <version>", group: :jekyll_plugins
    ```

    For more information, see [Dependency versions](https://pages.github.com/versions/) on the GitHub Pages site. 
    1. Close the `Gemfile`.
1. Remove the auto-generated `Gemfile.lock` via `rm Gemfile.lock`.
Otherwise, the next step failed with inconsistencies in version numbers of various components defined in the `Gemfile`.
1. Run `bundle install`.

The jekyll setup is now finished and you can start do develop your site.
To preview the site on your local machine, run `bundle exec jekyll serve` and use a brownser to navigate to the `Server address:`,
that has been printed in the terminal.

As your site is wrapped into a regular `git` repository, remember to commit your changes.
Once you're ready to publish the site, commit everything and push to GitHub via:

1. Create a repository with the name `<GitHubUserName>.github.io` on GitHub.
1. Set the new repository as remote on your local repository.
1. Push your local repository to GitHub.

Now, you can view your published site at `https://<GitHubUserName>.github.io`.
It might take a minute or two for jekyll to actually generate your site, so be patient.
The results will be worth it!
