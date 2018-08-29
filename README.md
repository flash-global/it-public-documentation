### Default

- MySql 5.7 
- Ubuntu 16.04.1 
- Apache 2.4.18 
- PHP 7.0.30 
- MySQL 5.7 
- Memcached 1.4.25 
- React &gt;= 16.4 
    - Used with single page app 

### Accepted (if justified)

- Redis 4.0 Only for Pub/Sub 
- SolR 7.4 
- NodeJs 8.11 LTS Only for WebSocket 

### Code quality

#### PHP

- Unit test &gt;= 80% coverage business code 
- [phpcs except line length](https://github.com/flash-global/it-public-documentation/blob/master/configurations/phpcs.xml) 

- Functionals tests are encouraged 
- Use [Grumph](https://github.com/phpro/grumphp) is encouraged [grumphp.yml](https://github.com/flash-global/it-public-documentation/blob/master/configurations/grumphp.yml) 

JS

- [ESLint](https://github.com/flash-global/it-public-documentation/blob/master/configurations/.eslintrc.json) 
- EcmaScript 6 
- [BABEL compatibility IE6](https://github.com/flash-global/it-public-documentation/blob/master/configurations/.babelrc) 
- Webpack 
- Jest 

## Documentation

Use [README template](https://github.com/flash-global/it-public-documentation/wiki/Project-readme-template)

#### API

All endpoint need to be documented

- Create [Postman](https://www.getpostman.com/collection) collection and add it to repo 
- Create documentation via [Postman documentation](https://www.getpostman.com/docs/v6/postman/api_documentation/viewing_documentation) or [Apiary](https://apiary.io/) 

## Installation

Use state less developpement prepared to load balancing. Installation via Phing (read [https://github.com/flash-global/phing-service](https://github.com/flash-global/phing-service)) vendor/bin/phing -f phing.xml local-setup-system

### Git dependancies

Use vcs link to composer.json

```
"repositories": [
    {
      "type": "vcs",
      "url": "https://github.com/flash-global/my-lib"
    }
  ]
```

## Infra
![](https://github.com/flash-global/it-public-documentation/raw/master/img/infra%20architecture.png)
## Services independent

We have a partnership with [Yoctu](https://www.yoctu.com/) we use [their services](https://www.yoctu.com/services/)

- Logger 
    - [GitHub](https://github.com/flash-global/logger-client) 
    - [packagist](https://packagist.org/packages/fei/logger-client) 

- Audit 
    - [GitHub](https://github.com/flash-global/audit-client) 
    - [packagist](https://packagist.org/packages/fei/audit-client) 

- Mailer 
    - [GitHub](https://github.com/flash-global/mailer-client) 
    - [packagist](https://packagist.org/packages/fei/mailer-client) 

- Filer 
    - [GitHub](https://github.com/flash-global/filer-client) 
    - [packagist](https://packagist.org/packages/fei/filer-client) 

- Translate 
    - [GitHub](https://github.com/flash-global/translate-client) 
    - [packagist](https://packagist.org/packages/fei/translate-client) 
    - [npmjs](https://www.npmjs.com/package/translate-client-js) 

- PDF-generator 
    - [GitHub](https://github.com/flash-global/pdf-generator-client) 
    - [packagist](https://packagist.org/packages/fei/pdf-generator-client) 

- Connect 
    - [GitHub](https://github.com/flash-global/connect-client) 
    - [packagist](https://packagist.org/packages/fei/connect-client) 

- Notification 
- payment 
- Chat
