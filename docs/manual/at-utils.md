# Utilities (at-utils)

The `at-utils` package is a bundle of utilities which aim to make application install and maintenance easier. 

### Quick navigation

<ul class="toc">
<li><a href="#/at-utils?id=install">install</a></li>
<li><a href="#/at-utils?id=mail-test">mail-test</a></li>
<li><a href="#/at-utils?id=register-super">register-super</a></li>
<li><a href="#/at-utils?id=update">update</a></li>
</ul>


## Running commands

All of the commands listed below are run using **npx**, which is a task runner utility which comes bundled with **npm**.

```bash
npx adapt-security/utils [COMMAND] [...OPTIONS] [ARGUMENTS]
```
> #### Arguments, options and flags - oh my! :astonished:
> There's a lot of terminology here which is confusing to anyone new to running commands in a command-line interface (CLI). If we look at the following as an example:
> ```bash
> npx adapt-security/at-utils install --no-ui --prerelease /home/user/adapt
> ```
> The 'command' element is the 'task' being run, and is first bit after `npx adapt-security/at-utils`, or in our case, `install`.
> 
> Anything that comes after the command is either an argument or an option; an argument is a mandatory value which the task requires to run, and an option is an optional value which usually modifies the task's behaviour in some way (options are noticable as being prefixed with `-` or `--`, and are also often referred to as 'flags').
>
> Looking at the above example again, `--no-ui` and `--prerelease` are both options, and `/home/user/adapt` is the only argument.

Below is a full reference of the commands available as part of **at-utils**.

***

## `install`

Installs the application into destination directory

#### Options

- `--branches --include-branches`: Whether to include git branches THIS COULD BE DANGEROUS
- `--dev --dev-mode`: Developer installation NOT FOR PRODUCTION
- `--drafts --include-drafts`: Whether to include draft releases THIS COULD BE DANGEROUS
- `--ignore-prereqs`: Whether to skip the prerequisites check. Warning this could result in expected errors
- `--prerelease --include-prereleases`: Whether to include prereleases THIS COULD BE DANGEROUS
- `--no-ui`: Run in CLI-only mode
- `--tag <tag>`: A specific git tag to use
- `-e --super-email <email>`: The admin user email address
- `-p --pipe-passwd`: Whether the admin password will be piped into the script

#### Arguments

- `destination`: The destination folder for the install


***

## `mail-test`

Sends a test email

#### Arguments

- `email`: Recipient email address for the test


***

## `register-super`

Registers a super user account

#### Options

- `-e --super-email <email>`: The admin user email address
- `-p --pipe-passwd`: Whether the admin password will be piped into the script


***

## `update`

Updates the application in destination directory

#### Options

- `--branches --include-branches`: Whether to include git branches THIS COULD BE DANGEROUS
- `--dev --dev-mode`: Developer installation NOT FOR PRODUCTION
- `--drafts --include-drafts`: Whether to include draft releases THIS COULD BE DANGEROUS
- `--ignore-prereqs`: Whether to skip the prerequisites check. Warning this could result in expected errors
- `--prerelease --include-prereleases`: Whether to include prereleases THIS COULD BE DANGEROUS
- `--no-ui`: Run in CLI-only mode
- `--tag <tag>`: A specific git tag to use
- `-d --dry-run`: Check for update without performing any update actions

#### Arguments

- `destination`: The destination folder for the source code


***

