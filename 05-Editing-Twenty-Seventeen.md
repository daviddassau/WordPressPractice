# Editing the Twenty Seventeen Wordpress Theme

If you'd like to get rid of those pesky page titles on the side, you can do the following:

Add this to the `style.css` in your child theme folder...
```CSS
body.page-template-template-full-width #content #primary {
	max-width: 100%;
}

body.page-template-template-full-width #content #primary .entry-header,
body.page-template-template-full-width #content #primary .entry-content {
    float: none;
    width: 100%;
}

body.page-template-template-full-width #content #primary .entry-header {
    margin-bottom: 4em;
}
```

Then, make a new file in your child theme folder called `template-full-width.php` and put this in there...
```PHP
<?php
/**
 * Template Name: Full Width
 *
 * Description: A custom template for displaying a fullwidth layout with no sidebar.
 *
 * @package Twenty Seventeen Child
 */

get_header(); ?>

<div class="wrap">
	<div id="primary" class="content-area">
		<main id="main" class="site-main" role="main">

			<?php
			while ( have_posts() ) : the_post();

				get_template_part( 'template-parts/page/content', 'page' );

				// If comments are open or we have at least one comment, load up the comment template.
				if ( comments_open() || get_comments_number() ) :
					comments_template();
				endif;

			endwhile; // End of the loop.
			?>

		</main><!-- #main -->
	</div><!-- #primary -->
</div><!-- .wrap -->

<?php get_footer();
```
