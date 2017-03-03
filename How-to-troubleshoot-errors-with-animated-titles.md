**This has been updated in the daily builds. Got to http://www.openshot.org/download/ and click on the _Other Windows Downloads_ link to get the latest**

There are a [large number of issues](https://github.com/OpenShot/openshot-qt/search?q=animated+title&type=Issues&utf8=%E2%9C%93) logged about errors when trying to create animated titles with Blender.  When trying to create an animated title OpenShot returns an error: No frame was found in the output from Blender.

### First, set the path to Blender correctly

On **Windows** Blender is installed by default into:
* 64-bit - C:\Program Files\Blender Foundation\Blender\blender.exe
* 32-bit - C:\Program Files (x86)\Blender Foundation\Blender\blender.exe

On **Linux** ```which blender``` will tell you the install path which is usually ```/usr/lib/blender/``` on Debian\Ubuntu systems.

On **Mac OS X** blender.app can be installed in the Applications folder and used like any other app.  Right click on the app and select Show Package Contents. Then navigate to the executable and drag and drop this to the terminal.  This will give you the path to the executable - something like ```/Applications/blender/blender.app/Contents/MacOS/blender```

### Second, update the Blender scripts

The Blender scripts bundled with OpenShot need to be updated to take into account a change to the Blender Python API where  the Python attribute in TextCurve has changed from ```text_object.align``` to ```text_object.align_x```.

The following scripts need to be updated:
* blinds, 
* blur, 
* colours, 
* defocus, 
* dissolve, 
* explode, 
* fly_by_1, 
* fly_by_two_titles, 
* glare, 
* glass_slider, 
* halo_zoom_out, 
* neon_curves, 
* rotate_360, 
* trees, 
* wireframe_text,
* zoom_clapboard.

The text to change is in the Modify Text / Curve settings section (search for ```text_object.align``` or ```spacemode```) and change the ```align``` to ```align_x```.

Restart OpenShot (sometimes a complete reboot is needed) and try creating an animated title.  Be patient.  Blender can take a long time to render some of the image sequences or AVI clips.

On Windows you can check in C:\Users\username\.openshot-qt\blender for output from the animation process.

### Further debugging

Hopefully, OpenShot and Blender are now working well together and you have some animated titles in your project.  If not enable debug mode and check the log file.  To enable debug mode go to Edit > Preferences > Debug and tick the box.  Logs are written to (on Windows) C:\Users\username\.openshot-qt\openshot-qt.log

You can also run the Blender files and scripts outside of OpenShot to see if there are any errors reported.  Open a command prompt or terminal and enter (adjusting paths as appropriate to your system):

```/path/to/blender -b /path/to/blend/file.blend -P /path/to/python/script.py```

This tells Blender to open the specified blend file and run the specified python script.  Progress and errors will be output in the terminal.  This together with the debug log will hopefully give you additional information to help you solve the problem.