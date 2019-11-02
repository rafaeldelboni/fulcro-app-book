# fulcro-app-book
Repository to store the app I'm doing while following the fulcro book http://book.fulcrologic.com/fulcro3

## Setting Up

The shadow-cljs compiler uses all js dependencies through
NPM. If you use a library that is in cljsjs you will also have to add
it to your `package.json`.

You also cannot compile this project until you install the ones it
depends on already:

```
npm install
```

## Development Mode

Shadow-cljs handles the client-side development build. The file
`src/main/app/client.cljs` contains the code to start and refresh
the client for hot code reload.

In general it is easiest just to run the compiler in server mode:

```
npx shadow-cljs server
```

then *navigate to the server URL* (shown in this example as http://localhost:9630) and
use the *Builds* menu to enable/disable whichever builds you want watched/running.

Shadow-cljs will also start a web server for any builds that configure one.
