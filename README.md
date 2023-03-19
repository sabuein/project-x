# prjctX

A community management system and tools for art collectors.

The project consists of:
- Front-end: Progessive web app (PWA) built with Bootstrap v[5.3.0-alpha1][bootstrap],
- Back-end: RESTful API built with Slim Framework v[4.11.0][slim], PHP v[8.1.2][php], and MariaDB v[10.6.12][mariadb].

```bash
$ composer show --direct 
selective/basepath 2.1.0  A URL base path detector for Slim 4
slim/psr7          1.6    Strict PSR-7 implementation
slim/slim          4.11.0 Slim is a PHP micro framework that helps you quickly write simple yet powerful web applications and APIs
```

## Local development:

```bash
# Start PHP built-in web server to run an API
cd ./core/apis/v1/collectors/ && sudo php -S localhost:8888 -t public public/index.php
cd /home/sabuein/my/projects/prjctX/core/apis/v1/collectors/ && sudo php -S localhost:8888 -t public public/index.php
```

### Web resources:

- Fetch API ([WHATWG][fetchwhat], [MDN][fetchmdn], [web.dev][fetchweb])
- Credential Management API ([MDN][creapimdn], [web.dev][creapiweb])
- Payment Request API ([W3C][payw3c], [MDN][paymdn], [web.dev][payweb], [Apple][payapple], [freeCodeCamp][payfreecode])
- Google Pay API ([Google][paygoogle])
- Stripe's payments APIs ([Payments][stripeapis], [CLI][stripcli], [SDK][stripephp])

### PHP resources:

- [rfc:request_response][rfc_rr]
- [PSR-4: Autoloader][psr4]
- [PSR-7: HTTP message interfaces][psr7]
- [PSR-15: HTTP Server Request Handlers][psr15]

[slim]: https://www.slimframework.com/2022/11/06/slim-4.11.0-release.html "Slim 4.11.0 released - Slim Framework"
[php]: https://www.php.net/releases/8_1_2.php "PHP: PHP 8.1.2 Release Announcement"
[mariadb]: https://mariadb.com/kb/en/mariadb-10-6-12-release-notes/ "MariaDB 10.6.12 Release Notes - MariaDB Knowledge Base"
[psr4]: https://www.php-fig.org/psr/psr-4/ "PSR-4: Autoloader - PHP-FIG"
[psr7]: https://www.php-fig.org/psr/psr-7/ "PSR-7: HTTP message interfaces - PHP-FIG"
[psr15]: https://www.php-fig.org/psr/psr-15/ "PSR-15: HTTP Server Request Handlers - PHP-FIG"
[fetchwhat]: https://fetch.spec.whatwg.org/ "Fetch Standard"
[fetchmdn]: https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API "Fetch API - Web APIs | MDN"
[fetchweb]: https://web.dev/introduction-to-fetch/ "Introduction to fetch()"
[creapimdn]: https://developer.mozilla.org/en-US/docs/Web/API/Credential_Management_API "Credential Management API - Web APIs | MDN"
[creapiweb]: https://web.dev/security-credential-management/ "The Credential Management API"
[payw3c]: https://www.w3.org/TR/payment-request/ "Payment Request API"
[paymdn]: https://developer.mozilla.org/en-US/docs/Web/API/Payment_Request_API "Payment Request API - Web APIs | MDN"
[payweb]: https://web.dev/how-payment-request-api-works/ "How Payment Request API works"
[payapple]: https://developer.apple.com/documentation/apple_pay_on_the_web/payment_request_api "Payment Request API | Apple Developer Documentation"
[stripeapis]: https://stripe.com/docs/payments/online-payments "Get started with Stripe APIs | Stripe Documentation"
[stripcli]: https://stripe.com/docs/stripe-cli/overview "Stripe CLI | Stripe Documentation"
[stripephp]: https://github.com/stripe/stripe-php "stripe/stripe-php: PHP library for the Stripe API"
[paygoogle]: https://developers.google.com/pay/api/web/overview "Overview  |  Google Pay API  |  Google Developers"
[payfreecode]: https://www.freecodecamp.org/news/payment-request-api-javascript/ "How to Use the Payment Request API in JavaScript"
[rfc_rr]: https://wiki.php.net/rfc/request_response "PHP: rfc:request_response"
[bootstrap]: https://getbootstrap.com/docs/5.3/getting-started/introduction/ "Get started with Bootstrap · Bootstrap v5.3"