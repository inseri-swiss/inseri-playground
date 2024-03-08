# inseri Playground

[inseri Playground](https://inseri.swiss/playground/) relies on [WordPress Playground](https://github.com/WordPress/wordpress-playground) to provide a playground where the users can test [inseri core for WordPress](https://github.com/inseri-swiss/inseri-core-wp).

[Start inseri Playground](https://playground.wordpress.net/?blueprint-url=https://raw.githubusercontent.com/inseri-swiss/inseri-playground/main/blueprint.json) is using the [`blueprint.json`](blueprint.json), i.e.:  
https://playground.wordpress.net/?blueprint-url=https://raw.githubusercontent.com/inseri-swiss/inseri-playground/main/blueprint.json

## How to generate `inseriswiss.WordPress.xml`

1. Export all content from https://inseri.swiss/ -> Tools -> Export
2. Open an empty playground with the same wp and php version and theme https://playground.wordpress.net/?theme=twentytwentythree&wp=6.4&php=8.2
3. Remove all Posts and Pages
4. import the exported xml from step 1.
5. Remove all
   1. Posts and Pages: draft and private pages and posts
   2. Remove / Edit SiteHeader and Footer and the last 3 columns -> Save
6. Edit Site title: add "Playground - " in the front of "inseri core beta"
7. Save
8. Export all content from your local playground -> Tools -> Export
9. Update `inseriswiss.WordPress.xml` using the xml from step 8.
