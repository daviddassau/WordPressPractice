# Integrate Bootstrap Into Your Child Theme

Essentially, all you have to do to integrate the Bootstrap 4 CDNs into your child theme is to make sure your `functions.php` file looks like this...

```PHP
<?php
function my_theme_enqueue_styles() {

    $parent_style = 'parent-style'; // This is 'twentyseventeen-style' for the Twenty Seventeen theme.

    wp_enqueue_style( $parent_style, get_template_directory_uri() . '/style.css' );
    wp_enqueue_style( 'child-style',
        get_stylesheet_directory_uri() . '/style.css',
        array( $parent_style ),
        wp_get_theme()->get('Version')
    );
}
add_action( 'wp_enqueue_scripts', 'my_theme_enqueue_styles' );

function theme_styles() {

	wp_enqueue_style( 'bootstrap_css', 'https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/css/bootstrap.min.css' );
	wp_enqueue_style( 'main_css', get_template_directory_uri() . '/style.css' );

}

add_action( 'wp_enqueue_scripts', 'theme_styles');

function theme_js() {

	global $wp_scripts;

    wp_enqueue_script( 'bootstrap_jquery', 'https://code.jquery.com/jquery-3.2.1.slim.min.js');
	wp_enqueue_script( 'bootstrap_popper', 'https://cdnjs.cloudflare.com/ajax/libs/popper.js/1.12.9/umd/popper.min.js');        
	wp_enqueue_script( 'bootstrap_js', 'https://maxcdn.bootstrapcdn.com/bootstrap/4.0.0/js/bootstrap.min.js');

}

add_action( 'wp_enqueue_scripts', 'theme_js');

?>
```


## Resources
[How to Add Bootstrap to Your WordPress Theme](https://www.zenwebthemes.com/blog/how-to-add-bootstrap-to-your-wordpress-theme/)

[Adding Bootstrap to Your WP Child Theme The Easy Way](https://www.youtube.com/watch?v=OsPbtZnpUZk&t=418s)

[How to include Bootstrap into a WordPress theme](https://www.youtube.com/watch?v=GWnDBUQwgv8)
