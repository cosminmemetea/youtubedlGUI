# youtubedlGUI
This product will provide a user interface to youtube-dl using yad

##########################################################################################

1. Tested links<br> 
#https://www.youtube.com/watch?v=JN7qaeiRq8U working link <br>
#https://www.youtube.com/watch?v=JEpks-O76rE&list=PL9d4T43DjoG0qKXrjP73GZiT1xopeYpoD&index=11 <br>
#https://www.youtube.com/playlist?list=PL1C815DB73EC2678E <br>

2. To create an executable we used arronax 
	To install arronax please the following steps are required:
sudo add-apt-repository ppa:diesch/testing 
sudo apt-get update
sudo apt-get install arronax

3. Used api-s: <br>
	[x] ==Zenity== <br>
	To install zenity on your machine the following steps are required:<br>
sudo apt-get install zenity<br>
	[x] ==youtube-dl==<br>
	To install youtube-dl on your machine follow the steps from this page:<br>
https://rg3.github.io/youtube-dl/download.html<br>

4. To create a shortcut use this command ln -s ../youtubedl/YouTubeDownloader.desktop .<br>

5. Requirements 
	[x] disable other fields if an option is selected.<br>
	[x] choose audio-format : "best", "aac", "flac", "mp3", "m4a", "opus", "vorbis"-oog<br>
	for this purpose : the  youtube-dl -x --audio-format mp3 https://www.youtube.com/watch?v=gJ3uT6LVsNA is used.<br>
	[x] choose  postprocessors<br>
	   --prefer-avconv                  Prefer avconv over ffmpeg(default) for running the<br>
    	   --prefer-ffmpeg <br>

	[x] choose the quality for a audio -audio-quality QUALITY 0 best 9 worst <br>
	[x] supress no-check-certificate https checks (if necessary) <br>
	[x] if it is only video --write-thumbnail --write-all-thumbnails  to write the thumbnail on the disk  <br>
	[x] download a play list in random order in normal or in reverse order <br>
		    --playlist-reverse               Download playlist videos in reverse order<br>
    		    --playlist-random                Download playlist videos in random order<br>

	[x] include adds --include-ads <br>
	[x] download the the video or the entire playlist<br>
		    --no-playlist                    Download only the video, if the URL refers<br>
                                     to a video and a playlist.<br>
    		    --yes-playlist                   Download the playlist, if the URL refers to<br>
                                     a video and a playlist.<br>
	[x] download a video only if it has at least X views or do not download a video if it has more then Y views.<br>
	  --min-views COUNT                Do not download any videos with less than<br>
                                     COUNT views<br>
    	  --max-views COUNT                Do not download any videos with more than<br>
                                     COUNT views<br>
	[x] download only the videos after a specifc date or before a specific date or videos with a specific date<br>
  	--datebefore DATE                Download only videos uploaded on or before<br>
                                     this date (i.e. inclusive)<br>
    	--dateafter DATE                 Download only videos uploaded on or after<br>
                                     this date (i.e. inclusive)<br>
	--date DATE<br>


	[x] download max n videos<br>
		  --max-downloads NUMBER           Abort after downloading NUMBER files<br>
	[x] do not downlaod files smaller then or no larger then<br>
    --min-filesize SIZE              Do not download any videos smaller than<br>
                                     SIZE (e.g. 50k or 44.6m)<br>
    --max-filesize SIZE              Do not download any videos larger than SIZE<br>
                                     (e.g. 50k or 44.6m)<br>
	=====videos===<br>
	[x] download videos <br>
	[x] choose either or not Write metadata to the video file using --add-metadata --xattrs <br>
        [x] choose either embed thumbnail in the audio as cover art --embed-thumbnail <br>
	[x] embed subtitles for mp4 webm wkv formats video <br>

