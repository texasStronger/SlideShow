# SlideShow.py
Python Screen Show to display photos with options.
Usage: python config.txt
    
    Info:
    SlideShow displays a slide show of photos (jpg, gif, png, jpeg).
    Start the program with a config.txt. All specified sub-folders will be searched. 
    The /path/ should have a config.txt file to change program operations. Otherwise hard coded
    defaults are used. Format of config.txt:
    
    [slideshow]
    #delay seconds from 1 to ...
    delay=30
    # reload this config file when it is changed: true or false
    reload=true
    # scale smaller photos up to screen: true or false
    scaleup=True
    # scale larger photos down to screen size: true or false
    scaledown=True: true or false
    # begin slide show at: format HH:MM
    time_begin=06:30
    # end slide show at: format HH:MM
    time_end=21:59
    # show filenames on the screen: true or false
    showfilenames=true
    # sort photos by full path name : none, ascending, descending or random
    sort=random
    # transition photos with a blend: true or false
    blend=true
    # blend speed: 0.0 to 1.0
    blend_speed=0.10
    # included photos from these folders and their subfolders
    includedfolders=  ./mmedia/pics
    # excluded photos from these folders and their subfolders
    excludedfolders= ./mmedia/pics/1996  ./mmedia/pics/1998
    
    Keys / mouse:
    Left click or 's' key: show the settings popup for changes to currently running SlideShow
    Right click or 'space bar' key: advance to next photo
    'p' key: pause the current photo
    'h' key: hide the screen
    'esc', 'q' keys: ends the program
    
    If config.txt or SlideShow.py are changed in the file system, the program will reload 
    and restart, respectively.
    
    Files needed: SlideShow.py PopupSettings.py config.txt
    Tested on windows 10 and raspberry pi buster, Python 3.9 with tkinter and Pillow
    
    Author P Bahrs
    
