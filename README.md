# Binford® Tools: Composer 

Provides custom packages for [Binford® Tools][1]. 

## Intro  

A custom [Composer][2] repository that is built with [Satis][3] and publicly hosted via [GitHub Pages][4].

[https://binford-tools.github.io/composer/][5]

## How to use

If your package depends on other packages provided by this repository, just add the repository to your package’s `composer.json`. 

```json
{
    "repositories":
    {
        "binford-tools.github.io": 
        {
            "type": "composer",
            "url":  "https://binford-tools.github.io/composer/"        
        }
    }
}
```

### Attention

Keep in mind that Composer [can’t resolve repositories recursively][6], so you might have to add the repository to your [root package][7] as well.

## How to build

Install dependencies and build via Composer.

```sh
$ composer install
$ composer build
```

## We’re hiring!

We’re currently looking for passionate ~~masochists~~ **PHP & Magento developers** to join our e-commerce team **in Munich**. Sounds interesting? Just drop me a line via [j.scherbl@techdivision.com][8].

[1]: https://github.com/binford-tools
[2]: https://getcomposer.org
[3]: https://github.com/composer/satis
[4]: https://help.github.com/en/github/working-with-github-pages
[5]: https://binford-tools.github.io/composer/
[6]: https://getcomposer.org/doc/faqs/why-can%27t-composer-load-repositories-recursively.md
[7]: https://getcomposer.org/doc/04-schema.md#root-package 
[8]: mailto:j.scherbl@techdivision.com
