---
description: >-
  Discover the benefits of Fish shell and the differences compared to Bash and
  Zsh to make your command-line experience even more efficient.
---

# 📜 Fish: A modern and powerful alternative to Bash and Zsh

The "shell" is the interface that allows users to interact with a computer's operating system. In Linux environments, the most common shells are Bash and Zsh. However, another option that has gained popularity in recent years is the "Fish Shell" (or simply "Fish"), which offers advanced auto-completion and syntax highlighting features to make the command line experience more user-friendly.

Fish offers several benefits over traditional shells, such as the ability to auto-complete based on context, suggestions for commands and options based on the user's usage history, and the ability to easily configure shortcuts and custom functions. These features can greatly increase a user's productivity and efficiency when working on the command line.

In this article, we will explore in more detail the benefits of the Fish shell and the main differences between it and the traditional Bash and Zsh shells. We will also discuss why choosing the Fish shell as the main shell can be a good choice for Linux users who want to streamline their workflow and take full advantage of the advanced features offered by Fish.

## The Fish Shell

In my opinion, the Fish shell, also known as the "**Friendly Interactive Shell**", is the most user-friendly and interactive shell available for Linux environments. Compared to traditional shells like Zsh and Bash, Fish offers a high level of customizability and numerous features, including uniform syntax, impressive tab completion and syntax highlighting, and a user-friendly interface.&#x20;

Furthermore, it includes an excellent runtime help system, making it easy for users to get started and use effectively.

It is important to note that Fish shell is not POSIX compliant, but this is actually a deliberate design choice rather than a limitation. Instead, Fish shell prioritizes ease of use and modern functionality, making it an excellent choice for users who prioritize productivity and efficiency.

### Customizing

One of the primary reasons that I made the switch from Zsh to Fish shell was due to my experience with **Oh My Zsh**. While I initially enjoyed using Oh My Zsh to add plugins and themes to my Zsh shell, I eventually found that it made my shell feel too heavy and ultimately worsened my experience.

In contrast, Fish shell offers a highly customizable environment that allows users to easily tailor their command line experience without the need for heavy add-ons like Oh My Fish. The built-in customization features of Fish are fast and straightforward, enabling users to quickly and easily configure their shell to their individual needs.

Moreover, the ease and speed of customization in Fish, coupled with its support for plugins, made my experience with the shell much more enjoyable. The available plugins can add additional functionality to Fish, such as syntax highlighting for various programming languages, enabling the shell to offer an even more streamlined and efficient command line experience for users.

### Syntax Highlighting

Fish shell provides a rich and powerful syntax highlighting, which interprets the command line in real-time as the user types, and uses colors to provide feedback. This feedback includes detecting potential errors and marking them in red by default.

Before hitting enter, Fish also shows whether the command or directory to be searched exists, which helps users identify any typing mistakes beforehand. This feature greatly facilitates command parsing and error detection.

In addition to highlighting misspelled commands and options, Fish can also detect errors such as non-existing files and mismatched parentheses and quotes. It further enhances user experience by highlighting matching quotes and parentheses in different colors.

Overall, Fish's syntax highlighting feature is not only functional but also aesthetically pleasing due to its colorful display.

### Config

In addition to its impressive customization features, Fish shell is also highly intuitive when it comes to configuration. Unlike other shells, which often require users to modify configuration files manually, Fish offers a user-friendly web interface that allows users to make changes to color schemes, functions, and other customization options graphically.

> _OBS: I personally still prefer to manually make changes to the configuration files xd_

To access the Fish configuration web interface, users can simply type the following command in the Fish shell:

```sh
fish_config
```

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption><p>Web-based config interface</p></figcaption></figure>

This command will launch the Fish configuration interface in a user's default web browser, providing an easy and intuitive way to modify Fish shell settings and preferences. With this powerful and user-friendly interface, configuring Fish to meet your specific needs has never been easier.

### Smart suggestions

The Fish Shell auto-suggestions are based on a machine learning model that uses convolutional neural networks. When the user types a command, the terminal usage history is analyzed to identify patterns of behavior and predict the most likely command based on the current context. The model is trained on a large-scale dataset, which includes information about the most common commands, their options and arguments, and the usage history of real users.

The auto-suggestions model is updated in real-time as the user types, allowing the suggestions to be adjusted based on changes in context. Additionally, the model also takes into account the current directory, which helps suggest more relevant commands for the current task.

To ensure user privacy, the Fish Shell auto-suggestions are executed locally on the user's computer and do not send data to external servers. Furthermore, the model is periodically updated, ensuring that the suggestions are always up-to-date and accurate.

### Abbreviations

The Fish Shell <mark style="color:blue;">`abbr`</mark> feature is a powerful tool for customizing and abbreviating commands, options, and arguments in the terminal. Abbreviations can be defined for frequently used commands, allowing the user to type shorter versions of the commands without sacrificing functionality.

The <mark style="color:blue;">`abbr`</mark> feature is based on a simple syntax, where the abbreviation is defined as a string and its corresponding command is specified. For example, the command <mark style="color:blue;">`ls -la`</mark> could be abbreviated as <mark style="color:blue;">`lla`</mark>. When the user types <mark style="color:blue;">`lla`</mark> in the terminal, Fish Shell will automatically expand it to <mark style="color:blue;">`ls -la`</mark>.

In addition to commands, options and arguments can also be abbreviated. For example, the "<mark style="color:blue;">`-a`</mark>" option of the <mark style="color:blue;">`ls`</mark> command could be abbreviated as <mark style="color:blue;">`-`</mark>. When the user types <mark style="color:blue;">`ls -`</mark> in the terminal, Fish Shell will suggest the <mark style="color:blue;">`-a`</mark> option as an auto-completion suggestion.

The "abbr" feature can be customized by the user to fit their specific needs and preferences. Abbreviations can be defined in the Fish Shell configuration file, which allows for easy management and sharing across multiple machines.

### Conclusion

Ultimately, the **Fish** shell is a highly customizable and powerful option that offers a smoother and more productive command line experience for users who demand high efficiency and productivity in their daily tasks.

I will make my fish settings available at [this link](https://github.com/devilgothies/dotfiles), where I keep a repository with some program settings that I use on a daily basis in my development/research environment.
