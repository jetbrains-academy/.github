# Marketplace course ready-for-publish checklist
Before publishing a course to the Marketplace, make sure that you can say "YES" to each point in this checklist.  
> [!IMPORTANT]
> We check courses to ensure that they match this checklist.

## Mandatory
### Language requirements
- [ ] The course title is in English
- [ ] At least the first sentence of the course description is written in English
- [ ] The language of the course in `course-info.yaml` specified correctly

### Clear descriptions
- [ ] The first sentence of the course description is self-sufficient, concise, and provides useful information about the course.
- [ ] Course description field contains an easy-to-understand detailed course description
- [ ] Course prerequisites are indicated at the beginning of the course.

### Technical requirements
- [ ] Make sure you use a [template](https://github.com/jetbrains-academy#templates) when creating your course, if there is one for your language/technology
- [ ] You've made sure that all tests in [GitHub Actions](https://docs.github.com/en/actions/quickstart#viewing-your-workflow-results) pass, if you used a template that has them
- [ ] All tests for all course tasks are passed. You can also [automate this check](https://blog.jetbrains.com/education/2022/10/27/edutools-plugin-2022-10-available/#🆕%C2%A0automatic-task-checking-for-new-courses) when creating the archive.
- [ ] The course contains more than 5 tasks
- [ ] Tasks have a meaningful description, tests check the solution of the problem given in the task description 
- [ ] Only the files needed by the user to solve the task are displayed in Course View. Other files (like images used in task.md, etc.) are [hidden](https://plugins.jetbrains.com/plugin/10081-jetbrains-academy/docs/educator-start-guide.html#create_course) from the user. So that they appear in the task description, but not in the list of files in Course View.
- [ ] Only the plugins required for the course are listed in the course dependencies. Read more about managing the required plugins [here](https://www.jetbrains.com/help/idea/managing-plugins.html#required-plugins).

### Python
- [ ] `requirements.txt` contains all the [dependencies](https://www.jetbrains.com/help/pycharm/managing-dependencies.html) required in the course

### Gradle
- [ ] A modern-style configurations are used: `implementation` and `testImplementation` instead of `compile` and `testCompile`, respectively. In Gradle 7.0 these configurations were [removed](https://docs.gradle.org/current/userguide/upgrading_version_6.html#sec:configuration_removal), and they lead to errors during course project loading.

## Optional
### Formatting
- [ ] `<code></code>` or/and backtick (&#96;) quote highlighting is really only used for code
- [ ] All code insertions are highlighted with `<code></code>` or/and backtick
- [ ] Multiple lines code blocks in `task.md` files highlighted with using Python syntax (&#96;&#96;&#96;text&#96;&#96;&#96;) instead of using single &#96;text&#96; code tags
- [ ] `highlighting` is used to highlight blocks of output.
- [ ] Images has `width` [attribute](https://www.w3schools.com/tags/att_width.asp) in case images in the task description are too large

### Code / text quality
- [ ] The text is well proofread. (Optionally, we can offer our assistance with this. Please let us know if this works for you)
- [ ] Code formatting follows the appropriate coding style for the language used, for example [PEP8](https://peps.python.org/pep-0008/). The IDE can [do the code formatting](https://www.jetbrains.com/help/pycharm/reformat-and-rearrange-code.html) on you.
