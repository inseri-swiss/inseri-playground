# inseri Playground

[inseri Playground](https://zi.uzh.ch/whp/science-it/inseri/playground/) relies on [WordPress Playground](https://github.com/WordPress/wordpress-playground) to provide a playground where the users can test [inseri core for WordPress](https://github.com/inseri-swiss/inseri-core-wp).

[Start inseri Playground](https://playground.wordpress.net/?blueprint-url=https://raw.githubusercontent.com/inseri-swiss/inseri-playground/main/blueprint.json) is using the [`blueprint.json`](blueprint.json), i.e.:  
https://playground.wordpress.net/?blueprint-url=https://raw.githubusercontent.com/inseri-swiss/inseri-playground/main/blueprint.json

## How to generate `inseriswiss.WordPress.xml`

1. Export all content from https://zi.uzh.ch/whp/science-it/inseri/ -> Tools -> Export
2. Open an empty playground with the same wp and php version and theme https://playground.wordpress.net/?theme=twentytwentythree&wp=6.7&php=8.1&plugin=wordpress-importer
3. Remove all Posts and Pages
4. Tools -> Import the exported xml from step 1.
5. Remove the **draft** and **private** Posts and Pages
6. Edit SiteHeader

- move the Search from the Header before the Title, in the same group,
- remove Header
- edit Site title: add "Playground - " in the front of "inseri core beta"
- Save

11. Export all content from your local playground -> Tools -> Export
12. Update `inseriswiss.WordPress.xml` using the xml from step 8.
