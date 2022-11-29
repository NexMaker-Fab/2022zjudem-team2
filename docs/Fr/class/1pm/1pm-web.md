<!-- How to buil web class/1pm-web.md -->
 # COMMENT CONSTRUIRE LA PAGE
 ### PREMIEREMENT: Préparer
   Installation de tous les outils nécessaires pour créer la page Web:

  - [Git](https://git-scm.com/downloads); Nous avons utilisé git pour contrôler notre version dans gitlab
  - [Github](https://github.com/); Nous avons utilisé github comme réparateur pour notre page Web
  - [Github desktop](https://desktop.github.com/); Nous avons utilisé le bureau github pour transporter ou pousser notre codage de local à github
  - [VScode](https://code.visualstudio.com/); Nous avons utilisé le code Visual Studio pour écrire nos documents
  - [Nodejs](https://nodejs.org/en/); Nous l'avons utilisé pour construire l'environnement
  - Le langage [Markdown](https://www.nexmaker.com/doc/1projectmanage/markdown.html); Nous avons utilisé le langage Markdown pour écrire des documents
  - [Image upload servive](https://www.nexmaker.com/doc/1projectmanage/imageuploadservice.html), Nous avons utilisé Picgo pour stocker nos images sur le cloud, dans notre cas dans gitlab et utilisé dans le document Markdown,
 ### DEUXIEMEMENT: Les astuces
   1. Paramètres de la page Web
      Construisez un référentiel, gardez-le public pour les membres de votre équipe afin que n'importe qui sur Internet puisse y avoir accès et ajoutez-y un fichier README car c'est là que vous pouvez écrire une longue description pour
      votre projet.
      <br>Exemple
      <div class="loader"><img src="images/1.jpg" alt="#" /></div>
      <br>REMARQUE:Ouvrez le référentiel, accédez aux paramètres, aux pages sous la branche, sélectionnez la source principale pour activer les pages Github pour ce référentiel et sous le dossier, sélectionnez racine et enregistrez(Attention; vous avez sélectionné le dossier racine car vous n'avez pas encore installé de dossier docs pour ce référentiel, vous devrez donc modifier ce paramètre ultérieurementvous avez sélectionné le dossier racine car vous n'avez pas encore installé de dossier docs pour ce référentiel, vous devrez donc modifier ce paramètre ultérieurement)
      <br> Exemple
      <div class="loader"><img src="images/2.jpg" alt="#" /></div>

   2. Paramètres locaux
      Ouvrez le bureau Github, clonez votre référentiel créé précédemment et ouvrez-le dans Visual Studio Code
      <br> Exemple
      <div class="loader"><img src="images/3.png" alt="#" /></div>

   3. Structure
    * Ajoutez le mot "Hello" au fichier README.md, enregistrez tout et utilisez le bureau github pour valider et pousser vers la page Web
    * Nous utilisons la méthode Docsify pour construire la structure, sous la barre de menu vscode ouvrez le Terminal
    <br> Exemple
      <div class="loader"><img src="images/4.png" alt="#" /></div>
     1. Installer docsify

          "npm i docsify-cli -g"
          <br>Pour [plus d'information](https://www.npmjs.com/package/docsify-build-cli)

     2. Make sure the position and then initialize environment
          
          "docsify init ./docs"
          <br>Pour [plus d'information](https://cli.docsifyjs.org/#/?id=links)

     3. Aperçu
          
          "docsify serve docs"

     4. Visite le navigateur http://localhost:3000
     <br> Exemple
      <div class="loader"><img src="images/5.png" alt="#" /></div>
     5. Définition de index.html
     <br>Pour [plus d'information](https://www.nexmaker.com/doc/1projectmanage/github&docsify.html)
     6. Ajouter une barre latérale et une barre de navigation (sidebar & navbar)
     <br>[for more information](https://github.com/kn0sky/docsify-autosidebar)
     7. Rédigez le document et enregistrez tous les documents sous [VScode](https://code.visualstudio.com/)
     8. Pousser vers Github
     <br><img src="images/push.png">

     <br>Utilisez le bureau github pour pousser les nouvelles informations téléchargées sur VScode, ouvrez Github sous les paramètres du référentiel/pages changent le dossier de la branche de root à docs.
     <br> Exemple
      <div class="loader"><img src="images/6.png" alt="#" /></div>

### TROISIEMEMENT: Méthode pour changer de langue
#### Première méthode 
1. Créez un dossier appelé langue et ajoutez-y 2 fichiers(ex:en.json and cn.json)

<br>Tles fichiers json doivent avoir une structure identique mais une traduction différente comme ci-dessous:

<br><h1 style="font-size:1.5vw"><span style="color:black">en.json</span></h1>

{<p>"date":<span style="color:green">"Date"</span>,</p>
<p>"save":<span style="color:green">"save"</span>,</p>
<p>"cancel":<span style="color:green">"cancel"</span>,</p>}

<br><h1 style="font-size:1.5vw"><span style="color:black">cn.json</span></h1>

{<p>"date":<span style="color:green">"日期"</span>,</p>
<p>"save":<span style="color:green">"节省"</span>,</p>
<p>"cancel":<span style="color:green">"取消"</span>,</p>}
 
 <br>
 
2. Créez une page html contenant un exemple de div et mettez 2 liens pour sélectionner la langue pointant vers la fonction js listée au point 3.

<br>

```html

 <a href="#" onclick="setLanguage('en')">English</a> 
 <a href="#" onclick="setLanguage('cn')">Chinese</a>

 <div id="div1"></div>

```
3. Créez 2 fonctions de script java pour obtenir/définir la langue sélectionnée:

```htm 

<script>
var language; 
function getLanguage() {
(localStorage.getItem('language') == null) ? setLanguage('en') : false;
$.ajax({ 
url:  '/language/' +  localStorage.getItem('language') + '.json', 
dataType: 'json', async: false, dataType: 'json', 
success: function (lang) { language = lang } });
}
function setLanguage(lang) {
localStorage.setItem('language', lang);
}
</script>

```
<br>

4. Utiliser la variable langue pour remplir le texte.

```html

<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
    <script>

    $(document).ready(function(){
    $('#div1').text(language.date);
    });

    </script>
``` 
<br>

#### Method 2

Build your webpage using html under a docs folder.
<br><img src="images/docs1.png">

<br>After buildind, open the docs folder, copy every files and folders under it, create a new folder under the original docs folder and name it (ex:folder name"Cn" for Chinese language), past all in the new folder created (Cn), this will keep all files and folders identical in structure.

<p><br><img src="images/docs2.png"><br><img src="images/docs3.png"></p>
<br>Translate every file's contents into chinese 

### STEP4: Method for steps sidebar
Nearly all Markdown applications support the basic syntax outlined in the original Markdown design document. There are minor variations and discrepancies between Markdown processors,those are noted inline wherever possible.

<br>In our case it's as simple as <span style="background-color: #FFFF00">adding 3 pound signs(#)</span> in front of each step or phrase. Normally the number of pound signs(#) correspond to the heading level.

 ### PROBLEMS & SOLUTIONS
  1. Docsify init ./docs cannot be loaded because running scripts is disabled on this system.

      <div class="loader"><img src="images/7.jpg" alt="#" /></div>
      <br>Solution
       <br>The reason why the running scripts was disable on the system was because the running mode was strict ,you can change to Unrestricted or Bypass，by using the following code <span style="background-color: #FFFF00">Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Unrestricted -Force</span> or <span style="background-color: #FFFF00">Set-ExecutionPolicy -Scope CurrentUser -ExecutionPolicy Bypass -Force</span>
  2. The term 'docsify' is not recognized as the name of a cmdlet, function, script file, or operable program.

      <div class="loader"><img src="images/8.jpg" alt="#" /></div>
      <br>Solution
       <br>This error means docsify cannot be found in the PATH. <span style="background-color: #FFFF00">Eitherinstall it globally</span> (recommended for many command-line tools, and where it is found in the global Github folder, already in the PATH) or <span style="background-color: #FFFF00">run it from where it is installed in the local Github</span>

     - [Verify Path](https://www.youtube.com/watch?v=pg4t48BPmh8&t=134s)
       <br><span style="background-color: #FFFF00">This PC->Properties->Advanced system settings->Environment Variables->User variables->Path->Edit</span>
       <br>Verify the path> <span style="background-color: #FFFF00">C:\Users\RAZER\Desktop\IDE\1ST YEAR\DESIGN ENGINEERING\Practice</span>
       <br>If the path is not there you can copy it and past a new path under the Edit environment variable
       <br>

  


  

