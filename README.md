# About

This project uses Foundation email CSS framework to build email templates, for more details about Foundation please check out [Foundation Email doc](foundation-email.md).

The background is described in this [JIRA ticket ABU-3113](https://aftership.atlassian.net/browse/ABU-3113), as we just build HTML template and not responsible for Email delivery service.

Ask @h.zhang and @l.sun (Data team) for email sending details.

What you need to do is:

```bash
# install dep
$ yarn

# modify the `src/pages/[page-name].html`

# run dev mode (output not minified), and check the output HTML at http://localhost:3000
$ yarn start
# run prod mode (output minified)
$ yarn build
```

Get the output HTML in `dist/[page-name].html`.

See more [examples] in `./src/pages/examples`.

Happy coding :tada:


## When you dev the Dropshipping email

Should run `yarn start:dps` instead of `yarn start`

It will watch file changes and output the un-minified html to `/dist`

Note that the watch only affect on the entry file, updating the partial .mjml or css file may not trigger.