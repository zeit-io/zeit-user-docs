# Microsoft 

Microsoft ist ein Softwarehersteller, der mittlerweile verschiedene Cloud-Dienste anbietet.

## Microsoft Entra SSO

Microsoft Entra (Früher Microsoft AD) ist eine Single Sign-On (SSO)-Lösung, die es Benutzern ermöglicht, sich mit einem einzigen Konto bei verschiedenen Anwendungen anzumelden.
Bei ZEIT.IO können Sie sich auch mit Ihrem Microsoft-Konto anmelden.
Dafür navigieren Sie einfach auf die [Anmelde-Seite von ZEIT.IO](https://zeit.io/de/signin) und klicken dort auf den Button "Mit Microsoft anmelden".
Sie werden dann weitergeleitet zu Microsoft und Sie werden gefragt, ob Sie ZEIT.IO Zugriff auf Ihre Profilinformationen geben möchten.
Wenn Sie dies bejahen, kann ZEIT.IO auf die folgenden Informationen ihres Microsoft Kontos zugreifen:

- Vorname
- Nachname
- Benutzername
- E-Mail-Adresse
- Profilbild

Wenn Sie noch kein Konto bei ZEIT.IO haben, dann werden diese Informationen verwendet, um ein neues Konto für Sie zu erstellen.
Wenn Sie bereits ein Konto bei ZEIT.IO haben, dann wird die E-Mail-Adresse aus Ihrem Microsoft-Profil verwendet, um Sie bei ZEIT.IO anzumelden.

Das bietet viele Vorteile! So müssen Sie sich kein weiteres Passwort merken.
Wenn Sie im Browser bereits bei Microsoft angemeldet sind, dann können Sie sich mit einem Klick auch bei ZEIT.IO anmelden.

Für dieses SSO-Verfahren (Single-Sign-On) benutzen wir das [OAuth2 Protokoll](https://learn.microsoft.com/de-de/entra/identity-platform/v2-oauth2-auth-code-flow). 
