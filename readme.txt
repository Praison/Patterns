=== Block Patterns ===
Contributors: mervinpraison
Donate Link: https://goo.gl/Q4oiBG
Tags: gutenberg, blocks, block, pattern, patterns, block patterns, block pattern, blocks pattern, blocks patterns,
Requires at least: 5.0
Tested up to: 5.5.1
Stable tag: trunk
License: GPLv2 or later

New Block Patterns to Gutenberg.

== Description ==

This plugin contains patterns for you to check out, ranging from a simple text pattern to a more complex pattern containing both images and text.

= Add your block patterns to this plugin =

1. Fork
    `
https://github.com/Praison/Patterns
    `

2. Clone your new fork locally
    `
git clone https://github.com/YOUR_USERNAME/Patterns.git
cd Patterns
    `

3. Connect to original repository https://github.com/Praison/Patterns
    `
git remote add --track master upstream https://github.com/Praison/Patterns.git
git fetch upstream
    `
4. Create a new branch for your changes
    `
git checkout -b YOUR_USERNAME upstream/master
    `

5. Add your block patterns in ``index.php``
    `
register_block_pattern(
    'praison-gutenberg-block-patterns/TITLE-OF-YOUR-BLOCK-PATTERN',  # Add Hyphens between lowercase words
    array(
        'title'   => __( 'TITLE_OF_YOUR_BLOCK_PATTERN', 'praison-gutenberg-block-patterns' ),
        'content' => "BLOCK_PATTERN_GOES_HERE",
        'categories' => array("CATEGORY"), # eg: columns, text ..etc
    )
);
    `

6. Add, Commit, Push
    `
git add .
git commit -m "Added block pattern TITLE_OF_YOUR_BLOCK"
git push -u origin YOUR_USERNAME
    `

7. Submit your [pull request](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/creating-a-pull-request "Creating Pull Request")   


== Installation ==

= Steps =

1. Download the zip file
2. Extract the contents
3. Upload the folder `patterns` to your WP plugin folder `/wp-content/plugins/` directory
4. Go to Plugins > Plugins, and activate the plugin

== ChangeLog ==

= Version 1.0 =

* First release