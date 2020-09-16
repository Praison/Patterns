# WordPress Block Patterns Plugin

New Block Patterns to Gutenberg.

## Description

This plugin contains patterns for you to check out, ranging from a simple text pattern to a more complex pattern containing both images and text.

## Add your block patterns to this plugin

1. Fork
```
https://github.com/Praison/Patterns
```

2. Clone your new fork locally
```
git clone https://github.com/YOUR_USERNAME/Patterns.git
cd Patterns
```

3. Connect to original repository https://github.com/Praison/Patterns
```
git remote add --track master upstream https://github.com/Praison/Patterns.git
git fetch upstream
```
4. Create a new branch for your changes
```
git checkout -b YOUR_USERNAME upstream/master
```

5. Add your block patterns in ``index.php``
```
register_block_pattern(
'praison-gutenberg-block-patterns/TITLE-OF-YOUR-BLOCK-PATTERN',  # Add Hyphens between lowercase words
array(
    'title'   => __( 'TITLE_OF_YOUR_BLOCK_PATTERN', 'praison-gutenberg-block-patterns' ),
    'content' => "BLOCK_PATTERN_GOES_HERE",
    'categories' => array("CATEGORY"), # eg: columns, text ..etc
)
);
```

6. Add, Commit, Push
```
git add .
git commit -m "Added block pattern TITLE_OF_YOUR_BLOCK"
git push -u origin YOUR_USERNAME
```

7. Submit your [pull request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request "Creating Pull Request")   


## Installation

1. Download the zip file
2. Extract the contents
3. Upload the folder `patterns` to your WP plugin folder `/wp-content/plugins/` directory
4. Go to Plugins > Plugins, and activate the plugin

## Patterns

This plugin contains patterns for you to check out, ranging from a simple text pattern to a more complex pattern containing both images and text.

### Intro Paragraph with Two Columns

![intro-paragraph-two-columns](https://user-images.githubusercontent.com/2846578/77936659-38f2b800-7281-11ea-9be8-4e33fe3e1fbd.png)

- Column block
  - 80% column with 28px paragraph
  - 20% empty column
- Column block
  - 50% column with paragraph
  - 50% column with paragraph

### An Article Introduction

![article-introduction](https://user-images.githubusercontent.com/2846578/77936648-34c69a80-7281-11ea-8c17-74063118242c.png)

- Centered bold paragraph, 16px, for the category or topic
- Centered h1 for the article title
- Centered paragraph, 48px, for the byline
- Centered paragraph, 28px, for an introductory paragraph

### River Gallery with Text

![river-gallery-with-text](https://user-images.githubusercontent.com/2846578/77939696-8d983200-7285-11ea-8699-ccffed67241c.png)

- Column block
  - 33% column with spacer bock, large image, and an image resized to 25%
  - 33% column with image resized to 25%, and large image
  - 33% column with spacer, h2, and paragraphs
