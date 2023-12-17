# Technical test

## Introduction

Fabien just came back from a meeting with an incubator and told them we have a platform “up and running” to monitor people's activities and control the budget for their startups !

All others developers are busy and we need you to deliver the app for tomorrow.
Some bugs are left and we need you to fix those. Don't spend to much time on it.

We need you to follow these steps to understand the app and to fix the bug : 
 - Sign up to the app
 - Create at least 2 others users on people page ( not with signup ) 
 - Edit these profiles and add aditional information 
 - Create a project
 - Input some information about the project
 - Input some activities to track your work in the good project
  
Then, see what happens in the app and fix the bug you found doing that.

## Then
Time to be creative, and efficient. Do what you think would be the best for your product under a short period.

### The goal is to fix at least 3 bugs and implement 1 quick win feature than could help us sell the platform

## Setup api

- cd api
- Run `npm i`
- Run `npm run dev`

## Setup app

- cd app
- Run `npm i`
- Run `npm run dev`

## Finally

Send us the project and answer to those simple questions : 
- What bugs did you find ? How did you solve these and why ? 
- Which feature did you develop and why ? 
- Do you have any feedback about the code / architecture of the project and what was the difficulty you encountered while doing it ? 

Bugs Fixés :

1) Lorsque l'on voulait modifié un profil, il était impossible de modifié le champ "Name". Je me suis apperçu que ce champ avait l'attribu "disabled", je l'ai donc mis en commentaire. (/app/src/scenes/user/view.js ligne 63)

2) Toujours lorsque l'on voulait modifié un profil, lorque l'on cliquait sur le bouton "Update", rien ne se passait. J'ai donc modifié l'évènement "onChange" en "onClick". (/app/src/scenes/user/view.js ligne 135)

3) Lorsque l'on créait un profil, le champ "Name" ne s'enregistrait pas. J'ai donc changé le nom de l'input en "name" et le la valeur en "user.name" comme cela est défini dans le state "values". (/app/src/scenes/user/list.js ligne 131)