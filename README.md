![Header - BetterJDocs](https://github.com/xMrAfonso/BetterJDocs/assets/44532605/572a4437-4b08-4447-8ec4-c473b7eac166)

This theme was specifically made to replace the old JavaDocs' Interface with a much needed improved version of its design & layout while being limited only to CSS.

To check out a live demonstration, go to [Andre601's JavaDocs](https://jd.andre601.ch/asl-api/).

If you like this resource, don't forget to leave a **Star <3.**

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
### Using Maven:
```xml
<build>
    <plugins>
        <plugin>
            <groupId>org.apache.maven.plugins</groupId>
            <artifactId>maven-javadoc-plugin</artifactId>
            <version>3.4.1</version> <!-- Make sure to update if outdated -->
            <configuration>
                <!-- Your own configurations... -->
                <stylesheetfile>./path/to/betterjdocs.css</stylesheetfile>
            </configuration>
        </plugin>
    </plugins>
</build>
```

<details><summary>Multi-module setup (Based on Maven docs example)</summary>
<p>

You set this in the root/parent `pom.xml` and use `mvn javadoc:aggregate`
```xml
<build>
    <pluginManagement>
        <plugins>
            <plugin>
                <groupId>irg.apache.maven.plugins</groupId>
                <artifactId>maven-javadoc-plugin</artifactId>
                <version>3.4.1</version> <!-- Make sure to update if outdated -->
            </plugin>
        </plugins>
    </pluginManagement>
    <plugins>
        <plugin>
            <groupId>org.apache.maven.plugins</groupId>
            <artifactId>maven-javadoc-plugin</artifactId>
            <version>3.4.1</version> <!-- Make sure to update if outdated -->
            <configuration>
                <!-- Your own configurations... -->
                <stylesheetfile>./path/to/betterjdocs.css</stylesheetfile>
            </configuration>
        </plugin>
    </plugins>
</build>
```

</p></details>

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

### Color Palettes
<details><summary>Dark Mode (Default)</summary>

```css
/* Mostly used on links & buttons */
--primary-color: #4186f5;
/* Used in fields, parameters, types, etc. */
--secondary-color: #ffffff;
/* Used specifically for descriptions and text */
--description-color: #949494;
/* Hover color for links */
--hover-color: #76a6f4;
/* Color for Top Navigation and Cards */
--bg-900-color: #121212;
/* Color used in the body's background */
--bg-800-color: #171717;
/* Mostly used for the odd row in tables */
--bg-700-color: #1c1c1c;
/* Mostly used for the even row in tables and used for the searchbar */
--bg-600-color: #212121;
```

</details>

<details><summary>Light Mode</summary>

```css
/* Mostly used on links & buttons */
--primary-color: #185bc7;
/* Used in fields, parameters, types, etc. */
--secondary-color: #000000;
/* Used specifically for descriptions and text */
--description-color: #3f3e3e;
/* Hover color for links */
--hover-color: #76a6f4;
/* Color for Top Navigation and Cards */
--bg-900-color: #f0f0f0;
/* Color used in the body's background */
--bg-800-color: #e0e0e0;
/* Mostly used for the odd row in tables */
--bg-700-color: #d0d0d0 ;
/* Mostly used for the even row in tables and used for the searchbar */
--bg-600-color: #c0c0c0;
```

</details>

## Contact me
If you have any questions or feedback, please contact me via Discord: `@mrafonso`.
