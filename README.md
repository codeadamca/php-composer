# php-composer
A basic example of using Composer to manage PHP packages.

Follow these steps to install Composer:

1. Using the command line, download Composer:

```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
```

2. Instal the download:

```
php composer-setup.php
```

3. Then delete the original download:

```
php -r "unlink('composer-setup.php');"
```

At this point Composer will work, but only in this folder. So we want to move Composer so that the ```composer``` command will work from any folder using the Command Line.

On a Mac, move the ```composer.phar``` file to ```/usr/local/bin/```: 

```
sudo mv composer.phar /usr/local/bin/composer
```

On a Windows machine, use the installer and the ```composer``` file will work from any folder.

## Set up a New Project

Now let's use Composer to download some PHP packages for a new project. 

1. Create a new folder for a new project.
2. Using the command line, navigate to your new folder.
3. Run the ```composer init``` command.
4. Walk through the questions (use the dfault answers or provide information if needed) until you needs to search for a package, then use the package ```wideimage```. It will be on the list as item 0 as ```cmottt/wideimage```.
5. Then provide the version "^1.1.4".
6. When the command line asks you to search again, just hit enter and it will move on.
7. Accept the next few defauts. It will show you want the ```package.json``` file will look like, keep continuing. 

Once the ```composer init``` command is complete you will see new ```vendor``` folder and a composer.json. 

From here you can add additional dependencies in the ```composer.json``` file.


## Requirements:

* [Visual Studio Code](https://code.visualstudio.com/)
* [Composer](https://getcomposer.org/)
* [WideImage](https://packagist.org/packages/smottt/wideimage)
* [dompdf](https://packagist.org/packages/dompdf/dompdf)

<a href="https://codeadam.ca">
<img src="https://codeadam.ca/images/code-block.png" width="100">
</a>
