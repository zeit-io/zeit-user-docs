# Google 

Google ist nicht nur eine Suchmaschine, sondern auch ein Cloud-Anbieter. 
Mit [Google Workspace](https://workspace.google.com/business/) bietet Google eine cloud-basierte Office-Suite an, samt E-Mail-Postfächer, Benutzerverwaltung und vieles mehr.

## Google SSO

Bei ZEIT.IO können Sie sich mit Ihrem bestehenden Google-Konto anmelden.
Dafür navigieren Sie einfach auf die [Anmelde-Seite von ZEIT.IO](https://zeit.io/de/signin) und klicken dort auf den Button "Mit Google anmelden". 
Sie werden dann weitergeleitet zu Google und Sie werden gefragt, ob Sie ZEIT.IO Zugriff auf Ihre Profilinformationen geben möchten. 
Wenn Sie dies bejahen, kann ZEIT.IO auf die folgenden Informationen ihres Google Kontos zugreifen:

- Vorname
- Nachname
- E-Mail-Adresse
- Profilbild

Wenn Sie noch kein Konto bei ZEIT.IO haben, dann werden diese Informationen verwendet, um ein neues Konto für Sie zu erstellen.
Wenn Sie bereits ein Konto bei ZEIT.IO haben, dann wird die E-Mail-Adresse aus Ihrem Google-Profil verwendet, um Sie bei ZEIT.IO anzumelden.

Das bietet viele Vorteile! So müssen Sie sich kein weiteres Passwort merken. 
Wenn Sie im Browser bereits bei Google angemeldet sind, dann können Sie sich mit einem Klick auch bei ZEIT.IO anmelden.

Für dieses SSO-Verfahren (Single-Sign-On) benutzen wir das [OAuth2 Protokoll](https://developers.google.com/identity/protocols/oauth2). 
