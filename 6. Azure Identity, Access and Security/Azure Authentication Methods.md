![](../Static/Pasted%20image%2020260929232344.png)


**Single Sign On (SSO)**
Sign in once and access multiple trusted apps. lowers chances of credential related incidents and reset overhead.
Access is tied to one identity, making it easier to update or remove access when roles change
Single sign-on is only as secure as the initial authenticator because the subsequent connections are all based on the security of the initial authenticator.

**Multifactor Authentication (MFA)**

prompts user for extra factor during sign-in like -
Something the user knows - a password
Something the user has - A code sent to phone
Something the user is - Biometric

**Microsoft Entra MFA -**
Users can choose an extra form of authentication like phone call, app notification

**Passwordless Authentication**
Eliminates password entirely. replacing with trusted device and a biometric signal or a pin.
After initial registration, the user signs in with a factor they know or are like PIN or fingerprint.

Entra ID supports 3 passwordless options - 
1. Windows Hello for Business
2. Microsoft authenticator
3. FIDO2 security keys
![](../Static/Pasted%20image%2020260929232910.png)

**Windows Hello for Business**

Ideal for workers with dedicated PC. Biometric and PIN are linked to user's PC. 
With public key infra (PKI) integration and built in support for SSO.

**Microsoft Authenticator**

Turns any phone into a strong sign-in factor

**FIDO2 Security Keys**

Open standard for passwordless authentication built on web authentication (WebAuthn) specification. These are unphishable hardware devices like USB, Bluetooth or NFC
Because hardware handles authentication, there's no password that can be exposed.
