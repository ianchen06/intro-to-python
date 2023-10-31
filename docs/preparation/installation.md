## Interactive Python Notebook

- [Google Colab](https://colab.research.google.com)

## Text Editor

- [Visual Studio Code](https://code.visualstudio.com/)

## Terminal

=== "MacOS"

    - Install iTerm2, a better Terminal for MacOS
        - [iTerm2](https://iterm2.com/)
    - Open iTerm2 Terminal
        - `Command + Space` and type `iterm`

=== "Windows"

    - Please refer to [Git installation instructions](#git-windows) below

## Python

=== "MacOS"

    - Install [Homebrew](https://brew.sh/) by running the following command in the Terminal
        ```bash
        /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
        ```
    - Install Python by running the following command in the Terminal
        ```bash
        brew install python
        ```
    - You can test your Python installation by running the following command in the Terminal
        ```bash
        python --version
        ```

=== "Windows"

    - Install Anaconda
        - [Anaconda](https://www.anaconda.com/products/individual)

## Git

=== "MacOS"

    - Git should be installed if you were able to install Homebrew from the previous step
    - You can test your Git installation by running the following command in the Terminal
        ```bash
        git --version
        ```

=== "Windows"
    <a name="git-windows"></a>

    - Install Git by following the instructions in the following link
        - [Installing Git Command Line - UW CSE154](https://courses.cs.washington.edu/courses/cse154/21su/resources/assets/vscode-git-tutorial/windows/index.html#installinggitcommandline)

    - Configure VSCode Terminal to use Git Bash by following the instructions in the following link
        - [Configuring VSCode to use Git Bash - UW CSE154](https://courses.cs.washington.edu/courses/cse154/21su/resources/assets/vscode-git-tutorial/windows/index.html#installandsetupvscode)
        - In the future, you can open Git Bash by pressing `Ctrl + Shift + ~`

        !!! note

            This is what I mean when I mention "Terminal" in the future

    - You can test your Git installation by running the following command in the Git Bash
        ```bash
        git --version
        ```