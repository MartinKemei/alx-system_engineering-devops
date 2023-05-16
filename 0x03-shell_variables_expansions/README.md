---
#					0x03. Shell, init files, variables and expansions

## Expansions
   * Brace Expansion
   * Tilde expansion
   * Parameter expansion
   * Command substititution
   * Arithmetic expansion
   * Word splitting
   * Filename expansion

## Shell Arithmetic
   * Arithmetic expansion allows the evaluation of an arithmetic expression and the substitution of the result. The format for arithmetic expansion is:
   * `$((EXPRESSION))` _- double quotes inside parantheses is not treated specially._

## Variables
   * A variable is a character string to which we assign a value. The value assigned could be a number, text, filename, device, or any other type of data.
   
### Variable Types
    * Local Variables - A local variable is a variable that is present within the current instance of the shell.
    It is not available to programs that are started by the shell. They are set at the command prompt.

    * Environment Variables - Environment variables store data that's used by the operating system and other programs.
    For example, the PATH environment variable stores a list of directories where the operating system looks for executable files.
    By modifying the value of the PATH variable, you can specify additional directories to be searched for executable programs.

    * Shell Variables - A shell variable is a special variable that is set by the shell and is required by the shell in order to function correctly.
    Some of these variables are environment variables whereas others are local variables.

## Shell Initialization Files
   * System-wide configuration files include **/etc/profile** **/etc/bashrc** - All settings that you want
   to apply to all your users' environments should be in this file.
   * Individual user configuration files e.g _~/.bash_profile_  _~/.bash_login_  _~/.profile_  _~/.bashrc_
   &&  _~./bash_logout_

## The `alias` Command
   * An alias allows a string to be substituted for a word when it is used as the first word of a simple command.
   The shell maintains a list of aliases that may be set and unset with the alias and unalias built-in commands.
   Issue the alias without options to display a list of aliases known to the current shell.
>Functions are faster
   * Aliases are looked up after functions and thus resolving is slower.
   While aliases are easier to understand, shell functions are preferred over aliases for almost every purpose.
---
