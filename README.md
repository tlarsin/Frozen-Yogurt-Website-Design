# Frozen-Yogurt-Website-Design
I created a mockup of a frozen yogurt website design for Jacq Frost, inspired by a frozen yogurt website for a Milwaukee based business. Not affiliated with Jacq Frost.

## Lab Stuff
> What does it report? Edit your README.md file and add a section about git status and what it does. Then, copy/paste the results from git status in there.

Git status checks the local files and displays whether or not the files have been changed since they were last opened. If a file has been modified, it will display it (colored in red) saying the it has been modified. This allows you to keep track of what has been changed, and also to know which files need to be uploaded to keep the project up to date. Once a file has been committed, it will appear as green signifying that it is ready to be pushed. After it has been pushed, there will be no files listed (assuming all files that had been changed were committed and pushed).

Here is the `git status` output:
```
On branch master
Your branch is up-to-date with 'origin/master'.
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

  modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)

  .DS_Store
  Icons/.DS_Store
  README.md~
  test.cpp~

no changes added to commit (use "git add" and/or "git commit -a")
```
  
<p align="center">
   <img src="https://github.umn.edu/novot039/TestGitRepo/blob/master/Icons/GitHub.png"/>
</p>

# Git Basics

This README covers the basics of Git usage.

## Commands and Editing

This section covers basic commands for modifying files and repositories.

#### Commits and Pushing
* Edit files by calling emacs with the command `emacs [FILE_NAME]`
* Commit files with a comment by using the command `git commit -m "[MESSAGE]" [FILE_NAME]`
  * To commit with a larger comment use the command `git commit [FILE_NAME]`
* Push files to GitHub using `git push`

#### Cloning and Initialization
* To clone a repository, cd to the desired destination and use the command `git clone <REPO_SSH_ADDRESS>`
* To turn a directory into a Git Repository, cd to the desired folder and use the command `git init`
  * Add the files in the directory by using the command `git add .`
  * Commit the files by using the commit command above
  * Add the repository URL by using the command `git remote add origin <REPO_SSH_ADDRESS>`
  * Push the changes and files to GitHub by using the command `git push -u origin master`

#### Removing Files
1. To remove a file from the repository, use the command `git rm <FILE_NAME>`
2. You will then have to commit the change using the commit command above
3. Push the changes to the repository by using the push command above

## README Markdown Notations

This section outlines what syntax is used for README file formatting.

#### Text Styling

Style|Syntax|Example|Output
---|---|---|---
Bold|`** **`|`**This is bold text**`|**This is bold text**
Italic|`* *`|`*This text is italicized*`|*This text is italicized*
Strikethrough|`~~ ~~`|`~~This text is bad~~`|~~This text is bad~~

#### Quotes, Links, and Lists

**Quotes**

There are two types of quotes that are available to use, *text* and *code* quotes. Text quotes are for quoting someone or something, and are used by placing `>` before the desired quote. This is an example of a text quote:
> Lorem ipsum dolor sit amet, an porro homero vim, ea modo illud vel. -Unknown

Code quotes are used for displaying snippets of code, and can be used by placing backticks in front and behind the desired area. Here is an example of a code quote:
```
string helloWorld(bool greeting) {
  if (greeting == true) {
    cout << "Hello World";
  }
}
```

**Links**

Links are handled as they would be on any online forum, simply by placing text in enclosed brackets, followed by the URL enclosed in parenthesis. In turn, the end result is this: 

`[Imgur](https://www.imgur.com)`

Which when handled in context, appears as a clickable link: [Imgur](https://www.imgur.com)

**Lists**

Lists can be either bulleted or numbered, and can be indented as well. Use `*` for bulleted lists, and `1.` for numbered list. List indentations can be applied by placing two spaces in front of the deliminator. Here is an example of a bulleted list:
* First item
  * Second item

The same technique applies for numbered lists as well:

1. First item
   1. Second item

#### Tables
Tables can be any size and can work with certain other types of formatting syntax. The formatting for tables is as follows:
```
Header 1|Header 2|Header 3
--------|--------|--------
 Item 1 | Item 2 | Item 3 
 Item 4 | Item 5 | Item 6 
```

Which will result in the table below:

Header 1|Header 2|Header 3
--------|--------|--------
 Item 1 | Item 2 | Item 3
 Item 4 | Item 5 | Item 6
