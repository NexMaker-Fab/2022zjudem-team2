<!-- How to buil web class/1pm-web.md -->
 # HOW TO BUILD
 ### STEP1: Prepare
   Installing all the necessary tools to build the webpage:

  - [Git](https://git-scm.com/downloads); We used git to controil our version in gitlab
  - [Github](https://github.com/); We used github as a servicer for our webpage
  - [Github desktop](https://desktop.github.com/); We used github desktop to transport or push our coding from local to github
  - [VScode](https://code.visualstudio.com/); We used the visual studio code to write down our documents
  - [Nodejs](https://nodejs.org/en/); We used it to build the environment 
  - [Markdown](https://www.nexmaker.com/doc/1projectmanage/markdown.html) language; We used the Markdown language to write documents
  - [Image upload servive](https://www.nexmaker.com/doc/1projectmanage/imageuploadservice.html), We used Picgo to storage our image on cloud, in our case in gitlab and used in markdown document,
 ### STEP2: Tips
   1. Web page settings
      Build a repository, keep it Public for your team members so that anyone on the internet can have access to it and add a README file to it cause that's where you can write a long description for 
      your project.
      <br>Example
      <div class="loader"><img src="images/1.jpg" alt="#" /></div>
      <br>NOTE:Open the repository go to settings, pages under branch select the main source to enable Github pages for this repository and under folder select root and save(Attention; you selected root folder because you havn't yet installed a docs folder for this repository, therefore you will have to change this setting later)
      <br> Example
      <div class="loader"><img src="images/2.jpg" alt="#" /></div>

   2. Local settings
      Open Github desktop, clone your repository created earlier on and open it in Visual Studio Code
      <br> Example
      <div class="loader"><img src="images/3.png" alt="#" /></div>

   3. Structure
    * Add "Hello" word to the README.md save all and use github desktop to commit and push to the web page
    * We use the Docsify methode to build the structure, under the vscode menu bar open the Terminal
    
     1. Install docsify

          "npm i docsify-cli -g"
          <br>[Read more](https://www.npmjs.com/package/docsify-build-cli)

     2. Make sure the position and then initialize environment
          
          "docsify init ./docs"
          <br>[Read more](https://cli.docsifyjs.org/#/?id=links)

     3. Preview
          
          "docsify serve docs"

     4. Browser visit http://localhost:3000


   - Problems & Solution

