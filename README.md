<p align="center"><h1>ARIMA-MD</h1><br> </p>

![banner](Arima.jpg)
![FCF6F1C9-1614-4C6B-9686-B7D0E949E3B7](https://github.com/user-attachments/assets/c7abc40a-2974-43b0-9cca-565720ed74c9)



## Obtenir ARIMA-MD 🛠️

1. Cliquez sur **[Fork](https://github.com/Luffy2ndAccount/zokou-2.0-versionVF/fork)** 

2. Obtenez une session du bot :  
   - [Session-1](https://Arscan.onrender.com)  
   - [Session-2](https://Arimascan-din3.onrender.com)


     ## Déploiement 


- **Déploiement sur Koyeb** :
  1. Si vous n'avez pas de compte **Koyeb**, cliquez [**ici**](https://dashboard.koyeb.com/signup) pour en créer un.
  2. Cliquez sur le bouton ci-dessous pour déployer sur Koyeb :<br>
     [![Deploy to Koyeb](https://www.koyeb.com/static/images/deploy/button.svg)](https://app.koyeb.com/deploy?name=zokouvf&type=docker&image=docker.io%2Fluffy077%2Fzokouvf%3Alatest&env%5BPREFIXE%5D=.&env%5BLECTURE_AUTO_STATUS%5D=oui&env%5BTELECHARGER_AUTO_STATUS%5D=oui&env%5BNOM_BOT%5D=Zokou-MD&env%5BLIENS_MENU%5D=https%3A%2F%2Fwallpapercave.com%2Fuwp%2Fuwp3943464.jpeg&env%5BPM_PERMIT%5D=non&env%5BMODE_PUBLIC%5D=oui&env%5BETAT%5D=1&env%5BSESSION_ID%5D=mettez+votre+session&env%5BNOM_OWNER%5D=Djalega%2B%2B&env%5BNUMERO_OWNER%5D=22891733300&env%5BWARN_COUNT%5D=3&env%5BSTARTING_BOT_MESSAGE%5D=oui&env%5BANTI_VUE_UNIQUE%5D=oui&env%5BPM_CHATBOT%5D=non&env%5BHEROKU%5D=non&env%5BDATABASE_URL%5D=mettez+une+database&env%5BANTI_COMMAND_SPAM%5D=non&ports=8000%3Bhttp%3B%2F)

- **Déploiement sur Render** :
  1. Si vous n'avez pas de compte **Render**, cliquez [**ici**](https://dashboard.render.com) pour vous inscrire.
  2. Créez un nouveau sweb service.  
  3. Choisissez **Public Git Repository**.  
  4. Dans le champ , entrez `https://gitlab.com/bankai421341/senbonzakura.git`.
  5. Cliquez sur **Connect**.  
  6. Sélectionnez le **Free Plan** si vous ne voulez pas payer.  
  7. Dans la section **environemment variable**, cliquez sur **Add from .env** et copiez le contenu suivant :

     ```env
     PREFIXE=.
     LECTURE_AUTO_STATUS=oui
     TELECHARGER_AUTO_STATUS=oui
     NOM_BOT=Zokou-MD
     LIENS_MENU=https:[//wallpapercave.com/uwp/uwp3943464.jpeg](https://wallpapercave.com/download/uwp-4570967)
     PM_PERMIT=non
     MODE_PUBLIC=non
     ETAT=1
     SESSION_ID=Ari
     NOM_OWNER=༺𒋲♱𝚫𝚪𝚰𝚳𝚫♱𒋲༻ 
     NUMERO_OWNER=237620934302
     WARN_COUNT=3
     STARTING_BOT_MESSAGE=oui
     ANTI_VUE_UNIQUE=oui
     PM_CHATBOT=non
     ANTI_COMMAND_SPAM=non
     ```

  8. Cliquez sur **Add env** pour enregistrer, puis modifiez selon vos besoins. N'oubliez pas d'entrer votre session ID.  
  9. Cliquez sur **Deploy service** et profitez-en !


 - **Déploiement GitHub**

  1. **Forkez le dépôt**.
  2. Modifiez le fichier `exemple_de_set.env` en `set.env` et ajoutez-y votre **session_ID**.
  3. Créez un nouveau fichier `.github/workflows/deploy.yml` et mettez-y ce contenu :

```yml
name: Node.js CI

on:
  push:
    branches:
      - main
  pull_request:
    branches:
      - main
  schedule:
    - cron: '0 */4 * * *'

jobs:
  build:

    runs-on: ubuntu-latest

    strategy:
      matrix:
        node-version: [20.x]

    steps:
    - name: Checkout repository
      uses: actions/checkout@v3

    - name: Set up Node.js
      uses: actions/setup-node@v3
      with:
        node-version: ${{ matrix.node-version }}

    - name: Install dependencies
      run: |
        npm install -g pm2
        npm install

    - name: Start application with timeout
      run: |
        timeout 14520s npm run zokou

```


## Contributions 🤝

Les contributions à Zokou sont les bienvenues ! Si vous avez des idées pour de nouvelles fonctionnalités, des améliorations ou des corrections de bogues, n'hésitez pas à ouvrir une issue ou à soumettre une demande de pull. 🙌

### Remerciements :
- **Fatao**, qui a ajouté des commandes (Fancy, GPT, Dall-e, APK)  
- **CrazyPrice**, qui a hébergé un second site web pour les session_id  

## Licence 📜

Le Bot WhatsApp Zokou est publié sous la [Licence MIT](https://opensource.org/licenses/MIT).

Profitez des fonctionnalités variées du Bot WhatsApp Zokou pour améliorer vos conversations et rendre votre expérience WhatsApp plus intéressante ! 🎊💬

## Développeurs :
- [**Djalega++**](https://github.com/djalega8000/Zokou-MD/)
- [**᚛M๏𝓷keℽ D Lบffy᚜**](https://github.com/Faouz995)
