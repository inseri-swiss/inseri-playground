# Issue Report

see https://github.com/WordPress/wordpress-playground/issues/1211

The content is generated using https://playground.wordpress.net/?theme=twentytwentythree&wp=6.5&php=8.2&plugin=wordpress-importer&plugin=inseri-core where a new post is created. The post is exported in the [issue.xml](issue.xml).

issue report:

## Expected behaviour:

1. Download [issue.xml](issue.xml)
2. Open https://playground.wordpress.net/?theme=twentytwentythree&wp=6.5&php=8.2&plugin=wordpress-importer&plugin=inseri-core
3. Admin UI: Tools -> Import -> Run Importer -> WordPress Run Importer -> Select the [issue.xml](issue.xml) file downloaded previously
4. Check the Issue post and notice the "#test" content

## Issue in Query API `import-wxr`

1. Try the xml: https://playground.wordpress.net/?theme=twentytwentythree&wp=6.5&php=8.2&plugin=wordpress-importer&plugin=inseri-core&import-wxr=https://raw.githubusercontent.com/inseri-swiss/inseri-playground/main/issue/issue.xml
2. Select the Issue post. You can notice that the block "is loading..." . In edit mode you can try to Attempt Block Recovery. The content looks like "u0022#testu0022".

The issue is present also in the blueprint.
