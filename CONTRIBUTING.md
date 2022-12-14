Hello! Thank you for choosing to help contribute to one of the SendGrid open source projects. There are many ways you can contribute and help is always welcome.  We simply ask that you follow the following contribution policies.

- [Improvements to the Codebase](#improvements-to-the-codebase)
- [Understanding the Code Base](#understanding-the-codebase)
- [Testing](#testing)
- [Style Guidelines & Naming Conventions](#style-guidelines-and-naming-conventions)
- [Creating a Pull Request](#creating-a-pull-request)
- [Code Reviews](#code-reviews)

<a name="improvements-to-the-codebase"></a>
## Improvements to the Codebase

We welcome direct contributions to the smtpapi-csharp code base. Thank you!

### Development Environment ###

#### Install and Run Locally ####

##### Prerequisites #####

- .NET version 4.5.2
- Microsoft Visual Studio Community 2015 or greater

##### Initial setup: #####

```bash
git clone https://github.com/sendgrid/smtpapi-csharp.git
```

Open `smtpapi-csharp/Smtpapi/SendGrid.SmtpApi.sln`

### Environment Variables

First, get your free SendGrid account [here](https://sendgrid.com/free?source=smtpapi-csharp).

Next, update your Environment (user space) with your SENDGRID_USERNAME and SENDGRID_PASSWORD.

##### Execute: #####

See the [examples folder](Smtpapi/Example) to get started quickly.

<a name="understanding-the-codebase"></a>
## Understanding the Code Base

<!---optionally provide a brief summary explaining the architecture of the code-->

**/Smtpapi Example**

Working examples that demonstrate usage.

**/Smtpapi/HeaderTests**

Unit tests

**/Smtpapi/Smtpapi**

Source code

<a name="testing"></a>
## Testing

All PRs require passing tests before the PR will be reviewed.

All test files are in the [`Smtpapi/HeaderTests`](Smtpapi/HeaderTests) directory.

For the purposes of contributing to this repo, please update the [`TestHeader.cs`](Smtpapi/HeaderTests/TestHeader.cs) file with unit tests as you modify the code.

From the Visual Studio menu: `Tests->Run->All Tests`

<a name="style-guidelines-and-naming-conventions"></a>
## Style Guidelines & Naming Conventions

Generally, we follow the style guidelines as suggested by the official language. However, we ask that you conform to the styles that already exist in the library. If you wish to deviate, please explain your reasoning. In this case, we generally follow the [C# Naming Conventions](https://msdn.microsoft.com/library/ms229045(v=vs.100).aspx) and the suggestions provided by the Visual Studio IDE.

## Creating a Pull Request<a name="creating-a-pull-request"></a>

1. [Fork](https://help.github.com/fork-a-repo/) the project, clone your fork,
   and configure the remotes:

   ```bash
   # Clone your fork of the repo into the current directory
   git clone https://github.com/sendgrid/smtpapi-csharp
   # Navigate to the newly cloned directory
   cd smtpapi-csharp
   # Assign the original repo to a remote called "upstream"
   git remote add upstream https://github.com/sendgrid/smtpapi-csharp
   ```

2. If you cloned a while ago, get the latest changes from upstream:

   ```bash
   git checkout <dev-branch>
   git pull upstream <dev-branch>
   ```

3. Create a new topic branch (off the main project development branch) to
   contain your feature, change, or fix:

   ```bash
   git checkout -b <topic-branch-name>
   ```

4. Commit your changes in logical chunks. Please adhere to these [git commit
   message guidelines](http://tbaggery.com/2008/04/19/a-note-about-git-commit-messages.html)
   or your code is unlikely be merged into the main project. Use Git's
   [interactive rebase](https://help.github.com/articles/interactive-rebase)
   feature to tidy up your commits before making them public.

4a. Create tests.

4b. Create or update the example code that demonstrates the functionality of this change to the code.

5. Locally merge (or rebase) the upstream development branch into your topic branch:

   ```bash
   git pull [--rebase] upstream main
   ```

6. Push your topic branch up to your fork:

   ```bash
   git push origin <topic-branch-name>
   ```

7. [Open a Pull Request](https://help.github.com/articles/using-pull-requests/)
    with a clear title and description against the `main` branch. All tests must be passing before we will review the PR.
    
## Code Reviews<a name="code-reviews"></a>
If you can, please look at open PRs and review them. Give feedback and help us merge these PRs much faster! If you don't know how, Github has some <a href="https://help.github.com/articles/about-pull-request-reviews/">great information on how to review a Pull Request.</a>
