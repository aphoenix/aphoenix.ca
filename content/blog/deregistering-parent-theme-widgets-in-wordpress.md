+++
title = "Deregistering Parent Theme Widgets in Wordpress"
date = 2011-03-21
+++

I had a "fun" time figuring out how to deregister parent theme widgets in Wordpress the other day so I went through the codex and learned a lot about how functions are called in function.php. I learned about something I didn't know - you can specify the order of priority that something has within a hook!

This made deregistering widget areas pretty easy. In twentyten (something I child theme from a fair bit), the widgets are added on line 373 with code that looks like this:

function twentyten\_widgets\_init() {   
  // Area 1, located at the top of the sidebar.                                                                    
    register\_sidebar( array(                                                                                         
    'name' => \_\_( 'Primary Widget Area', 'twentyten' ),                                                          
    'id' => 'primary-widget-area',
   // and so on
 

So, you write an unregister function in your child theme's functions.php that looks something like this:

function my\_unregister\_sidebars() {                                                                                  
    unregister\_sidebar('primary-widget-area');                                                                       
    unregister\_sidebar('secondary-widget-area');                                                                     
    unregister\_sidebar('first-footer-widget-area');                                                                  
    unregister\_sidebar('second-footer-widget-area');                                                                 
    unregister\_sidebar('third-footer-widget-area');                                                                  
    unregister\_sidebar('fourth-footer-widget-area');                                                                 
} 

Then you just call that in the widgets init hook, but give it a later priority:

  add\_action( 'widgets\_init', 'my\_unregister\_sidebars', 11);                                                           
  add\_action( 'widgets\_init', 'my\_widgets\_init',12);

Google wasn't super helpful for me until after I had figured out the solution to the problem. So, if you need to unregister widgets in a child theme, this is how to do it.

(Feel free to tell me if I have typoed anywhere.)
