# Sinix

Build games for Sinix with [Joystick](https://github.com/sinix-dev/sinix-android) support

# Installation and Setup

```bash
$ npm install sinix --save
```

Add script in `package.json`

```json
"scripts": {
  "sinix": "sinix",
}
```

Initialize a Sinix project
```
$ npm run sinix init
```

This will create `sinix.config.js` in the current directory. By default, sinix packages
the content of `dist/` directory, update the `distDir` value in `sinix.config.js`
as per your project.

### Build and Publish
Generates `app.dext` file in `release` folder, which you can open in [Sinix](https://github.com/sinix-dev/sinix)
or publish on Sinix.
```
$ npm run sinix build
```

It is also possible to publish directly from the command-line using following command.
```
$ npm run sinix publish
```

will prompt for `token` and `password` which can be retrieved from the account created on [sinix.dev](https://sinix.dev). The application
will go live in under 24 hours on [Sinix Store](https://sinix.dev/store).
