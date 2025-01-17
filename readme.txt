=== Login using cidaas ===

Contributors : gopimallela
Tested up to: 5.7
Tags: Single Sign On, SSO, Login, Authentication, Authorization, CIAM, OpenID Connect, OIDC, OAuth, OAuth 2.0
Stable tag: trunk
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Striking the perfect balance between security and comfort - unique user identification and the highest level of security

== Description ==

The perfect identity platform to manage customers, partners and employees, [cidaas](https://www.cidaas.com) lets you intelligently take care of identities securely without compromising on user experience. cidaas stands for "Cloud Identity and Access Management System" and delivers an out-of-the-box solution for standardized Identity Management and Access Control. The cidaas software offers Scalability, Security, Transparency & Flexibility and supports seamless integration into your existing software.

The appearance of the cidaas User Interfaces (e.g. login), including language, authentication and authorization settings, can be configured in cidaas Admin UI. In cidaas you have the option to:

* Select from more than 14 different *authentication options*
* Enable *Multi-Factor-Authentication* to increase security or fulfill regulatory requirements
* Configure *Consent Management* (for GDPR compliance)
* Enable Social Logins (e.g. Facebook, Google, Sign in with Apple)
* Allow *passwordless authentication*
* And more

[Watch our video](https://www.youtube.com/watch?v=wUP4xV-RxCY)

== Technical Notes ==

This plugin is using the OpenID Connect and OAuth 2.0 protocol to integrate cidaas, in particlar the Authorizaton Code Flow. The authentication and authorization are implemented through cidaas. After a successful authentication, the user information is stored in the Wordpress database. **Only the user information is stored in Wordpress, no authentication details (e.g. passwords) are transmitted**.

After configuring the plugin, you can integrate cidaas with a shortcode [cidaas_login_button]

== Installation ==

To use this plugin you need a cidaas plan, all detais about our free and paid plans you can find on the [cidaas pricing page](https://www.cidaas.com/pricing-packages/)

You can find an installation guide in our [docs](https://docs.cidaas.de/plugin/cidaas_for_wordpress.html)

== Frequently Asked Questions ==

= What is the client's Redirect URI? =

cidaas requires a whitelisting of a set of redirect URIs for security purposes. The Redirect URI used
by this plugin looks like this:  https://example.com/wp-admin/admin-ajax.php?action=openid-connect-authorize

Replace `example.com` with your domain name and path to WordPress.

= What social login providers do you provide and how can they be activated? =

cidaas provides many different social login providers. Select the providers that fits best to your use cases and configure them in cidaas. A list of social login providers and how to configure them can be found in the [cidaas documentation](https://docs.cidaas.de/configuration-settings/social-providers.html)

= How can I customize the cidaas User Interfaces? =

The cidaas User Interfaces are managed with the *Hosted Pages* concept. All cidaas user interfaces can be fully customized, for more information see the [Hosted Pages documentation](https://docs.cidaas.de/configuration-settings/hosted-pages.html)

