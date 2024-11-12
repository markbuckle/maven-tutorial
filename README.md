## Build steps

Make sure maven is installed. Check with:

```pwsh
mvn -v
```

Install the maven wrapper.

```pwsh
mvn wrapper:wrapper
```

You should now see two mvnw files in your root folder. mvnw is for mac and
linux, mvnw.cmd is for windows. Once the wrapper files are installed you
technically do not need to have maven installed anymore.

Next check to ensure if it is a valid maven project (clean .xml file):

```pwsh
mvn validate
```

If you want to browse Maven libraries, check out https://search.maven.org

Next delete the target file with:

```pwsh
mvn clean
```

Next compile packages in src/ folder into the target/ folder and then test:

```pwsh
.\mvnw compile test
```

Next package your files:

```mvn
mvn package
```

Next put the java file in your local maven repository:

```mvn
mvn clean install
```
