![Header - BetterJDocs](https://github.com/xMrAfonso/BetterJDocs/assets/44532605/572a4437-4b08-4447-8ec4-c473b7eac166)

This theme was specifically made to replace the old JavaDocs' Interface with a much needed improved version of its design & layout while being limited only to CSS.

If you want to check out a live demonstration, you may check [Hangar4J's JavaDocs](https://javadoc.jitpack.io/com/github/xmrafonso/hangar4j/63855dea54/javadoc/).

## How to install
1. Download the [stylesheet from GitHub](https://raw.githubusercontent.com/xMrAfonso/BetterJDocs/master/betterjdocs.css). (`betterjdocs.css`)
2. Place the file inside your project in a place of your choice.
3. Check below to see how to add the style to your project.
### Using Gradle:
```gradle
javadoc {
  // Your own configurations...
  options.stylesheetFile = file('path/to/betterjdocs.css')
}
```
### Using other methods:
- I only use Gradle, if you know how to do it in any other way, please consider contributing.

## How to customize
If you dislike the default colors, or just want to modify it to fit your own projects, you can _modify_ the colors by **opening the stylesheet**.

| Variable             | Description                                                          |
| -------------------- | -------------------------------------------------------------------- |
| --primary-color      | _Mostly used on links & buttons._                                    |
| --secondary-color    | _Used in fields, parameters, types, etc._                            |
| --description-color  | _Used specifically for descriptions and text._                       |
| --hover-color        | _Hover color for links._                                             |
| --bg-900-color       | _Color for Top Navigation and Cards._                                |
| --bg-800-color       | _Color used in the body's background._                               |
| --bg-700-color       | _Mostly used for the odd row in tables._                             |
| --bg-600-color       | _Mostly used for the even row in tables and used for the searchbar._ |

There are also comments explaining what each variable corresponds to and what it does inside the stylesheet. 

## Contact me
If you have any questions or feedback, please contact me via Discord: `@mrafonso`.
