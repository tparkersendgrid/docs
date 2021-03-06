---
seo:
  title: Two-Factor Authentication FAQ
  description: Find answers to commonly asked questions about our Two-Factor Authentication.
  keywords: 2FA, Two-Factor Authentication, Authentication, login, multifactor authentication
title: Two-Factor Authentication FAQ
weight: 0
layout: page
navigation:
  show: true
---

* [What is Two-Factor Authentication?](#-What-is-TwoFactor-Authentication)
* [How is this release of Two-Factor Authentication different from the Legacy Two-Factor Authentication?](#-How-is-this-release-of-TwoFactor-Authentication-different-from-the-Legacy-TwoFactor-Authentication)
* [Can I get locked out of my account by using Two-Factor Authentication? If this happens, how can I regain access?](#-Can-I-get-locked-out-of-my-account-by-using-TwoFactor-Authentication-If-this-happens-how-can-I-regain-access)
* [Can I use Two-Factor Authentication with multiple user credentials?](#-Can-I-use-TwoFactor-Authentication-with-multiple-user-credentials)
* [Will my multiple user credentials be supported on Two-Factor Authentication?](#-Will-my-multiple-user-credentials-be-supported-on-TwoFactor-Authentication)
* [What happens if I repeatedly attempt to log in with an invalid token?](#-What-happens-if-I-repeatedly-attempt-to-log-in-with-an-invalid-token)

{% anchor h2 %}
What is Two-Factor Authentication?
{% endanchor %}

Two-Factor Authentication is a security feature that requires you to provide an additional 7-digit code generated by the [Authy App](https://www.authy.com/), or sent to your phone, whenever you log into your account.

For more information on how you can get started using Two-Factor Authentication, please visit our [User Guide]({{root_url}}/User_Guide/Settings/two_factor_authentication.html).

{% anchor h2 %}
How is this release of Two-Factor Authentication different from the previous version?
{% endanchor %}

The previous version of Two-Factor Authentication would generate a 6-digit token delivered to your mobile device via SMS. You would then be required to submit this token to finish logging in. The functionality of the latest release of Two-Factor

Authentication remains largely the same. However, it now supports the use of the [Authy App](https://www.authy.com/) to generate a 7-digit authentication token.

**You may still resort to SMS if you encounter problems with the Authy App.**

Furthermore, the latest Two-Factor Authentication release also allows you to create multiple configurations so that you can authenticate with more than one device.

{% anchor h2 %}
Can I get locked out of my account by using Two-Factor Authentication? If this happens, how can I regain access?
{% endanchor %}

It is possible to lock yourself out of your account when using Two-Factor Authentication. Here are a couple of situations to be aware of:

* You lose your device configured with Authy, or your device runs out of power.
* You choose to only use SMS when retrieving authentication tokens, and you do not have cellular service.
* You choose to use Authy and SMS but have neither cellular service nor WiFi.
* You have a shared SendGrid account, but only one user has a mobile device configured with Two-Factor Authentication.

If you find that you’ve lost access to your account as a result of Two-Factor Authentication, please reach out to the [Authy Support Team](https://www.authy.com/faq/).

{% anchor h2 %}
Can I use Two-Factor Authentication with multiple user credentials?
{% endanchor %}

You can create multiple configurations of Two-Factor Authentication, allowing you to use more than one mobile device to authenticate when logging into your account. However, you cannot create multiple, distinct Two-Factor Authentication configurations to be used by multiple credentialed users.

The interaction between Two-Factor Authentication and multiple credentialed users has remained unchanged in the latest release. If Two-Factor Authentication is enabled and any multiple credentialed user attempts to log in, a notification will be triggered on the main credentialed user’s mobile device.

{% anchor h2 %}
Will my multiple user credentials be supported on Two-Factor Authentication?
{% endanchor h2 %}

Yes! Multiple user credentials can choose to have their own individual two-factor authentication.  

{% anchor h2 %}
What happens if I repeatedly attempt to log in with an invalid token?
{% endanchor %}

You may make no more than 3 requests to log in per minute. If you exceed this rate limit, you will receive a 503 Error response. Multiple unsuccessful attempts to log in will result in locking your account for a brief period of time. This time period will increase in duration as you continue to make unsuccessful login attempts.
