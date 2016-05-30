# buenosairestech.org

Web page for buenosairestech.org

# Dependencies

## Cactus

You can easily build the site using [Cactus](https://github.com/koenbok/Cactus). You can install it by running:

```bash
  git clone https://github.com/koenbok/Cactus
  cd Cactus/cactus
  sudo easy_install cactus
```

More info [here](https://github.com/koenbok/Cactus)

## Files structure

```
  - .build                Generated site (upload this to your host)
  - pages                 Your actual site pages
      - index.html
      - sitemap.xml
      - robots.txt
      - error.html        A default 404 page
  - templates             Holds your django templates
      - base.html
  - static                Directory with static assets
      - images
      - css
      - js
  - plugins               A list of plugins
```

## Run locally

You need to build the site with [Cactus](https://github.com/koenbok/Cactus). For this run:

```bash
  cactus serve
```

Then open [http://127.0.0.1:8000](http://127.0.0.1:8000)

## Deploy

Run:

```bash
  cactus deploy
```

The first time it will ask for your AWS S3 information. Be careful because the information will be saved in the [config.json](config.json). Thats why the file is in the [.gitignore](.gitignore). You can copy the [config.json.sample](config.json.sample) to start.

