# Self-Hosted Application Directory

[selfh.st/apps](https://selfh.st/apps) is a directory built for easy browsing and discovery of self-hosted software and related applications. 

This repository serves as a data store for the static files used to populate the directory:

* [/data](https://github.com/selfhst/apps/tree/main/data): JSON files populated from a backend database with project details for generating tiles
* [/icons](https://github.com/selfhst/apps/tree/main/icons): SVG, PNG, and WEBP icons for projects when available
* [/releases](https://github.com/selfhst/apps/tree/main/releases): RSS release feeds for each project excluding pre-releases, alphas, betas, and release candidates

While readers are free to browse and reference the contents of the repository, they are subject to change as the project evolves. Details surrounding periodic updates can be found in the repository's [changelog](https://github.com/selfhst/apps/blob/main/CHANGELOG.md).

### Frequently Asked Questions

#### How can I add my project to the directory?

Feel free to [reach out](mailto:hello@selfh.st) and share the details of your project with me.

Note that I will not manually intervene with the order in which a project is displayed. The current sort options (repository stars, last activity, alphabetical, recently added) are objective methods for displaying projects without personal bias.

#### How often is the directory updated?

A set of custom Python scripts update the application details using the various git APIs and populate the lists with recently added applications every morning.

#### But Awesome-Selfhosted and AlternativeTo already exist?

selfh.st/apps should be considered supplemental and not a direct replacement for existing resources. It was created as an alternate view for discovering software using resources I had previously built for my own purposes while also organizing projects in way that feels a bit more intuitive and helpful for others.

#### Why does selfh.st/apps use tags and not categories?

The decision to use tags was intentional given the number of self-hosted projects that serve multiple purposes. It's easy to overlook projects after searching in the wrong category on other lists – tags should decrease the possibility of this happening on selfh.st/apps.

#### What is the criteria for adding a companion app?

For discovery purposes, the criteria for adding an app to the companion list primarily focuses on two conditions:

* Listed applications should extend the functionality of a self-hosted project or assist with the management of self-hosted software
* Listed applications should not be a core service of the original project

While this does present a bit of a gray area, the ultimate goal of the project is to help users discover applications they might not have otherwise come across when deploying a self-hosted project.

#### What do the last activity date colors represent?

Each project's last activity date has been color-coded based on the days since the project's latest commit as a way to differentiate between projects that are and aren't actively maintained.

The logic is loosely inspired by Awesome-Selfhosted:

* <b>Green</b>: Projects that have received a commit in the last 6 months
* <b>Yellow</b>: Projects that have received a commit in the last year
* <b>Red</b>: Projects that haven't received a commit in over a year

#### Why publish your own release feeds?

You may have noticed each project on selfh.st/apps is assigned a custom release feed that can be used to receive updates via RSS. I rely on these feeds heavily for the updates I include in [This Week in Self-Hosted](https://selfh.st/newsletter-signup/), which I find necessary to use over GitHub's built-in feeds given they don't provide a method for excluding non-stable and beta releases.

Behind the scenes, the Python update scripts referenced above retrieve the latest releases for each project and filter for stable releases using my own custom logic.

The feeds in selfh.st/apps are also a successor and replacement for the feeds previously released under the selfh.st/releases banner.