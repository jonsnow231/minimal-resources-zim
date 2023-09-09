# minimal-resources-zim
Custom theme for Zim ( https://github.com/zim-desktop-wiki/zim-desktop-wiki ). Only 10kb including assets. Absolute black backgrounds and pale yellow text in order to use the least amount of system resources while providing low contrast as not to hurt your eyes.



# Instructions

Zim instructions for Portable on Windows: 

  1) Go to releases on right-hand of page and download source. Unzip the source. All you need is the minimal-resources folder.
  2) Add minimal-resources folder to Zim\share\themes\
  3) Go to Zim\etc\gtk-3.0\settings.ini  (create directory and .ini file if it doesn't exist) and input:
      [Settings]
      gtk-theme-name = minimal-resources
      gtk-application-prefer-dark-theme=1
	   
(There should be a gtk.css file and gtk-dark.css file for most themes (this one only uses dark), the input above first says to use minimal-resources theme, and then says to prefer dark themes if more than one .css is in the theme.)

  4) Go to Zim\config\zim\style.conf and change the following (ZIM must be restarted to see any changes in the config file):

     	 [Tag mark]
	background=#3d4468
	  
	  [Tag link]
      	foreground=lightblue
		  
(the following are **optional**, if you want different colored headings) 
	  
	  [Tag h2]
	  foreground=#b86b09
	  (don't delete anything below, just change the color of foreground)
	  
	  [Tag h3]
     	 foreground=#495ac7
	  
	  [Tag h4]
     	 foreground=#c749bd
	  
	  [Tag h5]
     	 foreground=#3bac9c
	  
	  [Tag h6]
     	 foreground=#7a3bac

   If you want to make bold and italic text stand out more, you can add a scale or color modifier in the same config file:
   
	[Tag strong]
	weight=PANGO_WEIGHT_BOLD
	scale=1.05
	foreground=#ecea80

	[Tag emphasis]
	style=PANGO_STYLE_ITALIC
	foreground=#ecea80

  5) Go to edit >preferences > Uncheck "show controls in window decoration" (I did not have this on when setting it up, so I will have to go through and find the css that affects this. I find it unnecessary though as it just decreases the amount of workspace. 


DONE. 

*********************

 
If you installed Zim rather than using portable, if this doesn't work, try putting in %appdata% instead of zim directory.



********************


Extra folder contains more CSS to alter zim more, as well as black assets for light themes. 
