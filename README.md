# Programming Fundamentals-1 (2022)

[УКР][readme_ua] | [ENG][readme]

[HOME][this_repo] | [PROJECT STRUCTURE][project_structure_readme] | [ASSESSMENT RESULTS][assessment_results]

Repository for assessing labs on the subject "Programming Fundamentals-1"

How to work with this repository and how assessment process will be organized:

1. Fork this repository into your account. [Here][this_repo] you need to press **Fork** or arrow near it and then option **Create new fork**. <br/>
    > *Briefly, **fork** is a full copy of main repository located in your GitHub account, which allows to introduce changes into main repository easily. More information about forks can be found [here][fork_info]*

<br/>

2. Now you need to pull **YOUR** fork on your PC/laptop. 
    1. On the page of your fork find button "Code", press it and copy provided URL
    2. In the console call `git clone https://github.com/<your nickname>/PF1_2022.git`. On this step you may be asked for some logins and passwords (or later). Great, the repo is on your machine now.
    3. One more thing so far. You need to add path to the parent repository. It is called **upstream** repository:
        ```
        git remote add upstream https://github.com/Igor-Sikorsky-IST-Hub/PF1_2022
        ```
    > Command `git remote -v` displays information about connection of your local repository to two repos: **origin** (the one you have) and the **upstream** (main parental).

<br/>

3. Prepare [project structure][project_structure_readme]

<br/>

4. For each LAB create a subdirectory in `reports` directory. See [project structure][project_structure_readme] for detailed instructions.

<br/>

6. Then based on `labs` branch create your own branch
    ```cmd
    git checkout labs
    git checkout -b IA-XX/LAB-YY-TEAM-ZZ-Surname_Name
    ```
    In described commands: `XX` is a group number, `YY` is a lab number and `ZZ` is a team number. Also, don't forget to put your name and surname. If you divide work into multiple parts (each teammate will do small chunk of LAB) then each of you will be required to run these commands.

<br/>

7. Do your lab

<br/>

8. Commit your work
    1. The command `git status` will show you files, which you have changed, added, deleted during work on a task. 
    2. Then take all files which you want to commit and add them one by one:
        ```cmd
        git add one.txt two.txt three.js
        ```
        or stage everything:
        ```cmd
        git add .
        ```
    3. After this do the commit
        ```
        git commit -m "Lab_X: Description which begins from Verb"
        ```
    4. Send branch to your fork:
        ```
        git push origin IA-XX/LAB-YY-TEAM-ZZ-Surname_Name
        ```

<br/>

9. Create pull-request
    After previous command console should provide an URL by which you could create a PR (pull-request). If no, go to the main repository page and create PR manually. Press **compare across forks**. Then select your fork branch `IA-XX/LAB-YY-TEAM-ZZ-Surname_Name` into `labs`.<br/>
    **ATTENTION!**: new lab = new branch = new PR

<br/>

10. When teacher will have time and will review your PRs, then he will either leave comments or merge PR into `labs` branch. If merged, your first part of the lab is done then all what is left is to answer on theory questions right on the lesson.

[assessment_results]: <https://docs.google.com/spreadsheets/d/1_sAxiHEJiXLBl7wpabV2LY9NcDkLxzGhVEhT1Th9oXw/edit?usp=sharing>
[this_repo]: <https://github.com/Igor-Sikorsky-IST-Hub/PF1_2022>
[project_structure_readme]: <Knowledge base/project_structure.md>
[fork_info]: <https://docs.github.com/en/get-started/quickstart/fork-a-repo>
[readme]: <README.md>
[readme_ua]: <README.ua.md>