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

If you want to have multiple levels of nesting for your content \(hence having multiple files\), you can create subdirectories in a top-level directory with a `README.md` file at the root of this subdirectory. The README file will be the top-level content of the subdirectory.

For example, if you want to have a meeting reports page with separate pages for each report you could create the following tree structure :

```text
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

When creating a new file or directory please follow these rules \(some are automatically enforced when you use Gitbook\) :

* Use only lowercase letters
* Use hyphens as a word separation
* Use a filename as close as possible as the title of the page but if it is too long shorten it

### Content types

As this documentation aims to be comprehensive it is important to organize the content well so it is easy to find the right information and easy to add information. The more the documentation grows the more this becomes important.

The documentation is organized around topics that enforces the structure of the documentation. Whether you use/modify the documentation through Gitbook or directly via Git, you will find the same structure.

Currently we have the following categories :

* **EthernautDAO**: Content that documents the DAO activity \(e.g. Improvement Proposal Reports, Pairing Reports, etc\)
* **Educational Resources**: Any type of external resources that can provide good information on any topics around Ethereum and Solidity development. Classified by level of knowledge.

You want to provide content and no category fits? Feel free to propose a new content type by creating an issue on the GitHub repository.

## Style guide

In order to have a consistent documentation we'd like you to follow the recommendations/conventions that are underlined below.

#### Markdown

All the documentation is written in [Markdown](http://commonmark.org/help/). If you are directly editing the documentation with Gitbook, you should check their [documentation](https://docs.gitbook.com/editing-content/markdown).

#### Code style

To ensure readability and consistency across the documentation, embedded code should also follow style convention:

* Solidity: use the [official style guide](https://docs.soliditylang.org/en/latest/style-guide.html). 

If there are no convention for your favorite language do not hesitate to propose a documentation improvement.

#### Media

Adding an image can be done using the proper Markdown syntax, either using an external link or a direct reference to the path of the image. In the latter case, the file must be added in the `.gitbook/assets/` hidden folder at the root of the documentation. Hence you will add a link to the image relative to where the documentation page is in the path. If you add a page in the section `activity` the image link will be`![]`\(`../.gitbook/assets/filename.jpeg)`

If you are using Gitbook you can directly add an image using the [insert palette](https://docs.gitbook.com/editing-content/rich-content/with-insert-palette).

#### Content templates

We currently do not have templates for each content type \(👋 help needed\). But each file should at least contain a description at the top of the file as follows:

```text
---
description: This is the description of the page
---
```

### Writing style

Even if this documentation is not a technical software documentation trying to write in a technical style that is concise, clear and objective should be what we aim for. Here are some general recommendations that you should follow when writing:

* Be as clear as possible to avoid ambiguity
* Use the same word for the same concept throughout a page. This can seems obvious but sometimes using what appears to be synonyms can cause ambiguity.
* When using acronyms provide at least a link to a glossary or if it is the first time it appears on the page, spell it out.
* A good example can help understanding a complex subject, so do not hesitate to provide some. They can take many form: schema, sample code or even a small exercise.

As this documentation targets multiple level of knowledge you should always have this target in the back of your mind when you write. 

For example, if you write for a beginner, do not hesitate to provide comprehensive explanations even for concepts that seem obvious. Some of the readers may be well versed in computer science but may not be so knowledgeable on the Ethereum ecosystem, so keep it in mind.

## Process

Ready to propose an improvement ? Depending on the type of improvement you want to make, you should follow these processes.

### Small improvement

These changes should not require a discussion and can be proposed directly as a PR on GitHub.

Example: typo correction, paragraph improvement, adding a resource

### Big improvement

These changes can have an important impact on the documentation and should therefore be discussed before having to work on it.

Example: documentation structure change, adding a new section, changing the structure of a page, propose a new process, etc.

As always if you have any doubts or questions around the contribution to the documentation, do not hesitate to contact us on our discord channel `#educational-material`

