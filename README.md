# Wordpress-Interview-Questions-for-Freshers


Wordpress Interview Questions for Experienced:


***1.Explain the term template tags in WordPress.***

Template tags are an immensely valuable part of WordPress, especially when developing themes. A WordPress template tag is a PHP function that generates and displays content dynamically on a website. Themes in WordPress contain different templates that theme developers use to display dynamic data. The WordPress themes can use several built-in template tags. The template tags are contained in 9 files in the wp-includes directory.

wp-includes/general-template.php

wp-includes/link-template.php

wp-includes/category-template.php

wp-includes/nav-menu-template.php

wp-includes/author-template.php

wp-includes/post-template.php

wp-includes/post-thumbnail-template.php

wp-includes/comment-template.php

wp-includes/bookmark-template.php


***2. List a few template tags that can be used in WordPress.***

The following are some template tags you can use in WordPress.

get_header()
get_footer()
get_sidebar()
wp_login_url()
get_calendar()
allowed_tags()
the_author()
get_the_author()
wp_list_bookmarks()
get_bookmark()
the_category()
the_category_rss()
comment_author()
comment_author_email()
the_permalink()
user_trailingslashit()
permalink_anchor()
post_class()
post_password_required()
get_post_thumbnail_id()
the_post_thumbnail()
wp_nav_menu()
walk_nav_menu_tree(), etc



***3.State the difference between Wordpress and Wix.***

Both WordPress and Wix are platforms for building websites, but each has completely different approaches. while Wix is a website builder.


 ![Blue and White Background Simple Resume ](https://user-images.githubusercontent.com/98220932/212672931-1ba3f758-6071-476f-b95d-6e860afc62d8.jpg)


***4.What do you mean by WordPress Hooks***

Whenever you wish to alter or customize something in WordPress, you can almost certainly make use of a hook. WordPress hooks enable you to manipulate the behavior of a procedure without having to modify the WordPress core files. With hooks, you can modify or add new features to WordPress without modifying the core files


***5. What is Action and Filter Hooks?***

Action and Filter are types of WordPress Hooks.

Action Hooks: Actions enable you to perform a task at predefined points during the WordPress runtime. In the WordPress code, actions are defined as follows:

do_action( 'action_name', [optional_arguments] );

Here, the 'action_name' string represents the name of the action. If you would like to pass additional arguments to the callback function, you can specify the [optional_arguments] variable. When no value is specified, this field is empty by default.


Filter Hooks: Filters allow you to modify and return any data processed by WordPress. In the WordPress code, filters are defined as follows:

apply_filters( 'filter_name', 'value_to_be_filtered', [optional_arguments] );

Here, the ‘filter_name’ string represents the name of the filter. 'value_to_be_filtered' represents the value that has to be filtered and returned. In the same way as actions, the [optional_arguments] variable can pass additional arguments


***6.What do you mean by importers in WordPress?***

Importers are WordPress tools that can move content from an existing WordPress site to a new one. A site can also be moved from localhost to an online server with this tool. Different data can be migrated using the WordPress importer. A few examples include:

Pages, posts, and other types of custom posts

Custom fields and post meta

Comments

Tags, Categories

Authors, etc


***7.How can I adjust the default length of an excerpt in WordPress?***

 Changing the default length of the excerpt in WordPress requires us to add the following syntax to the functions.php file and edit the number of words we wish to appear in the excerpt.
 
 
     function changed_excerptlength($length){
     return X;
     }
     add_filter(‘excerpt_length’, ‘changed_excerptlength’);
     
     
Here, X is the number of excerpt words to be displayed


***8.Explain avatar and gravatar in WordPress.***


In the case of WordPress blogs or business websites, putting a face to your content will help your visitors connect and become more engaged. A good way of accomplishing this is with an avatar, a picture identifying you across your website. An avatar gives your site a more personal touch and lets users get to know you better. Using Gravatar, WordPress provides its users with avatars. Gravatar is an acronym for Globally Recognized Avatar. The Gravatar platform allows users to upload an image and use that image as their avatar on various websites. Gravatar images are displayed alongside comments, posts, and various other website activities



 ***9.Can you tell me why widgets don't display in the sidebar?***
 
To add a widget, users must first verify that the themes they are using support it. It is possible that the problem could be caused by the absence of function.php or a file similar to it. Another possibility is that the user forgot to save the changes they made to the widget or did not refresh the older page display


***10. Explain shortcode in WordPress.***

A shortcode is a small chunk of code, placed between brackets like [yourshortcode], that performs a specific function for your site. It can be placed anywhere to provide a specific feature to a page, post, or other content. WordPress shortcodes make it easy to add dynamic content to pages, posts, and sidebars. Several WordPress plugins and themes offer shortcodes for adding specialized content to websites, such as sliders, image galleries, contact forms, and more.


***11.What is the best way to display a list of child pages in WordPress?***

Shortcodes are convenient, but they require you to add them to every page that has a parent or a child page. You may end up using shortcodes on a lot of pages, and you may even forget to do it. It would be beneficial to alter the page template file in your theme so that child pages will be displayed automatically. This can be achieved by editing the main page.php template, or by creating a custom page template in your theme

***12.Is it possible to check whether a featured image exists in WordPress?***

The has_post_thumbnail() method can be used to determine whether the featured image is present.

Example:  


            if ( has_post_thumbnail() ) 
            {
                the_post_thumbnail();
            } 


 ***13.Can you explain the user metafunction in WordPress?***
 
 A user meta in WordPress is a set of distinct, different, and customized text fields for each user according to his or her preferences. In other words, WordPress user meta allows you to add whatever information you wish about your users. Update_user_meta() is the function you use to add or update a user's metadata. It looks as follows:
 
 
    update_user_meta( $user_id, $meta_key, $meta_value, $prev_value );
 
 
Here,

$user_id: User's ID to be affected.

$meta_key: Name of user meta field to be altered.

$meta_value: The value to be assigned to the user meta field. You may use integer, string, array, etc.

$prev_value: Used for handling duplicate meta keys. Normally you can omit this option.


***14. In what situations does the plugin menu not appear on the WordPress website.***

When using free wordpress.com, users can't see the plugin menu because it's limited in plugin usage. Even users who do not have an administrator account will not be able to access the plugin menu

***15. What are WordPress Themes?***


***16.What is a Child theme in WordPress?***


***17. Explain WordPress Taxonomies.?***


***18.Explain Category and Tags in WordPress. How to convert a category into a tag?***


***19. What are meta tags?***


***20.What are widgets in WordPress?***







 
