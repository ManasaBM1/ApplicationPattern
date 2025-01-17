# Formulating Commit and Merge Request Messages

Development of documentation, specification and code shall be collaborative.  
This includes reviewing artifacts before consolidating them into the shared base.  
Such review is not just "additional work", but also time critical, because the shared base might change between merge request and merge commit.  
Well formulated **merge request messages must support efficiently reviewing** the contributed artifact.

### Subject line

* **50 characters** or less: formulate meaningful, concise and comprehensive!
* **start subject line with a verb, e.g. with one of the following keywords**, as e.g. Add, Update, Remove, Refactor, Revert ...
* write in the imperative: e.g. "Add ServiceList" not "ServiceList added" or "Adds ServiceList"
* do not end the subject line with a dot

### Message body

* **separate subject from body with a blank line**, if e.g. VSCode is used
* **automate by references**: In case of a pull-request, add "Fixes #issue-number" to the description and the pull-request will be mentioned in the issue and the issue will automatically close after successful merge.
* nice to have:
  * explain _what_ and _why_ something has been done, but details about _how_ a change has been made can be left out in most cases
  * describe effects of the change
  * relate to the content of the issue
  * describe limitations of the current code or delivery item
  * bullet points can be used
  * capitalize each paragraph
  * wrap lines at 72 characters
  * do not assume that reviewers understand what the original problem was
  * do not assume the change/code is self-evident/self-documenting
  * if documentation from inside GitHub or external pages should be referenced, these can be linked by \[add link text in square brackets\]\(add link URL in parenthesis\)
    
The commit message dialogues at GitHub and VSCode are slightly different.

|**GitHub**|**VSCode**|
|---|---|
|The subject line and body have own text fields.|There is only a single textfield (add linebreaks <br>like in any regular editor to separate subject line and body).|
|![commit_2](https://user-images.githubusercontent.com/57349523/155980718-cbbb2d14-89c7-4938-9e15-70253f7252e3.jpg)|![commit_1](https://user-images.githubusercontent.com/57349523/155980716-30b63626-4f73-4268-9851-cbefc6d24619.jpg)|

[<- Back to Formulating Issues](../FormulatingIssues/FormulatingIssues.md) - - - [Up to Preparing for Specifying Applications](../PreparingSpecifying.md) - - - [Ahead to Managing Conflicts ->](../ConflictManagement/ConflictManagement.md)
