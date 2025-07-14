# Best Practices

This page provides information on how to get the most out of Granite.Code. It covers best practices for getting accurate and helpful chat responses, as well as supplementary options which make Granite.Code's features even more powerful.

Before you read this guide, you should be familiar with the main Granite.Code features, which are described in the [getting started tutorial](getting-started).

## Asking effective questions

Being able to chat with a local AI model is one of the main features offered by Granite.Code. When asking questions or creating prompts for an AI model, there are a number of best practices which will help you to get the best responses possible:

* Always be as specific and precise as possible, and avoid broad or vague questions.
* If you are asking a complex question, consider breaking it down into sections. Questions can include paragraphs and lists of information, which can be useful to keep them organized. This will make it easier for the model to interpret what you are asking.
* If you want the model to provide an answer in a specific format, say what it is. For example, you could ask for a list of short points, or a code example, or you could ask for references for further reading.
* If a question doesn't give you the answer you want, use follow-up questions to refine or amend it.

Remember that asking AI models questions is a skill that gets better with practice.

## Providing context for queries

Most questions have a context that they are related to. In the coding world that context can be a project, a file, a programming language, a platform, or code section. However, by default an AI model has no information about that context: its response will be based only on the prompt it receives and the general information that it already has access to.

This is where context comes in. Context allows you to feed additional information to the model, so that it has additional knowledge about the question you are asking. Granite.Code allows a variety of different types of context to be specified for a question. These include:

* `@Files`: adds specific files
* `@Folder`: adds a specific folder
* `@Codebase`: adds all the files in the current project
* `@Terminal`: adds the contents of the VS Code terminal
* `@Git Diff`: adds the Git changes in the current branch
* `@Problems`: adds data from the VS Code problems panel

To use any of these types of context to a question, just type an **@** symbol in the chat, and a list of available context types will be shown. You can also click the **@** button in the chat prompt.

Some examples of questions you can ask that make use of additional context:

* Please summarize @sort.js
* How do I fix the syntax errors in @sort.js @Problems
* When I ran ``git pull`` I got weird errors. Please explain @Terminal
* Please write a commit message for the current @Git Diff

## Using docs

`@Docs` is another powerful type of context in Granite.Code, which can be used to ask questions that have a documentation website as its context.

What makes `@Docs` a little different is that it must be set up prior to use. To do this:

1. Click the docs button above the chat prompt.
2. Enter a title and URL for the docs site you want to make available.
3. Click add, and wait for indexing to complete.

Once this has been done you can enter `@Docs` in the chat prompt to use a docs site in a question.

For more information on the docs context provider, see the [Continue documentation](https://docs.continue.dev/customize/deep-dives/docs).

## Making different types of edits

Granite.Code's edit feature was introduced in the [getting started tutorial](getting-started), where we saw how code can be easily made more readable. There are many other types of changes that can be made with Granite.Code. Some of these are available in the Granite.Code context menu in the code editor. This includes actions to:

* Fix grammar and spelling mistakes
* Fix code errors
* Optimize code
* Add code comments

These menu items are a great way to access some of Granite.Code's editing features. They are also a great example of the different possibilities of the editing feature.

## Using keyboard shortcuts for common contexts

Granite.Code provides keyboard shortcuts for common contexts, which allow those contexts to be quickly used without needing to manually specify them.  The main shortcuts to know are:

| Context      | Mac | Windows/Linux |
|--------------|-----|---------------|
| Current file | Option+Return  | Alt+Return  |
| Codebase     | Command+Return | Ctrl+Return |
