# Holy Spirit Home

Site web et serveur Flask permettant de recevoir les sujets de prière et de les envoyer par e-mail.

## 🚀 Déploiement local

1. Crée un fichier `.env` avec :
   ```
   MAIL_USERNAME=goitatoperetsin@gmail.com
   MAIL_PASSWORD=pclojkbsdtskrwne
   RECEIVER_EMAIL=goitatoperetsin@gmail.com
   SECRET_KEY=holyspirit2024
   ```
2. Installe les dépendances :
   ```bash
   pip install -r requirements.txt
   ```
3. Lance le serveur :
   ```bash
   python app.py
   ```
4. Ouvre [http://localhost:5000](http://localhost:5000)

## ☁️ Déploiement sur Render

- Connecte ton dépôt GitHub.
- Choisis un nouveau service **Web**.
- Commande de démarrage :
  ```bash
  gunicorn app:app
  ```
- Configure les variables d’environnement avec les mêmes valeurs que dans ton `.env`.

Le site sera alors en ligne et le formulaire enverra les sujets de prière à ton Gmail.
