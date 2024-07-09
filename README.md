# Learning npm: A Package Manager

This is the repository for the LinkedIn Learning course Learning npm: A Package Manager. The full course is available from [LinkedIn Learning][lil-course-url].

![Learning npm: A Package Manager][lil-thumbnail-url]
![Learning npm: A Package Manager][lil-thumbnail-url]

npm is an indispensable part of every developer's toolbox. It's the package manager for JavaScript and JavaScript frameworks such as Node.js, enabling developers to easily share and re-use code. In this course, Emmanuel Henri teaches developers how to work with npm commands to install and manage project dependencies. He starts with showing how to install npm, and details all the basic tools you can use with npm, such as adding, updating, or removing a package. Emmanuel then shows you how to take your skills to the next level, taking a dive deep into advanced features like npm cache, audits, scripting, and more.

_See the readme file in the main branch for updated instructions and information._

## Instructions

This repository has branches for each of the videos in the course. You can use the branch pop up menu in github to switch to a specific branch and take a look at the course at that stage, or you can add `/tree/BRANCH_NAME` to the URL to go to the branch you want to access.

## Branches

The branches are structured to correspond to the videos in the course. The naming convention is `CHAPTER#_MOVIE#`. As an example, the branch named `02_03` corresponds to the second chapter and the third video in that chapter.

The branches are structured to correspond to the videos in the course. The naming convention is `CHAPTER#_MOVIE#`. As an example, the branch named `02_03` corresponds to the second chapter and the third video in that chapter.
Some branches will have a beginning and an end state. These are marked with the letters `b` for "beginning" and `e` for "end". The `b` branch contains the code as it is at the beginning of the movie. The `e` branch contains the code as it is at the end of the movie. The `main` branch holds the final state of the code when in the course.

When switching from one exercise files branch to the next after making changes to the files, you may get a message like this:

    error: Your local changes to the following files would be overwritten by checkout:        [files]
    Please commit your changes or stash them before you switch branches.
    Aborting

To resolve this issue:
Add changes to git using this command: git add .
Commit changes using this command: git commit -m "some message"
Add changes to git using this command: git add .
Commit changes using this command: git commit -m "some message"

### Instructor

Emmanuel Henri

Emmanuel Henri

Author

Check out my other courses on [LinkedIn Learning](https://www.linkedin.com/learning/instructors/emmanuel-henri).

[lil-course-url]: https://www.linkedin.com/learning/learning-npm-a-package-manager?dApp=59033956
[lil-thumbnail-url]: https://media.licdn.com/dms/image/C560DAQF6xNNOUO2ZwQ/learning-public-crop_288_512/0/1678465785599?e=2147483647&v=beta&t=INjO7_K3vfBFPnr7LP3QDkABNI2O9yUJvAuOaYP2xoY

npm init cria o package.json
npm -save-dev sigfica que vai salvar como dev dependecy, ou seja quando
rodar uma build de prod, esse package não vai ta la
npx instala os pacote, faz o que tem que fazer, depois remove, tipo o create-react-app, a mesma coisa com angular pode ser feita

npm install -g instala globalmente
pra instalar com versão é desse jeito npm install eslint@5.2.0
npm outdated checa quais packages estão desatualizados
se for npm outdated -g, checa os globais
npm update [package-name] atualiza pra ultima versão, se usar o install também funciona
na duvida usa o npm install [package-name]@latest

npm uninstall recebe os mesmo paramentro do install, -g ou -save-dev também

~ (tio) é mais restritivo, permitindo apenas atualizações de patch.
^ (chapéu) é mais permissivo, permitindo atualizações de patch e minor, desde que a versão principal (major) não mude.

package-lock.json é a saida, praticamente é pra garantir que em outra maquina não vai dar ruim as versões

As vezes no npm tem que limpar o cache
npm cache verify ve o que tem no cache
pra limpar o cache usa npm cache clean -force

npm audit mostra os problemas dos package instalado
npm audit fix tenta resolver alguns problemas, mas nao resolve todos

npx pode ter script dele
se rodar por exemplo nrpm run createangapp, vai rodar o comando do npx dentro dele
