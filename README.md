## Jekyll ANU Website Template Repo

**Note**: this template repo is still under construction, and is frequently
broken as we try new (and better) ways of doing things. If you're looking to
create a new Jekyll ANU website right now, then talk to
[Ben](mailto:ben.swift@anu.edu.au) or ask in the [CECS Jekyll web support
channel](https://teams.microsoft.com/l/channel/19%3aIcnInMyxTJ26Ik8FrUs9SefrG_9seawpDu95NmKwiIE1%40thread.tacv2/General?groupId=dab190b1-14f2-40cf-b384-ee00c63d2019&tenantId=e37d725c-ab5c-4624-9ae5-f0533e486437)
for assisstance.

This is a template repo for creating webpages using the new Jekyll ANU theme.
You may fork it/copy it into your own webpage repo and adapt to your needs. This
template repo is sort of like the 'Course In a Box' repo that existed for an
older version of the theme. You may use it for any type of page, including but
not limited to:

- course pages, e.g. [COMP2300](https://cs.anu.edu.au/courses/comp2300/)
- research group pages, e.g. the [c/c/c studio](https://cs.anu.edu.au/code-creativity-culture/)
- School websites, e.g. [School of Cybernetics](https://cybernetics.anu.edu.au/)

The aim of this template is to ease the transition process as much as possible,
with the ideal process being as follows:

1. copy/fork this template, modify the structure and page names to fit your
   needs, then copy over the content from your old page (or create it fresh if
   it does not exist), adapting to any new requirements or formatting that the
   new theme permits

2. if you require any advanced functionality, such as additional features, more
   formatting options, or a slightly different look, this can be done through a
   few different ways, the easiest one being through the `_includes` folder (you
   can explore the `_includes` folder in this repo if you want to see concrete
   examples), which allows you to bring in `html` documents, or override
   existing ones in the theme

---

## Documentation

Getting setup/started with the new theme can be a little bit difficult. We have put together documentation
over at [CECS Jekyll theme docs](https://cs.anu.edu.au/docs/gitlab-pages/). If there is any information missing
or you would like additional help, please do not be afraid to contact the CECS Jekyll web support teams channel/email (linked above).

---


## Directories Explanation

The directories in the the Jekyll ANU website template repo (and all webpages using the new ANU Jekyll theme) are split into two groups:
 - Theme/Jekyll required
 - Content directories

The `assets` directory is the only one not starting with an underscore (`_`).

The directories required by the theme/Jekyll are:
 * `_sass`
 * `_layouts`
 * `_includes`
 * `assets`

Technically you do not need any of these directories as they are in the theme as well, and files included in these directories will either
override files of the same name in the theme, or just be added to the theme. Thus if you have no custom includes, layouts or sass files, you can
delete these directories. You will probably need the `/assets/` directory though.

Then for every collection of pages you have (essentially every 'tab' in the top menu bar) is its own directory as well.
I.e. the template website has 'About', 'Lectures', 'Labs', 'Assessments', and 'Resources' collections.

You can find an exact list of all the collections in the `_config.yml` file, under the `collections:` key.

Each collection directory also starts with an underscore (`_`), thus the following directories in the template are for collections (content):
 * `_about`
 * `_assessments`
 * `_labs`
 * `_lectures`
 * `_resources`

Collections will usually have another `index.md` file in them as the landing page for that collection. I.e. if you click on the `About` top bar option, you are taken to the { base-url }/about/ page, which is dictated by the `_about/index.md` file. Other files that may be in the drop down menu or linked to from the `index.md` page will also be placed inside that collection.

## Licence

MIT
