# Wyam Blog Template

This template is created by unrolling the Blog recipe from the wyam tool.

The reason I wanted to do that is the recipe hid too much away from me for my tastes. Consequently, the config.wyam file is a *LOT* bigger as I put the recipe contents in it. The top part is using the config script, the bottom is the C# classes which allow the script to work.

More information on Wyam: https://wyam.io

Requirements:

* dotnet 2.x (I used 2.2)

To install:

### install the wyam cli tool

```bash
dotnet tool install -g Wyam.Tool
```

### ensure wyam in your path

```bash
wyam --help
```

### build site

```bash
wyam build
```

### preview site

```bash
wyam preview
```

### change theme

```bash
mv theme theme_bak
wyam build --theme <theme_name>
wyam preview
```

Themes can be seen here:

* https://github.com/Wyamio/Wyam/tree/master/themes/Blog

### edit config / build pipelines

* edit the config.wyam
* build
* preview

### edit theme

* edit files in theme folder
  * Note, that if you prefer a different base theme, just replace the theme files.
* build
* preview

## Note

I added the output folder to the .gitignore

If you prefer to store the generated site in your repository, you may want to remove that.
