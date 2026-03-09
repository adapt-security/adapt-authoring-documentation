# Utilities (at-utils)

The `at-utils` package is a bundle of utilities which aim to make application install and maintenance easier. 

### Quick navigation

<ul class="toc">
<li><a href="#/at-utils?id=deps-check">deps-check</a></li>
<li><a href="#/at-utils?id=deps-gen">deps-gen</a></li>
<li><a href="#/at-utils?id=install">install</a></li>
<li><a href="#/at-utils?id=mail-test">mail-test</a></li>
<li><a href="#/at-utils?id=register-super">register-super</a></li>
<li><a href="#/at-utils?id=release-notes">release-notes</a></li>
<li><a href="#/at-utils?id=update">update</a></li>
<li><a href="#/at-utils?id=version-check">version-check</a></li>
</ul>


## Running commands

All of the commands listed below are run using **npx**, which is a task runner utility which comes bundled with **npm**.

```bash
npx adapt-security/at-utils [COMMAND] [...OPTIONS] [ARGUMENTS]
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

## `deps-check`

Checks dependencies and peerDependencies against source code analysis

#### Options

- `--recursive`: Check all AAT modules in child directories
- `--versions-only`: Only check dependency versions are up to date (skip code analysis)


***

## `deps-gen`

Generates correct dependencies and peerDependencies from source code analysis

#### Options

- `--recursive`: Process all AAT modules in child directories
- `--write`: Write changes to package.json files
- `--versions-only`: Only update dependency versions (skip code analysis)


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
- `--v --verbose`: Include extra debug messages
- `-e --super-email <email>`: The admin user email address
- `-p --pipe-passwd`: Whether the admin password will be piped into the script

#### Arguments

- `destination`: The destination folder for the install


***

## `mail-test`

Sends a test email

#### Options

- `--v --verbose`: Include extra debug messages

#### Arguments

- `email`: Recipient email address for the test


***

## `register-super`

Registers a super user account

#### Options

- `-e --super-email <email>`: The admin user email address
- `--ignore-prereqs`: Whether to skip the prerequisites check. Warning this could result in expected errors
- `-p --pipe-passwd`: Whether the admin password will be piped into the script
- `--v --verbose`: Include extra debug messages


***

## `release-notes`

Fetches GitHub release notes for all changed dependencies since the last git tag

#### Options

- `--cwd <path>`: Path to the git repository
- `--json`: Output results as JSON


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
- `--v --verbose`: Include extra debug messages
- `-d --dry-run`: Check for update without performing any update actions
- `--patch-only`: Only show patch releases
- `--minor-only`: Only show patch and minor releases

#### Arguments

- `destination`: The destination folder for the source code


***

## `version-check`

Compares dependency versions between the last git tag and now, and recommends a semver bump

#### Options

- `--cwd <path>`: Path to the git repository
- `--json`: Output results as JSON


***

