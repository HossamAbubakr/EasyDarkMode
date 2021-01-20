# EasyDarkMode, Csharp Theme Engine

![Showcase.gif](/Showcase.gif)

## Table of Contents

* [Summary](#Summary)

* [Features](#Features)

* [Usage](#Usage)

* [Customization](#Customization)

* [Extras](#Extras)



## Summary

While I was making on my router management app I wanted to implement darkmode in an elegant way that is simple but none of the solutions suited my need so I made my own!


## Features

1. Easily integratable.

2. Simple to use.

3. Can force flat style (recommended) on all controls automatically.

4. Applicable to the entire project or a single form.

5. Highly customizable.

## Usage

You can get the engine up and running in 2 simple steps.

1. Set the theme you want.
```csharp
Theme.LightTheme();
```
```csharp
Theme.DarkTheme();
```

2. Call the Update theme function and pass in the form and voila!
```csharp
Theme.UpdateTheme(form: this);
```

## Customization

- Pass a custom color palette to your theme.
```csharp
Theme.CustomTheme(formBack: Color.White, controlBack: Color.Gray, controlFore: Color.Black);
```
- Use default winforms styling (flat style is on by default and is recommended)
```csharp
Theme.UpdateTheme(form: this, flatStyle: null);
```

## Extras

If your application uses images that you would like to turn into greyscale for darkmode you can use.
```csharp
imageGreyscale(SourceImage);
```
And the returned image will be greyscale. Please do note that this feature carries a relatively high performance impact if used with large images as it goes pixel by pixel.   
So its best suited for small images and pictures
