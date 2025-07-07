# Getting Started

This tutorial provides an introduction to the main features of Granite.Code. To complete it, we recommend that you have a running instance of VS Code with the Granite.Code extension enabled and setup.

## Setup your workspace

For the best experience, we recommend moving the Granite.Code chat to the secondary sidebar, so that it is visible alongside the code editor. To do this:

1. If the secondary side bar is not visible, show it by clicking the **Toggle Secondary Side Bar** button in the VS Code header.
2. Find the Granite.Code icon in the Activity Bar, then drag it to the secondary side bar header.

Granite.Code should now be located next to the VS Code editor area. With that done, let's explore Granite.Code's features.

## Ask questions

Granite.Code provides an interactive chat feature, which can be used to ask the Granite models questions.

To use the chat, either click on the "Ask anything" prompt, or use the **Command+L** / **Ctrl+L** keyboard shortcut. Then enter your question and press return.

The Granite.Code assistant can answer a range of question types, including general coding knowledge questions, advice on particular coding problems, learning best practices, and generating example code. Here are some example questions that you can try out:

1. What is an index in SQL and why is it important?
2. I have a CSV with the format: student_id, subject, test_score. How do I write a Python script to show average score per subject?
3. In React, I want to get information from the server when the component is created. How do I do that?

Once you have asked a question, you can ask follow-up questions about the model's response. For example:

 How can I handle loading and error states while fetching the data from the server?

## Ask about a code section

In addition to being able to ask general coding questions, you can also ask Granite.Code questions about sections of code. This can be useful for understanding how a piece of code works, or for asking how a section of code can be improved.

To ask a question about a code section:

1. Highlight the code you want to ask a question about.
2. Use the **Command+L** / **Ctrl+L** keyboard shortcut to start a chat, or use the **Granite.Code → Add Highlighted Code to Context** context menu item.
3. The code section will be shown in the chat prompt.
4. Enter a question about the code in the chat prompt, and press return.

You can try this using the code section below:

1. Copy the section to a Python file.
2. Highlight the code, and add it to the chat.
3. In the chat prompt, ask: "what sorting algorithm is this?".

```
def sorting_algorithm(x):
    for i in range(len(x)):
        for j in range(len(x) - 1):
            if x[j] > x[j + 1]:
                x[j], x[j + 1] = x[j + 1], x[j]
    return x
```

## Use Granite.Code to make changes

With Granite.Code it is possible to make code changes by giving editing instructions to the Granite models. An easy way to try this is to edit a code section:

1. In the editor, highlight the code you want to change.
2. Use the **Command+I** / **Ctrl+I** keyboard shortcut to add the code section to the prompt and switch to edit mode.
3. Describe how you want the code to be changed, then press return or click the **⏎ Enter** button.

You can try this with the code section below:

1. Copy the code section to the Python file you used earlier.
2. Highlight the code and add it to the chat.
3. In the chat, type "make this more readable", and press return.
4. New code will be shown in the editor, alongside the existing code.
5. Click Accept to accept the new code. Alternatively, you can use the **Command+Shift+Return** / **Ctrl+Shift+Return** keyboard shortcut to accept the changes.

```
def sorting_algorithm(x):
    for i in range(len(x)):
        for j in range(len(x) - 1):
            if x[j] > x[j + 1]:
                x[j], x[j + 1] = x[j + 1], x[j]
    return x
```

## Autocompletion

Granite.Code automatically makes suggestions as you type in the VS Code editor. Using the feature is simple: as you type you will see suggestions appear after the cursor. To accept a suggestion, just press the **Tab** key.

Let's use autocompletion to write assertions for the sorting algorithms from the previous examples:

* Copy the comment line below into the Python file that you used in the previous examples.
* Place the cursor at the end of the line, then press **Return**.
* When the suggestion is shown, press **Tab** to accept it.
* You can keep pressing **Tab** to generate additional assertions for the other sorting algorithms in the file.

```
# Basic assertion for sorting_algorithm...
```

## Next steps

This guide has introduced some essential Granite.Code features. However, there is much more to Granite.Code, including techniques which will allow you to get the most out of the features that have just been introduced. When you're ready, head over to the [best practices guide](https://docs.granitecode.github.io/best-practices) to learn more.
