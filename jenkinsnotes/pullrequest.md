#### PULL request beased senario
* What is the use of pull request?
  Actually pull request is used in organizations the manger have the code in main branch and developers take the code and change after the build success the developer create a pull request to manager.The manger check the code and if he satisfied with that code he can merge the code into main branch if he not satisfied he can close the pull request and then he said again some changes in that.
#### GitHub Pull Request
* To make contributions to the repositories where we dont have direct permissions
* We fork the repository
* We make changes
* To get our changes published We create pull requests to the original repo
* The author/owner of repo reviews the changes and merges the pull request if he wants or closes the pull request
  [Referhere](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)
* Development Branches will not have write permissions for developers.
* The create local feature/task/defect branches. Once the work is done, they create pull request.
* We would do Continuous Integration with Static Code Analysis, unit tests, smoke/sanity tests are working or not. If every thing is passing
  we show the results to users who can merge pull requests to make decision to merge or reject.
*  Post merge we do day build.
#### for pull request practise purpose:-
* we need 2 git hub projects
  I can create the new github account(git new acnt:mailid:archanaraj20142019@gmail.com,username:archana2023)
  fork the spc project form old github acnt gotot new github acnt=>repositories=>(search bar)=>dummy spring=>click and fork on click=>fork the project
  * search with old github account username-projectname in new github acnt
  ![Preview](./jenkinsimages/pullgit1.png)
  ![Preview](./jenkinsimages/pullgit2.png)
  ![Preview](./jenkinsimages/pullgit3.png)
  ![Preview](./jenkinsimages/pullgit4.png) 
* Next new git hub account we can change any file after send the pull request (select the branch)
* create a pull request
  ![Preview](./jenkinsimages/pullgit5.png)
  pullrequest=>newpullreqest=>createpullrequest
  ![Preview](./jenkinsimages/pullgit6.png)
* Next goto old github acnt goto repository(ex:dummyspring)=>settings=>webhooks=>add webhooks
  ![Preview](./jenkinsimages/pullgit7.png)
  ![Preview](./jenkinsimages/pullgit8.png)
  ![Preview](./jenkinsimages/pullgit9.png)
  ![Preview](./jenkinsimages/pull1.png)
  ![Preview](./jenkinsimages/pull2.png)
  ![Preview](./jenkinsimages/pull4.png)
  ![Preview](./jenkinsimages/pull5.png)
  ![Preview](./jenkinsimages/pull6.png)
  ![Preview](./jenkinsimages/pull7.png)
  ![Preview](./jenkinsimages/pull8.png)
  ![Preview](./jenkinsimages/pull9.png)
  * Before that we can install pull request plugin in jenkins
  * mangae jenkins=>manage plugins=>available plugins=>githubpullrequest=>install without restart
* Next goto dashboard=>Free style=>New Item=>ok=>(spc-free-pull)
  ![Preview](./jenkinsimages/pull10.png)
  ![Preview](./jenkinsimages/pull11.png)
  build triggers=>githubpullrequestbuilder=>adavance=>
  ![Preview](./jenkinsimages/pull12.png)
  ![Preview](./jenkinsimages/pull13.png)
  BuildEnvironments=>delete workspace after build
  ![Preview](./jenkinsimages/pull14.png)
* Build Now 
  ![Preview](./jenkinsimages/pull15.png)
* If this ![Preview](./jenkinsimages/pull16.png) error came give mvn path in execute shell 
* It's autometically triggering the bulid in jenkins
Actually we created pull request in develop branch so we can mentioned branch name in whitelist.
[Referhere](https://plugins.jenkins.io/ghprb/)for Documentation   
  

* Then if the project is success the and the manger satisfied for that code he can accept the pull request and merge the code
