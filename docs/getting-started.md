# Getting Started

This tutorial provides an introduction to the main features of Granite.Code. To complete it, we recommend that you have a running instance of VS Code with the Granite.Code extension enabled.

## Setup your workspace

For the best experience, we recommend moving Granite.Code chat to the secondary sidebar, so that it is visible alongside the code editor. To do this:

* If the secondary side bar is not visible, show it by clicking the **Toggle Secondary Side Bar** button in the VS Code header.
* Find the Granite.Code icon in the Activity Bar, then drag it to the secondary side bar header.

Granite.Code should now be located next to the VS Code editor area. With that done, let's explore Granite.Code's features.

## Ask questions

Granite.Code provides an interactive chat feature, which can be used to ask the Granite models questions.

To use the chat, either click on the "Ask anything" prompt, or use the **Ctrl+L** keyboard shortcut. Then enter your question and press return.

The Granite.Code assistant can answer a range of question types, such as:

* TODO
* TODO
* TODO

You can try some of these out now, to see what kind of responses you get.

Once you have asked a question, you can ask follow-up questions. For example, TODO.

## Ask about a code snippet

In addition to being able to ask general coding questions, you can also ask Granite questions about sections of code. This can be useful for understanding how a piece of code works, or for asking how a part of the code can be improved.

To ask a question about a code snippet:

* Highlight the code you want to ask a question about.
* Use the **Ctrl+L** keyboard shortcut to start a chat, or use the **Granite.Code > Add Highlighted Code to Context** context menu item.
* The code snippet will be shown in the chat prompt.
* Enter a question about the code in the chat prompt, and press return.

You can try this using the code snippet below:

* Copy the snippet to a Python file.
* Highlight the code, and add it to the chat.
* In the chat prompt, ask: "what sorting algorithm is this?".

```
def sorting_algorithm(x):
    for i in range(len(x)):
        for j in range(len(x) - 1):
            if x[j] > x[j + 1]:
                x[j], x[j + 1] = x[j + 1], x[j]
    return x
```

## Use Granite.Code to make changes

Granite.Code allows making code changes by giving editing instructions to the Granite models. An easy way to try this is to edit a code snippet:

* In the editor, highlight the code you want to change.
* Use the **Ctrl+E** keyboard shortcut to add the snippet to the prompt and switch to edit mode.
* Write how you want the code to be changed, then press return or click the **⏎ Enter** button.

You can try this with the code snippet below:

* Copy the snippet to a Python file.
* Highlight the code and add it to the chat.
* In the chat, enter "make this more readable", and press return.

Granite.Code will suggest... TODO

```
def sorting_algorithm(x):
    for i in range(len(x)):
        for j in range(len(x) - 1):
            if x[j] > x[j + 1]:
                x[j], x[j + 1] = x[j + 1], x[j]
    return x
```

## Autocompletion

Granite.Code makes suggestions, which are shown after the cursor as you type. To accept a suggestion that is being shown, press the **Tab** key.

To try out autocomplete:

* Copy the snippet below into a Python file.
* Place the cursor at the end of the line, then press **Enter**.
* When the suggestion is shown, press **Tab**.

```
# Basic assertion for sorting_algorithm...
```

## Next steps

This tutorial covers just a few of the basic Granite.Code features. Once you have got the hang of them, it is time to [learn how to get more from Granite.Code](FIXME).
