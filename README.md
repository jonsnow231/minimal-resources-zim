# minimal-resources-zim
Custom theme for Zim. Only 10kb including assets. Absolute black backgrounds and pale yellow text in order to use the least amount of system resources while providing low contrast as not to hurt your eyes.



# Instructions

Zim instructions for Portable on Windows: 

  1) Go to releases on right-hand of page and download source. Unzip the source. All you need is the minimal-resources folder.
  2) Add minimal-resources folder with .css and assets to Zim\share\themes\
  3) Go to Zim\etc\gtk-3.0\settings.ini  (create directory and .ini file if it doesn't exist) and input:
      [Settings]
      gtk-theme-name = minimal-resources
      gtk-application-prefer-dark-theme=1
	   
(There should be a gtk.css file and gtk-dark.css file for most themes, the input above makes sure it uses the gtk-dark file)

  4) Go to Zim\config\zim\style.conf and change the following:
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
	  
	  
DONE. 

*********************

 
If you installed on system, if this doesn't work, try putting in %appdata% instead of zim directory.



********************


Extra folder contains more CSS to alter zim more, as well as black assets for light themes. 
