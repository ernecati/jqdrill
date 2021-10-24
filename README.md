# jqdrill
Straight Plunge Drill GCode Generator.

https://jqdrill.necatier.com/
https://youtu.be/9hhMKms6DUc

If you use JS Cutter for your SVG to GCode projects JQdrill will help you to drills.

Uses GCodes which generated by "JScut.org". 
You can convert your SVG files to GCode with jscut. 
But jscut generates 'path followed' codes. 
If you need to drill a hole jscode drills it with a spiral path. 
After you generate your 'spiral pathed' gcodes, you can convert them straight plunge gcodes. 
For PCB drill you have two options.You can check your GCodes with NCviewer on browser or CAMotics on you desktop.

METHOD1
With using InkScape you can determine hole coordinates. 
Just create a blank page with your cnc size. 
Put circle centers to coordinates of holes that you want to drill. 
Circle diameters must bigger than yor drill diameter. 
Color and other parameters are not important. 
Select all circles Ctrl+A on the screen and convert them to path Ctrl+Shift+N After saving your SVG file browse to jscut.org and generate your GCode. 
Open your GCode with any text editor, copy all of them and paste to input text area.

METHOD2
If you designed your pcb as Gerber file or if you have a excellon file you can generate svg file with Flatcam.
Run Flatcam software and open Ctrl+E your excellon file. Select your excellion file on 'Project' tab and click 'Selected' tab. 
Configure you settings and click 'Generate Drills GCode'. Generally generated GCode not compatible for sizing. 
Bu yu can export your GCode as SVG with Flatcam. When you export your SVG, turn the Method #1.
