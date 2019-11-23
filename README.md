# videotool
### Description
it is a small tool for testing purpuses ,built with php Laravel freamwork , it can :
- stacke videos vertically
- stack videos horizontally
- separate soundtrack and video

### Installation
- This project requires a working FFMpeg install. You will need both FFMpeg and FFProbe binaries to use it. Be sure that these binaries can be located with system PATH to get the benefit of the binary detection.
 Please find the binaries at http://ffmpeg.zeranoe.com/builds/. ,
 you can test if **FFmpeg** working correctly by writing ```ffmpeg``` in your shell or cmd
 - clone the project on your device
 - after cloning the project you should do a few cmd commands in the project directory to run the project correctly :
 1. install composer files ```composer install``` 
 2. copy .env file ```cp .env.example .env```
 3. generate an app key ```php artisan key:generate```
 4. link the storage file ```php artisan storage:link```
 4. that's all , ```php artisan serve``` and start
 ### Video Class explaining
 in ```app/Http/Controllers/Classes``` there is a Video Class and it has 4 methods :
 - mregeVideoHorizontally : it takes pathes of 2 videos and stack it side by side in one video file and return the new video path .
 - mregeVideoHorizontally : it takes pathes of 2 videos and stack it vertically in one video file and return the new video path .
 - SeparateSoundLayer : it takes path of one video and return 2 files , first is only mp3 soundtrack , second is video without a sound
 - GetSize : returns size of video in kilobytes.
 - GetDuration : returns duration of video.
