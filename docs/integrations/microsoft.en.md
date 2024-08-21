# Microsoft 

Microsoft is a software manufacturer that now offers various cloud services.

## Microsoft Entra SSO

Microsoft Entra (formerly Microsoft AD) is a single sign-on (SSO) solution that allows users to log into various applications with a single account.
You can also log in to ZEIT.IO with your Microsoft account.
To do this, simply navigate to the [ZEIT.IO login page](https://zeit.io/de/signin) and click on the "Sign in with Microsoft" button.
You will then be redirected to Microsoft and asked if you want to give ZEIT.IO access to your profile information.
If you answer yes, ZEIT.IO can access the following information from your Microsoft account:

- First name
- Last name
- User name
- Email address
- Profile picture

If you do not yet have an account with ZEIT.IO, this information will be used to create a new account for you.
If you already have an account with ZEIT.IO, the email address from your Microsoft profile will be used to log you in to ZEIT.IO.

This offers many advantages! You don't have to remember another password.
If you are already logged in to Microsoft in your browser, you can log in to ZEIT.IO with one click.

For this SSO (Single Sign-On) process, we use the [OAuth2 protocol](https://learn.microsoft.com/de-de/entra/identity-platform/v2-oauth2-auth-code-flow).
