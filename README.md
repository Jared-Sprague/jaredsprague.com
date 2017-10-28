# Jared Sprague blog

After cloning:

    npm install -g hexo-cli
    npm install

## Start a dev server

    hexo server

## Write a new post

    hexo new post "Hello World"

## Deploy

    npm run deploy

## Add a game or demo

Make a directory and copy the game/demo into it.

    mkdir source/game
    cp -r $GAME/src/* source/game

Then tell hexo not to process those files:

  1. editing `_config.yml`
  2. find the `skip_render` section
  3. add `- "game/**/*"`
  4. delete `db.json` if hexo refuses to build after this

The game should now be available at the `/game` path.
