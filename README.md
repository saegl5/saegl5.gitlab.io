![Build Status](https://gitlab.com/pages/hugo/badges/master/build.svg)

- - -

Example [Hugo](https://gohugo.io) website using GitLab Pages.

Learn more about GitLab Pages at https://pages.gitlab.io and the official
documentation https://docs.gitlab.com/ce/user/project/pages/.

- - -

**Table of Contents** *generated with [DocToc](https://github.com/thlorenz/doctoc)*

* [GitLab CI](#gitlab-ci)
* [Building locally](#building-locally)
* [GitLab User or Group Pages](#gitlab-user-or-group-pages)
* [Did you fork this project?](#did-you-fork-this-project)
* [Troubleshooting](#troubleshooting)

## GitLab CI

This project's static Pages are built by [GitLab CI](https://about.gitlab.com/gitlab-ci/), following the steps
defined in [`.gitlab-ci.yml`](.gitlab-ci.yml).

## Building locally

To work locally with this project, you'll have to follow the steps below:

1. Fork, clone or download this project
2. [Install](https://gohugo.io/overview/installing/) Hugo
3. Preview your project: `hugo server`
4. Add content
5. Generate the website: `hugo` (optional)

Read more at Hugo's [documentation](https://gohugo.io/overview/introduction/).

### Preview your site

If you clone or download this project to your local computer and run `hugo server`,
your site can be accessed under `localhost:1313/hugo/`.

The theme used is adapted from http://themes.gohugo.io/beautifulhugo/.

## GitLab User or Group Pages

To use this project as your user/group website, you will need one additional
step: just rename your project to `namespace.gitlab.io`, where `namespace` is
your `username` or `groupname`. This can be done by navigating to your
project's **Settings**.

You'll need to configure your site too: change this line
in your `config.toml`, from `"https://pages.gitlab.io/hugo/"` to `baseurl = "https://namespace.gitlab.io"`.
Proceed equally if you are using a [custom domain](https://about.gitlab.com/2016/04/07/gitlab-pages-setup/#custom-domains): `baseurl = "http(s)://example.com"`.

Read more about [user/group Pages](http://doc.gitlab.com/ee/pages/README.html#user-or-group-pages) and [project Pages](http://doc.gitlab.com/ee/pages/README.html#project-pages).

## Did you fork this project?

If you forked this project for your own use, please go to your project's
**Settings** and remove the forking relationship, which won't be necessary
unless you want to contribute back to the upstream project.

## Troubleshooting

1. CSS is missing! That means two things:
Either that you have wrongly set up the CSS URL in your templates, or
your static generator has a configuration option that needs to be explicitly
set in order to serve static assets under a relative URL.