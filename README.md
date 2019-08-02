# example_ofxFilikaHapPlayer
 example project shows how to use ofxFilikaHapPlayer

## Dependencies
- ofxFilika
- ofxHapPlayer

## USAGE
You should include;
1- A video foler
2- An xml settings file as follows

#### XML SETTINGS STRUCTURE
```
 <root>
     <SOURCE_FOLDER>/Users/alptugan/oF/assets/hap</SOURCE_FOLDER>
     <SOUND_FOLDER></SOUND_FOLDER>
     <COVER_FOLDER></COVER_FOLDER>
     <VID_SPEED>1</VID_SPEED>
     <VID_VOLUME>1</VID_VOLUME>
     <VID_IS_LOOPING>1</VID_IS_LOOPING>
     <VID_X>0</VID_X>
     <VID_Y>0</VID_Y>
     <VID_W>full</VID_W>
     <VID_H>full</VID_H>
     <VID_ID_TO_START>0</VID_ID_TO_START>
     <BTN_PLAY>btnplayw.png</BTN_PLAY>
     <BTN_PAUSE>btnpausew.png</BTN_PAUSE>
 </root>
```
#### INIT IN A PROJECT
In header file;

```ofxFilikaHapPlayer player;```
 
 
In .cpp file;

```player.setup("path_to_settings_file.xml", bool autoplay = false, bool loadsound = false, bool navigation = false, bool enableCoverImages = false); ```

#### Notes:
- If loadsound = true; Then, you should specify "SOUND_FOLDER" in XML file. Your sounds should have the same filename as video filenames
- If navigation = true; Then, you should specify "BTN_PLAY" and "BTN_PAUSE" in XML file. 
- If enableCoverImages = true; Then, you should specify "COVER_FOLDER" in XML file. Your sounds should have the same filename as video filenames. .png and .jpg files are allowed
