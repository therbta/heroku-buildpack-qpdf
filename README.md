# Heroku Buildpack: QPDF

This is a custom Heroku buildpack that installs `qpdf` (version 12.2.0) into your dyno.

- Adds qpdf binary to `$PATH`
- Ready for use with Node.js apps via node-qpdf2

## Usage

1. Add the buildpack to your app:

```
heroku buildpacks:add https://github.com/yourusername/heroku-buildpack-qpdf.git -a your-app-name
```

2. Deploy your app:

```
git push heroku main
```

3. Verify:

```
heroku run bash -a your-app-name
qpdf --version
```

✅ Done!
