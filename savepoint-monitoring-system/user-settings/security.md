# Security

## Security <a id="security"></a>

On the _Security_ tab of the [user settings dialog](https://docs.wialon.com/en/hosting/user/set/set) you can make the authorization settings and enable two-factor authorization.

![](https://docs.wialon.com/en/hosting/_media/set/set2.png)

### Authorization settings <a id="authorization_settings"></a>

**E-mail**  
An e-mail address is required to recover the password in case it is lost and to receive a verification code when the two-factor authentication is enabled.

**Change password**  
Type in your current password, and then your [new password](https://docs.wialon.com/en/hosting/cms/users/props?&#general) \(twice\). Click _OK_ to save.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) Attention! No every user at the time of its creation is provided with the right to change the password.

### Two-factor authentication <a id="two-factor_authentication"></a>

To enable two-factor authentication, in the drop-down menu select the method of receiving the confirmation code: via e-mail or by SMS.

**Via e-mail**  
The code is sent to the e-mail address specified in the authorization settings. To confirm the address, press _Send e-mail_ and enter the received code in the line that appears.

![](https://docs.wialon.com/en/hosting/_media/set/set2email.png)

**Via SMS**  
Specify the phone number to which you want the code to be sent. To confirm the phone number, press _Send SMS_ and enter the received code in the line that appears. Standard rates apply for SMS messages.

![](https://docs.wialon.com/en/hosting/_media/set/set2sms.png)

In order to receive text messages, you should activate the [_SMS Messages_](https://docs.wialon.com/en/hosting/cms/accounts/services) service in the account properties and the [_Can send SMS_](https://docs.wialon.com/en/hosting/cms/users/props) function in the user properties.

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) If an SMS cannot be sent \(for example, the service is disabled or the number of available text messages is exceeded\), the confirmation code is sent to the e-mail specified in the authorization settings.

### Advanced settings <a id="advanced_settings"></a>

**Notify about account blocking by e-mail**

Activate this option to receive notifications about account blocking to the e-mail address specified in [user properties](https://docs.wialon.com/en/hosting/cms/users/props#advanced). Notifications start arriving daily 5 days prior to blocking.  
![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) To work with this option, activate the [_Е-mail notifications_](https://docs.wialon.com/en/hosting/cms/accounts/services) service in the account properties.

### flespi settings <a id="flespi_settings"></a>

![:!:](https://docs.wialon.com/en/hosting/lib/images/smileys/icon_exclaim.gif) The _flespi settings_ section is available only to the top users.

**Authorization**

To obtain a token, log in to flespi using one of the available methods \(Facebook, GitHub, Google, Microsoft, flespi\).

**Token**

This field with the generated token appears after successful authorization in flespi. The token is valid for 1 year. To make sure it is not expired, press _Check_. As a result, a tooltip with the information about the status \(active/expired\) and the expiration date of the token shows up. If necessary, the token can be edited manually.  


