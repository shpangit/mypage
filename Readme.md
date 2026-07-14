# My page with Hugo

## Set-up
After installing *hugo*, the directory is initialized with:

```
    hugo new site mypage 
    git init
```

## Applying *hugo-coder* Theme
Adding the theme repo as submodule

```
    git submodule add https://github.com/luizdepra/hugo-coder.git themes/hugo-coder
```

Starting with the default template contents:
```
    cp themes/hugo-coder/exampleSite/hugo.toml .
```

## Starting Hugo server
```
    hugo server -D
```
The page will be available @ localhost:1313.  
*-D* option is for drafts.

## How to deploy on Github Page
1. Create a *.github/workflows/hugo.yaml* file.
2. Push the code
3. Setting the Deployment on Github repo (setting -> page). The repo must be in public visibility.