# Personal-Blog

Step 1: Install Hugo

```brew install hugo```

Step 2: Create a New Site 

```hugo new site quickstart```

Step 3: Add a Theme 
```
cd quickstart
git init
git submodule add https://github.com/budparr/gohugo-theme-ananke.git themes/ananke
```

Step 4: Add Some Content

```
hugo new posts/my-first-post.md
```

Step 5: Start the Hugo server 

```
hugo server -D
```

Navigate to your new site at http://localhost:1313/.

# Mastering Markdown:
https://guides.github.com/features/mastering-markdown/

# Basic writing and formatting syntax
https://help.github.com/en/github/writing-on-github/basic-writing-and-formatting-syntax
