git clone git@github.com:symfony/symfony-docs.git
cd symfony-docs
    <img git clone git@github.com:symfony/symfony-docs.git
cd symfony-docs


<h3 align="center">
  The official Symfony Documentation
</h3># Build HTML version
make html

# Or if you're on Windows
.\make.bat html


<p align="center">
  <a href="https://symfony.com/doc/current/index.html">
    Online version
  </a>
  <span> | </span>
  <a href="https://symfony.com/components"># Using Python's built-in server
cd _build/html
python -m http.server 8000

    Components
  </a>
  <span> | </span>
  <a href="https://symfonycasts.com">
    Screencasts
  </a>
</p>

Contributing
------------

We love contributors! For more information on how you can contribute, please read
the [Symfony Docs Contributing Guide](https://symfony.com/doc/current/contributing/documentation/overview.html).

> [!IMPORTANT]
> Use `6.4` branch as the base of your pull requests, unless you are documenting a
> feature that was introduced *after* Symfony 6.4 (e.g. in Symfony 7.2).

Build Documentation Locally
---------------------------

This is not needed for contributing, but it's useful if you would like to debug some
issue in the docs or if you want to read Symfony Documentation offline.

```bash
$ git clone git@github.com:symfony/symfony-docs.git

$ cd symfony-docs/
$ cd _build/

$ composer install

$ php build.php
```

After generating docs, serve them with the internal PHP server:

```bash
$ php -S wordpress:8000 -t output/
```

Browse `http://wordpress:8000` to read the docs.
