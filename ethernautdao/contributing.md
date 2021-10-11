---
description: How to contribute to the Ethernaut DAO documentation
---

# Contributing

You want to contribute to the documentation but you don't know where to start ? You are at the right spot ! This page should give you all the necessary information to contribute efficiently to our documentation.

First off, regardless of the time you have or your experience you can provide meaningful contribution to the documentation. Here are some examples depending on the time you have:

* ⏲️: Add a resource, correct a typo, [deduplicate information](contributing.md#favor-links-to-repetition)
* ⏲️⏲️: Rewrite a paragraph, add information to an existing page, create an issue for an improvement, propose a content template
* ⏲️⏲️⏲️: Propose a new content, write an activity report, take an issue

If you really have not much time but you have found a broken link, an error in the documentation or have a minor suggestion, we'd still like to hear from you. Drop us a message on our [discord](https://discord.gg/RQ5WYDxUF3)!

## Structure

The documentation is structured around top-level directories that map the different [content types](contributing.md#content-types) of the documentation and create a hierarchical structure between contents. These top-level directories appear as the sections of the documentation on our Gitbook page. 

{% hint style="warning" %}
Subdirectories to top-level directories will be seen as a content with different levels of nesting and not as subsections.
{% endhint %}

If you want to have multiple levels of nesting for your content (hence having multiple files), you can create subdirectories in a top-level directory with a `README.md` file at the root of this subdirectory. The README file will be the top-level content of the subdirectory.

For example, if you want to have a meeting reports page with separate pages for each report you could create the following tree structure :

```
├── ethernautdao // top-level section
│   └── meetings
│       ├── first-meeting.md
│       └── README.md
```

In this case, the `README.md` would contain a list of the different meetings and at least a [description of the page](contributing.md#content-templates).

There are no hard limits on the nesting of pages but you should avoid having more than 3 levels.

### Summary

The `SUMMARY.md` file at the root of the page is - as its name suggests - the summary. It is automatically edited when you are using Gitbook.

{% hint style="warning" %}
If you are modifying content directly by making commits on the repository, make sure to edit the SUMMARY.md file in order to reflect your changes.
{% endhint %}

### Naming

When creating a new file or directory please follow these rules (some are automatically enforced when you use Gitbook) :

* Use only lowercase letters
* Do not use special characters and spaces
* Use hyphens as a word separation
* Use a filename as close as possible as the title of the page but if it is too long shorten it

### Content types

As this documentation aims to be comprehensive it is important to organize the content well so it is easy to find the right information and easy to add information. The more the documentation grows the more this becomes important.

The documentation is organized around topics that enforces the structure of the documentation. Whether you use/modify the documentation through Gitbook or directly via Git, you will find the same structure.

Currently we have the following categories :

* **EthernautDAO**: Content that documents the DAO activity (e.g. Improvement Proposal Reports, Pairing Reports, etc)
* **Educational Resources**: Any type of external resources that can provide good information on any topics around Ethereum and Solidity development. Classified by level of knowledge.

You want to provide content and no category fits? Feel free to propose a new content type by creating an issue on the GitHub repository.

## Style guide

In order to have a consistent documentation we'd like you to follow the recommendations/conventions that are underlined below.

#### Markdown

All the documentation is written in [Markdown](http://commonmark.org/help/). You can either edit the documentation via any text editor or directly on Gitbook (an account & the correct role is needed). 

Regardless on how you plan to edit the documentation you should also check Gitbook's [markdown documentation](https://docs.gitbook.com/editing-content/markdown) as there are some specific syntax that could be useful (e.g. hint boxes).

Embedded HTML is supported but should be avoided. If there are cases where you think it should be used, make an improvement proposal.

#### Code style

To ensure readability and consistency across the documentation, embedded code should also follow style convention:

* Solidity: use the [official style guide](https://docs.soliditylang.org/en/latest/style-guide.html). 

If there are no convention for your favorite language do not hesitate to propose a documentation improvement.

#### Media

Adding an image can be done using the proper Markdown syntax, either using an external link or a direct reference to the path of the image. Videos files can also be added to pages as Gitbook supports [embedded content](https://docs.gitbook.com/editing-content/embeds), do not upload videos to the repository.

When adding image to the documentation :

1. File must not exceed 150 KB.
2. All files must be in the`.gitbook/assets` at the root of the documentation
3. File reused across multiples sections must be in the `common`subdirectory
4. File specifically used in one section must be in the subdirectory with the same name as the section
5. Following [naming](contributing.md#naming) conventions use clear names describing the content of the media

As the assets directory is at the root of the documentation, to add a link to the image the path must be relative : if you add a page in the section `activity` the image link will be`![]`(`../.gitbook/assets/filename.jpeg)`

If you are using Gitbook you can directly add an image using the [insert palette](https://docs.gitbook.com/editing-content/rich-content/with-insert-palette).

#### Content templates

Content templates are markdown files that provides the basic structure for the different content types of the documentation. Creating a new page from a template will allow you to easily ensure that you are using the right structure for your page.

All templates are located in the `templates` hidden folder. 

We currently provide the following templates :

* **Basic Template** \[`basic-page.md`]: as the name suggests, it contains the very minimal elements that are required for a page.

If there are no template for a specific content type, you can propose one by following our [improvement processes](contributing.md#process). As there are some minimal requirements for a page, make sure to use our basic template as a start.

### Writing style

Even if this documentation is not a technical software documentation trying to write in a technical style that is concise, clear and objective should be what we aim for. Here are some general recommendations that you should follow when writing:

* Be as clear as possible to avoid ambiguity
* Use the same word for the same concept throughout a page. This can seems obvious but sometimes using what appears to be synonyms can cause ambiguity.
* When using acronyms provide at least a link to a glossary or if it is the first time it appears on the page, spell it out.
* A good example can help understanding a complex subject, so do not hesitate to provide some. They can take many form: schema, sample code or even a small exercise.

As this documentation targets multiple level of knowledge you should always have this target in the back of your mind when you write. 

For example, if you write for a beginner, do not hesitate to provide comprehensive explanations even for concepts that seem obvious. Some of the readers may be well versed in computer science but may not be so knowledgeable on the Ethereum ecosystem, so keep it in mind.

## Process

Ready to propose an improvement ? Depending on the type of improvement you want to make, you should follow these processes. You can propose an improvement either through Gitbook or Github, but the process is roughly the same.

We can define two category of improvements :

* **Small** : These changes do not necessarily require a discussion and the process is straightforward. (e.g. typo correction, paragraph improvement, adding a resource, etc)
* **Big** : These changes can have an important impact on the documentation and should therefore be discussed before having to work on it. (e.g. documentation structure change, adding a new section, changing the structure of a page, propose a new process, etc.)

### Github

Using this method is the most straightforward way of proposing a modification for the documentation as it does not require the creation  of an account by the documentation admins. Anyone with a Github account can propose a pull request or create an issue.

#### Small improvement

1. Fork the documentation repository
2. Create a new branch following the branche naming convention
3. Make the changes and commit them
4. Create a pull request on the documentation repository

#### Big improvement

1. Create an issue on the documentation repository using the improvement template
2. If you want to add a proposal to your issue you can follow steps 1-3 of the small improvement and put a link to your branch in the issue body
3. If the issue is accepted you can create a pull request from a new branch or from your previously created branch

Once the PR is created the code review will start and after it, the branch will be merged if it meets all the requirements.

### Gitbook

Even if there are [roles](https://docs.gitbook.com/collaboration/team-management/setting-up-permissions) on Gitbook, account with writing permission can merge their modifications without any prior review. Hence, to be able to contribute via this platform you must must be part of the documentation team.

If you want to join us, feel free to drop a message on the `#educational-material`channel. Note that if we'll be easier for us to consider you for a writer account if you've already contributed to the documentation via Github. 

#### Small improvement

Except if you have doubts or want to have a discussion on these small improvements, it should be straightforward :

1. Edit the page
2. Save your draft. At this step, if you want you can always ask on of the team member to review the changes and add comments.
3. Merge

The changes will be made on Gitbook and synced with Github. If there are conflicts please refer to the [documentation](https://docs.gitbook.com/collaboration/conflict-resolution).

#### Big improvement

Before adding or making big changes or improvements to the documentation, we recommend that you double-check and share your thoughts and ideas with the community in the `#educational-material` channel. Most likely, other community members will be happy to assist you. 

Further details are to be determined as we go. If you have ideas or suggestions, let us know!



{% hint style="info" %}
As always if you have any doubts or questions around the contribution to the documentation, do not hesitate to contact us on our discord channel `#educational-material`
{% endhint %}
