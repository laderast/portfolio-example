# Simple Hugo Portfolio Template

Simple hugo portfolio example derived from the forty theme. Designed to be used for Data Scientists sharing their R projects.

## Getting Started

To get started, click the green "Use This Template" to make a copy to your own GitHub account. 

Name your new repository, and click the "Create Repository From Template".

## Customizing

Almost all elements are edited within the `config.toml` file. At the bare minimum, these are the fields you should customize:

```
title = "Portfolio for Ted Laderas, PhD"
```

```
name = "Ted Laderas"
description = "Portfolio/CV for Ted Laderas"
```

Menu can be modified here.

```
  [params.navigation]
    title = "Ted Laderas, PhD"
    subtitle = "Data Scientist and Collaborator"
    menu = "Menu"
    # Optional logo as brand stored in img/
    # logo = "logo.png"

    [[params.navigation.links]]
      name = "Home"
      url = "#"

    [[params.navigation.links]]
      name = "Blog"
      url = "blogs"

```

Banner: 

```
  # Banner section
  [params.banner]
    # To change the background image on the homepage banner, replace 'banner.jpg' in
    # the 'static/img' folder.
    title = "Ted Laderas, PhD"
    subtitle = "Portfolio of Data Science and Visualization Projects"

```

Most importantly, Tiles, where you'll put individual projects and links! 

Add a project Rmarkdown by adding a folder in the `content/projects` directory, and name your 
RMarkdown html file `index.html` in the folder. Refer to the `url` as `projects/choropleth` (look in the `content/projects` folder for examples.)

Add an image for each tile in `static/image/projects/`, and refer to them in the `image` field as `projects/choropleth.png`.

```
 [params.tiles]
    enable = true
    # Display your showcases here.
    
    [[params.tiles.showcase]]
      title = "Choropleths for Ready for R Class"
      subtitle = "Understanding our email list by country domain"
      image = "projects/choropleth.png"
      url = "projects/choropleth"

    [[params.tiles.showcase]]
      title = "Animal Crossing Tidy Tuesday"
      subtitle = "Understanding Character and Animal Types in Animal Crossing"
      image = "projects/ac.png"
      url = "projects/animal_crossing"
```

Play around with this and update the fields. You'll have a portfolio up in no time!

## Next Step: Building on Netlify

[TBA]
