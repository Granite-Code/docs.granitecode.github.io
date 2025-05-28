# Best Practices

This page provides information on how to get the most out of Granite.Code. It covers best practices for getting accurate and helpful responses, as well as a range of supplementary features that are included in Granite.Code.

Before you read this guide, you should be familiar with the main Granite.Code features, which are described in the [getting started tutorial](FIXME).

## Ask effective questions

Being able to chat with a local AI assistant is one of the main features offered by Granite.Code. The following guidelines are recommended for asking questions, in order to get the most useful responses:

* Be specific and precise - avoid broad or vague questions
* Break complex questions down into sections - you can use bullet points or sections
* If you want the answer in a specific format, describe it
* Ask follow-up questions to refine the response
* Provide the right context for your question (see below)

## Provide context for queries

By default, when making requests, an AI model has no awareness of the objects or environment that the query is related to - each response is based on general information that is available to the model, rather than specific information about the project or current focus. As a result, by default, requests to the model will return general responses.

Setting context allows you to provide additional information to the model about what you are asking about. Granite.Code allows a variety of different types of context to be specified for a given chat prompt:

* Code snippets: sections of the code that you can include in your query
* Codebase: to ask a question about an entire project of code
* Files: to ask questions about specific files
* Docs: to ask questions about a particular source of documentation
* Git diffs: to ask questions about a change in version control
* Folders: to ask questions about a directory of files

To add any of these types of context to a query, just type an **@** symbol, and a list of available context types will be shown. You can also click the **@** button in the chat prompt.

Examples of context-based queries you can ask include:

* TODO
* TODO
* TODO

## Ask about your codebase

Codebase is a special type of context, which can be used to ask questions about an entire project. This can be useful for learning how a project works, or finding ways to improve a project.

To ask a question about a codebase, you can either:

* Include **@Codebase** in your chat query, or
* Enter your query and click the **Ctrl⏎ @codebase** button, or
* Enter your query and press **Ctrl+⏎**

Examples of the type of question you can ask about a codebase include:

* TODO
* TODO
* TODO

## Add docs

In addition to being able to specify docs as the context for an individual query, it is also possible to add them as the context for all queries for a project. Adding doc in this way gives the models access to additional information about the technologies being used in your project, and allows it to give more accurate and helpful responses. When a docs website is added, the Granite.Code crawls the site and makes the content available locally to the AI model.

To add docs for your project:

* Click the docs button above the chat prompt
* Enter a title and URL for the docs site you want to make available
* Click add, and wait for indexing to complete

For more information on docs, see the [Continue documentation](https://docs.continue.dev/customize/deep-dives/docs).

## Make different types of edits

The Granite.Code context menu also includes a set of actions that can be performed on a selected code snippet, including:

* Fixing grammar and spelling mistakes
* Fixing errors in your code
* Optimizing code
* Adding code comments
