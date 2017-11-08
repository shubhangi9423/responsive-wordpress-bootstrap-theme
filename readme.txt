
1. create folder inside Theme folder
2. create file index.php and copy the code from this link
( http://blog.teamtreehouse.com/wp-content/uploads/2012/10/bootstraop-demo-source-code.txt)
3. download the bootstrap the bootstrap folder inside this theme (http://getbootstrap.com/2.3.2/)
4. Create style.css (WordPress requires a specially formatted comment to appear at the top of the style.css page. It uses this comment to get all of the meta information about your theme.)

   ### Comment format ###
    (/*
      Theme Name: WP Bootstrap
      Theme URI: http://teamtreehouse.com/wordpress-bootstrap-theme-tutorial
      Description: A demo theme built to accompany the Treehouse blog post <a href="http://teamtreehouse.com/wordpress-bootstrap-theme-tutorial">How to Build a WordPress Theme with Bootstrap</a>.
      Author: Zac Gordon
      Author URI: http://teamtreehouse.com/
      Version: 1.0
      Tags: responsive, white, bootstrap

      License: Attribution-ShareAlike 3.0 Unported (CC BY-SA 3.0)
      License URI: http://creativecommons.org/licenses/by-sa/3.0/

      This simple theme was built using the example Bootstrap theme "Basic marketing site" found on the Bootstrap web site http://twitter.github.com/bootstrap/examples/hero.html
*/)
5. download the 300 X 225 px size image and paste into same folder  
     (The last thing we need to do before we install and start building our new theme is to upload an image that will appear with our theme in the WordPress admin area. This image needs to be 300 x 225 px and named “screenshot.png”)

6.  go into the admin area and install our new theme. Login to the admin area and go to Appearances > Theme. You should see WP Bootstrap listed as one of the themes.
Click Activate under the WP Bootstrap theme to set it as the current theme for the site.

    none of the CSS is working on this site currently,

###### Converting Bootstrap Files to WordPress Templates #########

7.  create empty files for the header.php, footer.php, and sidebar.php.


      ****** header file (copy the top of code of index.php into the header.php) 

       (<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <title>Bootstrap, from Twitter</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta name="description" content="">
    <meta name="author" content="">

    <!-- Le styles -->
    <link href="../assets/css/bootstrap.css" rel="stylesheet">
    <style type="text/css">
      body {
        padding-top: 60px;
        padding-bottom: 40px;
      }
    </style>
    <link href="../assets/css/bootstrap-responsive.css" rel="stylesheet">

    <!-- Le HTML5 shim, for IE6-8 support of HTML5 elements -->
    <!--[if lt IE 9]>
      <script src="http://html5shim.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->

    <!-- Le fav and touch icons -->
    <link rel="shortcut icon" href="../assets/ico/favicon.ico">
    <link rel="apple-touch-icon-precomposed" sizes="144x144" href="../assets/ico/apple-touch-icon-144-precomposed.png">
    <link rel="apple-touch-icon-precomposed" sizes="114x114" href="../assets/ico/apple-touch-icon-114-precomposed.png">
    <link rel="apple-touch-icon-precomposed" sizes="72x72" href="../assets/ico/apple-touch-icon-72-precomposed.png">
    <link rel="apple-touch-icon-precomposed" href="../assets/ico/apple-touch-icon-57-precomposed.png">
  </head>

  <body>

    <div class="navbar navbar-inverse navbar-fixed-top">
      <div class="navbar-inner">
        <div class="container">
          <a class="btn btn-navbar" data-toggle="collapse" data-target=".nav-collapse">
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
            <span class="icon-bar"></span>
          </a>
          <a class="brand" href="#">Project name</a>
          <div class="nav-collapse collapse">
            <ul class="nav">
              <li class="active"><a href="#">Home</a></li>
              <li><a href="#about">About</a></li>
              <li><a href="#contact">Contact</a></li>
              <li class="dropdown">
                <a href="#" class="dropdown-toggle" data-toggle="dropdown">Dropdown <b class="caret"></b></a>
                <ul class="dropdown-menu">
                  <li><a href="#">Action</a></li>
                  <li><a href="#">Another action</a></li>
                  <li><a href="#">Something else here</a></li>
                  <li class="divider"></li>
                  <li class="nav-header">Nav header</li>
                  <li><a href="#">Separated link</a></li>
                  <li><a href="#">One more separated link</a></li>
                </ul>
              </li>
            </ul>
            <form class="navbar-form pull-right">
              <input class="span2" type="text" placeholder="Email">
              <input class="span2" type="password" placeholder="Password">
              <button type="submit" class="btn">Sign in</button>
            </form>
          </div><!--/.nav-collapse -->
        </div>
      </div>
    </div>

    <div class="container">
)    


      ****** index.php (now the index.php file is)
      (

      <!-- Main hero unit for a primary marketing message or call to action -->
      <div class="hero-unit">
        <h1>Hello, world!</h1>
        <p>This is a template for a simple marketing or informational website. It includes a large callout called the hero unit and three supporting pieces of content. Use it as a starting point to create something more unique.</p>
        <p><a class="btn btn-primary btn-large">Learn more &raquo;</a></p>
      </div>

      <!-- Example row of columns -->
      <div class="row">
        <div class="span4">
          <h2>Heading</h2>
          <p>Donec id elit non mi porta gravida at eget metus. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod. Donec sed odio dui. </p>
          <p><a class="btn" href="#">View details &raquo;</a></p>
        </div>
        <div class="span4">
          <h2>Heading</h2>
          <p>Donec id elit non mi porta gravida at eget metus. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus. Etiam porta sem malesuada magna mollis euismod. Donec sed odio dui. </p>
          <p><a class="btn" href="#">View details &raquo;</a></p>
       </div>
        <div class="span4">
          <h2>Heading</h2>
          <p>Donec sed odio dui. Cras justo odio, dapibus ac facilisis in, egestas eget quam. Vestibulum id ligula porta felis euismod semper. Fusce dapibus, tellus ac cursus commodo, tortor mauris condimentum nibh, ut fermentum massa justo sit amet risus.</p>
          <p><a class="btn" href="#">View details &raquo;</a></p>
        </div>
      </div>

    )

    ***** fooder.php
    (      <hr>

      <footer>
        <p>&copy; Company 2012</p>
      </footer>

    </div> <!-- /container -->

    <!-- Le javascript
    ================================================== -->
    <!-- Placed at the end of the document so the pages load faster -->
    <script src="../assets/js/jquery.js"></script>
    <script src="../assets/js/bootstrap-transition.js"></script>
    <script src="../assets/js/bootstrap-alert.js"></script>
    <script src="../assets/js/bootstrap-modal.js"></script>
    <script src="../assets/js/bootstrap-dropdown.js"></script>
    <script src="../assets/js/bootstrap-scrollspy.js"></script>
    <script src="../assets/js/bootstrap-tab.js"></script>
    <script src="../assets/js/bootstrap-tooltip.js"></script>
    <script src="../assets/js/bootstrap-popover.js"></script>
    <script src="../assets/js/bootstrap-button.js"></script>
    <script src="../assets/js/bootstrap-collapse.js"></script>
    <script src="../assets/js/bootstrap-carousel.js"></script>
    <script src="../assets/js/bootstrap-typeahead.js"></script>
      </body>
    </html>
   )


8.  The two tags we will user are get_header() and get_footer(). These are built in WordPress functions that find the header.php and footer.php files and include them at the top and bottom of the page.   


     copy get_header() and get_footer() into the index.php get.header() should on top and get_footer() should be on bottom.

9.  Find the links to the CSS files in the header.php file and change them from this
   (<!-- Le styles -->
      <link href="../assets/css/bootstrap.css" rel="stylesheet">
      <style type="text/css">
        body {
          padding-top: 60px;
          padding-bottom: 40px;
        }
      </style>
      <link href="../assets/css/bootstrap-responsive.css" rel="stylesheet">
  )

  and to this
          ( <!-- Le styles -->
            <link href="<?php bloginfo('stylesheet_url');?>" rel="stylesheet">
          )


     The in your style.css file, add the following:

           (
             @import url('bootstrap/css/bootstrap.css'); 
              @import url('bootstrap/css/bootstrap-responsive.css'); 
              body { 
                   padding-top: 60px; 
                   padding-bottom: 40px; 
              }
            ) 

10. The wp_head() function is an important hook that allows for plugin developers to dynamically add CSS or JavaScript to your site and  our JavaScript in the way WordPress recommends loading JavaScript. This method includes using the wp_enqueue_script() function.

   wp_head() function is what plugins and themes use to add CSS and JavaScript to the header.php file.
 
      now header.php is look like :

          (<head>
    <meta charset="utf-8">
    <title>Bootstrap, from Twitter</title>
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <!-- Le styles -->
    <link href="<?php bloginfo('stylesheet_url');?>" rel="stylesheet">

    <!-- Le HTML5 shim, for IE6-8 support of HTML5 elements -->
    <!--[if lt IE 9]>
      <script src="http://html5shim.googlecode.com/svn/trunk/html5.js"></script>
    <![endif]-->

    <?php wp_enqueue_script("jquery"); ?>
    <?php wp_head(); ?>
  </head>
  <body>

  <div class="navbar navbar-inverse navbar-fixed-top">
    <div class="navbar-inner">
      <div class="container">
        <a class="btn btn-navbar" data-toggle="collapse" data-target=".nav-collapse">
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
          <span class="icon-bar"></span>
        </a>
        <a class="brand" href="<?php echo site_url(); ?>"><?php bloginfo('name'); ?></a>
        <div class="nav-collapse collapse">
          <ul class="nav">

              <?php wp_list_pages(array('title_li' => '', 'exclude' => 4)); ?>

          </ul>
        </div><!--/.nav-collapse -->
      </div>
    </div>
  </div>

  <div class="container">
 )

 and updated footer.php is

 ( <hr>

      <footer>
        <p>© Company 2012</p>
      </footer>

    </div> <!-- /container -->

    <?php wp_footer(); ?>

  </body>
</html>
 )


 11.  wp_head() function is what plugins and themes use to add CSS and JavaScript to the header.php file.

To do this we will have to create a new file called functions.php and load our JavaScript from there. This may seem like a lot of extra steps to load a JavaScript file, but as your themes get more complex it will help everything stay clean and organized.


  functions.php
  (<?php 

function wpbootstrap_scripts_with_jquery()
{
  // Register the script like this for a theme:
  wp_register_script( 'custom-script', get_template_directory_uri() . '/bootstrap/js/bootstrap.js', array( 'jquery' ) );
  // For either a plugin or a theme, you can then enqueue the script:
  wp_enqueue_script( 'custom-script' );
}
add_action( 'wp_enqueue_scripts', 'wpbootstrap_scripts_with_jquery' );

?>)



12.  Creating the WordPress Homepage

    To do this, go to the WordPress admin area and click Pages > Add New. Title the page “Home” and then click on the HTML tab above the Content Editor.  Now we will cut the remaining markup from the index.php file and paste it into this page and click “Publish”. 

     The WordPress Loop through a page or post and pulls in its title and content, as well as a lot of other information like the date it was published, the author who published it, and even any comments associated with the post or page.


     and index.php will look like this

     (    <?php get_header(); ?>

          <?php if ( have_posts() ) : while ( have_posts() ) : the_post(); ?>

          <?php endwhile; else: ?>
            <p><?php _e('Sorry, no posts matched your criteria.'); ?></p>
          <?php endif; ?>

          <?php get_footer(); ?>

      ) 

      The code for the title looks like this the_title() and the code for the content looks like this the_content(). 


        so now updated index.php 

        (
            <?php if ( have_posts() ) : while ( have_posts() ) : the_post(); ?>

            <h1><?php the_title(); ?></h1>  
            <?php the_content(); ?>

            <?php endwhile; else: ?>
            <p><?php _e('Sorry, no posts matched your criteria.'); ?></p>
            <?php endif; ?>
        )


        {Before we can test this in the browser, we have to update a setting in WordPress to make it display our Home page as the front page instead of recent blog posts. To do this navigate in the admin area to Settings > Reading and under “Front page displays” and click on the “A static page” radio button. Next select “Home” from the “Front page:” dropdown.}


 13. WordPress allows us to use a special file called the front-page.php file just for the   home page of the site. 
       go ahead and save the index.php file as front-page.php and remove the get_title() from the template since we don’t want “Home” appearing in an h1 at the top of the page.

       front-page.php
       (<?php if ( have_posts() ) : while ( have_posts() ) : the_post(); ?>

        <?php the_content(); ?>

        <?php endwhile; else: ?>
        <p><?php _e('Sorry, no posts matched your criteria.'); ?></p>
        <?php endif; ?>)


14. Now we are going to use the WordPress code wp_list_pages() for listing the pages. the options for this tag, but what it is doing is creating a list item and a link for each of the pages. Add the following code inside of the empty unordered list with the “nav” class.

           (<ul class="nav">

            <?php wp_list_pages(array('title_li' => '')); ?>

            </ul>)      


15.  Creating the Page, Post and Post Listing Templates

    Pages Template

       page.php


       (    <?php get_header(); ?>

            <div class="row">
            <div class="span8">

            <?php if ( have_posts() ) : while ( have_posts() ) : the_post(); ?>
              <h1><?php the_title(); ?></h1>
                <?php the_content(); ?>

            <?php endwhile; else: ?>
              <p><?php _e('Sorry, this page does not exist.'); ?></p>
            <?php endif; ?>

            </div>
            <div class="span4">
               <?php get_sidebar(); ?>  
            </div>
          </div>

          <?php get_footer(); ?>)     

          add  the get_sidebar() code inside the “span4” div like this.   

16.  Posts Listing Page

      the home.php template is reserved for the page that lists out posts.
      the_permalink(), that we can use with an anchor tag to link from the main news page to individual news articles. This is what the markup with around the_title() should look like now.

      <h2><a href="<?php the_permalink(); ?>"><?php the_title(); ?></a></h2>

      In the place of the content we’re going to add in the date of the post using a tag called the_time().

      To do this we are going to use the_time() function customized like this:

        (the_time('l, F jS, Y'))  


      The final home.php template should look like this.   

      (<?php get_header(); ?>

        <div class="row">
          <div class="span8">
            <h1>News</h1>

            <?php if ( have_posts() ) : while ( have_posts() ) : the_post(); ?>
            <h2><a href="<?php the_permalink(); ?>"><?php the_title(); ?></a></h2>
            <p><em><?php the_time('l, F jS, Y'); ?></em></p>
            <hr>

            <?php endwhile; else: ?>
              <p><?php _e('Sorry, there are no posts.'); ?></p>
            <?php endif; ?>

          </div>
          <div class="span4">

            <?php get_sidebar(); ?>   

          </div>
        </div>

        <?php get_footer(); ?>)       

17.  Single Post Template

      This leaves us one template left to do and that is the template to display individual posts. This template is going to look very similar to our page.php template so we’ll start by opening the page.php file and saving it as single.php. In WordPress, the single.php template is used to display individual posts. 

       The biggest change we are going to make to this template is adding the ability to post comments. While there is a lot of complex code that is required behind the scenes to make comments work, it is actually pretty easy to add comments to the template thanks to the comments_template() tag.           


      single.php 
      (<?php get_header(); ?>

        <div class="row">
          <div class="span8">

          <?php if ( have_posts() ) : while ( have_posts() ) : the_post(); ?>
            <h1><?php the_title(); ?></h1>
            <p><em><?php the_time('l, F jS, Y'); ?></em></p>

              <?php the_content(); ?>

              <hr>
            <?php comments_template(); ?>

          <?php endwhile; else: ?>
            <p><?php _e('Sorry, this page does not exist.'); ?></p>
          <?php endif; ?>

          </div>
          <div class="span4">
          <?php get_sidebar(); ?>   
          </div>
        </div>

        <?php get_footer(); ?>)

18.  Widgetizing the Sidebar
      this will do is allow us to use WordPress widgets in our sidebar.
     Open the functions.php file and add the following code to the file.
     (<?php 

      function wpbootstrap_scripts_with_jquery()
      {
        // Register the script like this for a theme:
        wp_register_script( 'custom-script', get_template_directory_uri() . '/bootstrap/js/bootstrap.js', array( 'jquery' ) );
        // For either a plugin or a theme, you can then enqueue the script:
        wp_enqueue_script( 'custom-script' );
      }
      add_action( 'wp_enqueue_scripts', 'wpbootstrap_scripts_with_jquery' );

      if ( function_exists('register_sidebar') )
        register_sidebar(array(
          'before_widget' => '',
          'after_widget' => '',
          'before_title' => '<h3>',
          'after_title' => '</h3>',
        ));
?>)


19. Update the sidebar.php so it looks like this:
    (<?php if ( !function_exists('dynamic_sidebar') || !dynamic_sidebar() ) : ?>
<?php endif; ?>)


20. thewme is created.


   if you want follow this document(http://blog.teamtreehouse.com/responsive-wordpress-bootstrap-theme-tutorial)









