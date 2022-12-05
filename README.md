# Symfony-RestApi

## Prerequisitos
#### 1. Composer
#### 2. Mysql
#### 3. PHP >= 8.02

### Step 1 - Install Symfony 6 - Create project
>`composer create-project symfony/skeleton symfony-6-rest-api`

### Step 2 - Install packages
> `composer require jms/serializer-bundle`
> `composer require friendsofsymfony/rest-bundle`
> `composer require symfony/maker-bundle`     
> `composer require symfony/orm-pack`

### Step 3 - Configure FOSRest Bundle
#### Open the file ***config/packages/fos_rest.yaml***
> `fos_rest:`
>   `format_listener:`
>       `rules:`
>           `- { path: ^/api, prefer_extension: true, fallback_format: json, priorities: [ json, html ] }`

### Step 4 - 