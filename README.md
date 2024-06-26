# minishell

*Minishell - As beautiful as a shell*

### Description

This project is about creating a fully functional shell from scratch, which should behave like bash, just with less features.
This was a group project consisting of [@mottjes](https://github.com/mottjes/) and [@me](https://github.com/frbeyer1).

### Features

- **Executable Search**: Minishell can execute the appropriate executable with a relative and a absolute path

- **Signal Handling**: Only one global variable is used to indicate received signals. This maintains the integrity of our main data structures.

- **Ctrl-C, Ctrl-D, Ctrl-\ Handling**: The shell behaves like bash with respect to these keyboard shortcuts:
    - Ctrl-C: Displays a new prompt on a new line.
    - Ctrl-D: Exits the shell.
    - Ctrl-\: No action taken.

- **Command History**

- **Quoting**: Minishell handles single quotes ('), preventing the interpretation of metacharacters within the quoted sequence. Double quotes (") do the same, except for the dollar sign ($).

- **Redirections**: The shell supports various redirections:
    - `<` redirects input.
    - `>` redirects output.
    - `<<` reads input until a specified delimiter, without updating history.
    - `>>` redirects output in append mode.

- **Pipes**: Our shell implements pipes (`|`), to get output from one command to the input of the next.

- **Environment Variables**: Minishell handles environment variables ($ followed by characters), expanding them to their corresponding values.

- **Exit Status**: `$?` expands to the exit status of the most recently executed foreground pipeline.

- **Built-in Commands**: Minishell supports the following built-in commands:
    - `echo` with the `-n` option
    - `cd` with relative or absolute paths
    - `pwd` with no options
    - `export` with no options
    - `unset` with no options
    - `env` with no options or arguments
    - `exit` with no options

For more detail: The subject pdf is inside of the project folder.

### Installation

Follow these steps to set up and run Minishell on your system:

1. **Clone the Repository**:

    ```sh
    git clone https://github.com/yourname/minishell.git
    ```

2. **Navigate to the Directory**:

    ```sh
    cd minishell
    ```

3. **Compile the Code**: Ensure you have `make` and `gcc` installed on your system.

    ```sh
    make
    ```

4. **Launch the Executable**:

    ```sh
    ./minishell
    ```
    
