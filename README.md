# php-debug

## Travail à faire 

Installation et configuration de Xdebug avec PHP

## Etapes 

1. Affichage de phpinfo dans le fichiers index.php

```
php -S localhost:8081
```

2. Trouver le fichier DLL

- https://xdebug.org/wizard

3. Configuration de fichier php.ini

```conf
[XDEBUG]
zend_extension="C:\php\ext\php_xdebug.dll"
xdebug.mode=debug
;xdebug.client_host = 127.0.0.1
;xdebug.client_port = 9003
xdebug.start_with_request=yes
```

Après la résolution d'un problème  #1

```conf
[XDebug]
zend_extension="C:\php\ext\php_xdebug.dll"
xdebug.mode = debug,develop
xdebug.discover_client_host = yes
xdebug.log_level = 0
xdebug.log = "%sprogdir%/userdata/temp/xdebug/log.txt"
xdebug.start_with_request = yes
xdebug.idekey = VSCODE
```



4. Installation de l'extention VS Code 
- PHP Debug


## Ressources
- [How to debug PHP in Visual Studio Code (Simple steps)](https://www.youtube.com/watch?v=8ka_Efpl21Y)
- [Setup debugging for PHP8.1 with XDebug 3 in VSCode](https://www.youtube.com/watch?v=HrQWtbxY1Hs)