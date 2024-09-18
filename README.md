# Python
-  Préparer son environnement de développement (Python3.11; PIP; Unix)


-  S'arruser que le workflow fonctionne bien
-  Développer des tests
-  automatiser les tests dans Docker
-  Finir le TP CODE CI


docker build -t fastapi-demo .
sudo docker-compose -f docker-compose.yml up


## Etape pour configurer son répo GIT en local:
- créer une clé ssh
  - ssh-keygen -t ed25519 -C "yanis.riguet@gmail.com"
 - eval "$(ssh-agent -s)"
 - ssh-add ~/.ssh/id_ed25519
 - cat ~/.ssh/id_ed25519.pub (copier l'entiereté de la clé et l'insérer dans son compte github)
   
- git clone https://github.com/yan-rig/Python.git
- git add . (pour add les fichiers du le répétoire dans le rép)
- git commit -m "commit"
- git push origin main (dans le cas ou il y a un pb de login/password, générer un token sur github et le renseigner à la place du password)
- git config --global user.name "yan-rig"
- git config --global user.email "yanis.riguet@gmail.com"
- git config --global credential.helper store (plus besoin de se loguer H24 quand on push)

