[![generate](https://github.com/Spatial-Web-Foundation/SWF-Corpus_and_IEEEP2874-D2/actions/workflows/generate.yml/badge.svg)](https://github.com/Spatial-Web-Foundation/SWF-Corpus_and_IEEEP2874-D2/actions/workflows/generate.yml) [![nightly artifacts cleanup](https://github.com/Spatial-Web-Foundation/SWF-Corpus_and_IEEEP2874-D2/actions/workflows/nightly_cleanup.yml/badge.svg)](https://github.com/Spatial-Web-Foundation/SWF-Corpus_and_IEEEP2874-D2/actions/workflows/nightly_cleanup.yml) [![post status report](https://github.com/Spatial-Web-Foundation/SWF-Corpus_and_IEEEP2874-D2/actions/workflows/post_status_report.yml/badge.svg)](https://github.com/Spatial-Web-Foundation/SWF-Corpus_and_IEEEP2874-D2/actions/workflows/post_status_report.yml)

# HSML Implementation Specification

This repo contains the contents of the HSML Implementation Specification.

At this time and until further notice, only SWF employees and advisors can access this repository. All contents are SWF copyright.

Most of the information below is provided in [this video](https://app.usebubbles.com/qgVNGBkdFQbNevxAJRwNum/p2874-d2-contribution-strategy). 

## 1 Getting Started

The PDF and HTML are automatically generated and available in the `site.zip` artifact of the `generate` stage of the GitHub actions that run on every single commit for any branch. The generated artifacts will only be available for approximately 24 hours, after which they will be automatically deleted.

## 2 How To Contribute

The recommended practice to contribute is by creating a pull request with a specific GitHub issue that it is addressing. There are two strategies that can be used to accommodate individuals with various levels of git experience. They can be broken down into either:

- Without Cloning Repository (Easy)
- Cloning Repository (Preferred)

The high level process for contributing can be summarized by the image as seen below.
![development-issue-create-branch](https://github.com/Spatial-Web-Foundation/HSML-Implementation-Specification/blob/main/documentation/images/pr-process.png)

The image shown above outlines the following high-level steps:

1. Create a branch
2. Add commits to branch
3. Open a pull request
4. Discuss and review pull request
5. Merge pull request to `main`

### 2.1 Without Cloning Repository (Easy)

**Who is this for?** This strategy is geared towards expending minimal effort to get desired changes to the repository. This would allow for the changes to be made using a more simplified process.

#### 2.1.1 Contribution Strategy

1. <u>Create a branch from issue</u>

   - Navigate to the issue that you would like to make a contribution for. From the issue view, click the "Create a branch" button from the "Development" section on the right column.

     Note: If a branch has already been created for this issue, the name of the branch will be shown instead.

     ![development-issue-create-branch](https://github.com/Spatial-Web-Foundation/HSML-Implementation-Specification/blob/main/documentation/images/development-issue-create-branch.png)

2. <u>Open browser vscode editor</u>

   - Click [here](https://github.dev/Spatial-Web-Foundation/HSML-Implementation-Specification) to open a browser version of vscode with the repository checked out.

3. <u>Checkout desired branch</u>

   - In order to checkout the desired branch, click the currently checked out branch in the bottom left of the editor. See the image below.

     ![vscode-change-branch-1](https://github.com/Spatial-Web-Foundation/HSML-Implementation-Specification/blob/main/documentation/images/vscode-change-branch-1.png)

   - Select, from the list or by searching, the desired branch from the pop window.

     ![vscode-change-branch-2](https://github.com/Spatial-Web-Foundation/HSML-Implementation-Specification/blob/main/documentation/images/vscode-change-branch-2.png)

4. <u>Contribute (commit) to branch</u>

   - Once you've made changes (create, update, or delete) to the checked out branch, the changes need to be committed.

   - Navigate to the commit window by clicking the icon from the left vertical pane. See image below.

   ![vscode-source-control-view](https://github.com/Spatial-Web-Foundation/HSML-Implementation-Specification/blob/main/documentation/images/vscode-source-control-view.png)

   - Add (stage) the files that you would like to commit by pressing the "+" icon next to the files.

   - Write a short message describing the changes that you've made

   - Click the commit button that looks like a checkmark on the top right of the source control view panel. See image below.

   ![vscode-commit-button](https://github.com/Spatial-Web-Foundation/HSML-Implementation-Specification/blob/main/documentation/images/vscode-commit-button.png)

5. <u>Create a pull request (PR)</u>

   - This can be done by navigating to the "Pull Requests" tab and clicking the "New Pull Request" button.
   - Once clicked, the branches to create a pull request for should be selected. There should be two drop down menus available: "base" and "compare". The "base" branch should be "main". The "compare" branch should be the branch that you created in step 1 for which you have made commits (changes) and you would like to compare changes for.

6. <u>Associate GitHub issue with pull request</u>

   - There are two ways to associate a GitHub branch to a pull request:

     - _Modify the description of the PR_ - edit the description of the pull request (i.e. edit the empty description) and typing "Closes" followed by the issue reference on a NEW line. For example, `Closes #123` on a new line in the description will automatically link the issue to the pull request `Closes #123`. Multiple issues can be referenced in the pull request by repeating for each issue to be closed on a new line in the description.
     - _Manually associate issue with PR_ - click the gear icon next to the "Development" section in the right column of the pull request's view. This will prompt a drop down that can be used to search for and associate one or more issues to be closed when the pull request is merged to the "main" branch.

       ![section called "Development"](https://github.com/Spatial-Web-Foundation/HSML-Implementation-Specification/blob/main/documentation/images/development-part-of-PR-page.png)

7. <u>Add reviewers</u>
   - In the upper right of the PR view, add the editors, Christine (@cperey) and Prasaanth (@PrasaanthSridharan). In addition, add the lead of the clause associated with the clause or subclause you are changing (assuming that you are not the clause lead). If you create the PR, you can't also be a reviewer.

### 2.2 Cloning Repository (Preferred)

**Who is this for?** If you are familiar with the git toolchain and are comfortable using an IDE (e.g. Visual Studio Code, Atom, etc.), you will be most comfortable with this strategy.

#### 2.2.1 Contribution Strategy

1. <u>Clone the repository</u>

   - This can be done from the command line (e.g. Git Bash, Terminal, etc.) or by using an application like GitHub Desktop.

2. <u>Create a branch</u>

   - This can be done from the command line (e.g. Git Bash, Terminal, etc.), by using an application like GitHub Desktop, or from the GitHub issue view.

3. <u>Commit changes to a branch</u>

   - Using the IDE of your preference (e.g. Visual Studio Code), make changes to the repository and then commit your changes. The commits can be done from the command line, using the user interface available in Visual Studio Code, or using GitHub Desktop application.

4. <u>Create a pull request</u>

   - This can be done by navigating to the "Pull Requests" tab and clicking the "New Pull Request" button.
   - Once clicked, the branches to create a pull request for should be selected. There should be two drop down menus available: "base" and "compare". The "base" branch should be "main". The "compare" branch should be the branch that you created in step 2 for which you have made commits (changes) and you would like to compare changes for.

5. <u>Associate GitHub issue with pull request</u>

   - There are two ways to associate a GitHub branch to a pull request:

     - _Modify the description of the PR_ - edit the description of the pull request (i.e. edit the empty description) and typing "Closes" followed by the issue reference on a NEW line. For example, `Closes #123` on a new line in the description will automatically link the issue to the pull request `Closes #123`. Multiple issues can be referenced in the pull request by repeating for each issue to be closed on a new line in the description.
     - _Manually associate issue with PR_ - click the gear icon next to the "Development" section in the right column of the pull request's view. This will prompt a drop down that can be used to search for and associate one or more issues to be closed when the pull request is merged to the "main" branch.

       ![section called "Development"](https://github.com/Spatial-Web-Foundation/HSML-Implementation-Specification/blob/main/documentation/images/development-part-of-PR-page.png)

6. <u>Add reviewers</u>
   - In the upper right of the PR view, add the editors, Christine (@cperey) and Prasaanth (@PrasaanthSridharan). In addition, add the lead of the clause associated with the clause or subclause you are changing (assuming that you are not the clause lead). If you create the PR, you can't also be a reviewer.
   
#### 2.2.2 Useful Visual Studio Code Extensions

| Name                                                                                           | ID                               | Description                                 |
| ---------------------------------------------------------------------------------------------- | -------------------------------- | ------------------------------------------- |
| [AsciiDoc](https://marketplace.visualstudio.com/items?itemName=asciidoctor.asciidoctor-vscode) | `asciidoctor.asciidoctor-vscode` | Provides rich language support for AsciiDoc |
