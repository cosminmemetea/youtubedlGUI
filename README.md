# youtubedlGUI
This product will provide a user interface to youtube-dl using yad

##########################################################################################

1. Tested links 
#https://www.youtube.com/watch?v=JN7qaeiRq8U working link
#https://www.youtube.com/watch?v=JEpks-O76rE&list=PL9d4T43DjoG0qKXrjP73GZiT1xopeYpoD&index=11
#https://www.youtube.com/playlist?list=PL1C815DB73EC2678E

2. To create an executable we used arronax 
	To install arronax please the following steps are required:
sudo add-apt-repository ppa:diesch/testing 
sudo apt-get update
sudo apt-get install arronax

3. Used api-s: 
	[x] ==Zenity==
	To install zenity on your machine the following steps are required:
sudo apt-get install zenity
	[x] ==youtube-dl==
	To install youtube-dl on your machine follow the steps from this page:
https://rg3.github.io/youtube-dl/download.html

4. To create a shortcut use this command ln -s ../youtubedl/YouTubeDownloader.desktop .

5. Requirements 
	[x] disable other fields if an option is selected.
	[x] choose audio-format : "best", "aac", "flac", "mp3", "m4a", "opus", "vorbis"-oog
	for this purpose : the  youtube-dl -x --audio-format mp3 https://www.youtube.com/watch?v=gJ3uT6LVsNA is used.
	[x] choose  postprocessors
	   --prefer-avconv                  Prefer avconv over ffmpeg(default) for running the
    	   --prefer-ffmpeg 

	[x] choose the quality for a audio -audio-quality QUALITY 0 best 9 worst
	[x] supress no-check-certificate https checks (if necessary)
	[x] if it is only video --write-thumbnail --write-all-thumbnails  to write the thumbnail on the disk 
	[x] download a play list in random order in normal or in reverse order 
		    --playlist-reverse               Download playlist videos in reverse order
    		    --playlist-random                Download playlist videos in random order

	[x] include adds --include-ads 
	[x] download the the video or the entire playlist
		    --no-playlist                    Download only the video, if the URL refers
                                     to a video and a playlist.
    		    --yes-playlist                   Download the playlist, if the URL refers to
                                     a video and a playlist.
	[x] download a video only if it has at least X views or do not download a video if it has more then Y views.
	  --min-views COUNT                Do not download any videos with less than
                                     COUNT views
    	  --max-views COUNT                Do not download any videos with more than
                                     COUNT views
	[x] download only the videos after a specifc date or before a specific date or videos with a specific date
  	--datebefore DATE                Download only videos uploaded on or before
                                     this date (i.e. inclusive)
    	--dateafter DATE                 Download only videos uploaded on or after
                                     this date (i.e. inclusive)
	--date DATE


	[x] download max n videos
		  --max-downloads NUMBER           Abort after downloading NUMBER files
	[x] do not downlaod files smaller then or no larger then
    --min-filesize SIZE              Do not download any videos smaller than
                                     SIZE (e.g. 50k or 44.6m)
    --max-filesize SIZE              Do not download any videos larger than SIZE
                                     (e.g. 50k or 44.6m)
	=====videos===
	[x] download videos 
	[x] choose either or not Write metadata to the video file using --add-metadata --xattrs 
        [x] choose either embed thumbnail in the audio as cover art --embed-thumbnail 
	[x] embed subtitles for mp4 webm wkv formats video 

