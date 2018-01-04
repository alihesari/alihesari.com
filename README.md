# alihesari.com

This is the home of my blog published in two languages. This repo uses [Mira](https://miraxy.github.io/) a static website generator written in Perl.

## How to use?

1- Install Mira:
    - [Mira on Github](https://github.com/kiamazi/mira#install)
    - [Mira documents](https://miraxy.github.io/)

2- Clone this repository
``` bash
git clone https://github.com/alihesari/alihesari.com.git
```

3- Configuration and Edit `config.yml`, `config\en.yml`, and `config\fa.yml`

4- Build your blog
```bash
$ mira new -t "Hello world" -f "en"   # creat new post
$ mira build                          # Build contents
$ mira view                           # serve locally at http://localhost:5000
```

## License

Licensed under the [MIT License](LICENSE).

Content is licensed under [CC BY-NC-ND 3.0](https://creativecommons.org/licenses/by-nc-nd/3.0/)

