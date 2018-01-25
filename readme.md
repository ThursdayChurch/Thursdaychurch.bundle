This is a Plex channel for Thursday Church located in Vincennes, IN for displaying sermon video feeds.

It requires a specific structure of the shows URL. Please see the notes below.

NOTES AND INSTRUCTIONS FOR USING THIS CHANNEL

With this channel you can add shows from any of the show types listed.  I have also added a "Channel Tools" section with some additional tools that can be useful including clearing all shows, using the json files available in the Resources folder of this bundle to facilitate adding multiple shows, and special instructions for Roku and Plex Web users. 

Live feeds must be HLS(m3u8) to work with this channel. Since live feeds do not access a website with metadata, once a live feed is added, you should go to the Edit Show option and add a title for each live feed.

RSS feeds works for any video or audio RSS feed if either the videos for that website works with the PlexIt bookmarklet or direct links to the video files (like .mp4) are listed in each entry of the feed. So you cannot enter the URL for an text based RSS Feed. And, for example, a video RSS Feed for your local news station will not work if the videos for that site do not work with the PlexIt bookmarklet or the feed include direct links to the video streams. Media streams listed in the XML code as enclosure or media:content URL are recognized by the channel code. The channel can support RSS feed that show a media file of type mp3, m4a, mp4, and flv. Examples of RSS feeds that have media files and provides direct access to the video files are http://thebrowncast.libsyn.com/rss and http://feeds.feedbur...arge?format=xml.  The channel has a built in function that will check the media in the RSS feed. If there is no URL service (meaning it will not work with PlexIt) or the media stream links are not listed in the RSS feed, the entry will be listed as "No URL Service or Media Files for Entry,".

To add a new show to sections of the Webisode channel, other than the RSS feed, you just need to enter the name or id of the show. For example to add the show High Maintenance to the Vimeo section, you would just type in "High Maintenance". For the YouTube section,you would enter the playlist id, channel id, or user name. You must include the PL at the beginning of playlist and UC at the beginning of channel ids for them to be recognized. For a playlist from Youtube with a url of https://www.youtube.com/playlist?list=PL4F5986B34F73F112, you would only need to enter "PL4F5986B34F73F112" or for a user account like http://www.youtube.com/user/NewarkTimesWeddings, you would just enter the user name NewarkTimesWeddings.

If you are having issues with a show not being recognized or returning as invalid using the method above, you can instead enter the full url address for the show. The format for the URL to be entered is given below and usually follows the URL address given in your browsers address bar:

YOUTUBE
Examples:
Playlist url: https://www.youtube.com/playlist?list=PLl4T6p7km9dbx0o8J35KjWAwaiEo5tV7G
User upload url: https://www.youtube.com/user/NewarkTimesWeddings

VIMEO
Example: http://vimeo.com/highmaintenance

RSS FEEDS
Example: http://www.cwtv.com/feed/video/xml


IMPORTANT INSTRUCTIONS FOR ROKU USERS:

A LINK TO THE REMOKU WEB BASED REMOTE CONTROL AT http://remoku.tv/ MAKES INPUT OF URLS VERY EASY. LINK IT TO THE ADDRESS OF YOUR ROKU MACHINE. MORE INFO IS AVAILABLE AT http://forums.roku.c...p?f=28&t=46852. ONCE YOU HAVE REMOKU RUNNING IN YOUR BROWSER, YOU CAN THEN CAN COPY AND PASTE THE URL ADDRESS INTO THE REMOKU DIRECTLY INTO THE ADD CHANNEL USER ENTRY.

IMPORTANT INSTRUCTIONS FOR Plex/Web USERS:

THE PLEX/WEB INTERFACE WILL ONLY UPDATE ONCE A DAY UNLESS YOU CLEAR YOUR CACHE. SO ANY SHOWS ADDED OR CHANGES MADE TO THIS CHANNEL WILL BE SEEN IMMEDIATELY IN OTHER CLIENTS BUT CAN TAKE 24 HOURS TO SHOW UP IN THE PLEX/WEB INTERFACE UNLESS THE CACHE IS CLEARED.

PLEX/WEB (AKA MEDIA MANAGER) DOES NOT PRODUCE THE LISTINGS FOR USER INPUT OPTIONS, SO IT WILL NOT SHOW THE ADD SHOW BUTTON OFFERED IN EACH SHOW SECTION OR LIST ALL THE EDIT OPTIONS OFFERED FOR EACH SHOW. 

YOU CAN STILL USE THE INDIVIDUAL INPUT OPTIONS TO ADD NEW SHOWS AND ADD OR UPDATE CUSTOM TITLES, BUT YOU WILL HAVE TO DO SO BLINDLY USING THE SEARCH INPUT DIALOG BOX AT THE TOP OF THE SCREEN WHILE IN THE SECTIONS OF THE CHANNEL THAT OFFER THAT USER INPUT. 

TO ADD A NEW SHOW, ENTER THAT SHOW SECTION, SUCH AS YOUTUBE SHOWS OR VIMEO SHOWS AND ENTER THE NEW SHOW URL YOU WOULD LIKE TO ADD IN THE SEARCH INPUT DIALOG BOX AT THE TOP OF THAT SCREEN PAGE AND HIT ENTER. TO ADD OR UPDATE A TITLE FOR A SHOW, GO TO THE EDIT SHOWS OPTION SECTION FOR A SHOW AND ENTER THE NEW SHOW URL YOU WOULD LIKE TO ADD IN THE SEARCH INPUT DIALOG BOX AT THE TOP OF THAT SCREEN PAGE AND HIT ENTER. IN EACH CASE, AFTER YOU HAVE ENTERED THE INPUT, A DIALOG BOX WILL APPEAR INFORMING YOU THAT THE NEW SHOW WAS ADDED OR THE TITLE WAS UPDATED.

AND YOU WILL NOT BE ABLE TO UPDATE OR ADD CUSTOM IMAGES THROUGH THE PLEX WEB INTERFACE BECAUSE PLEX WEB ONLY RECOGNIZES ONE USER INPUT OPTION IN EACH SECTION.

IMPORTANT NOTE FOR ADVANCED USERS:
WARNING: PLEASE MAKE BACKUPS BEFORE EDITING THE JSON FILES. CHOOSING TO EDIT THE JSON FILE PROVIDED CAN CAUSE THOS JSON FILES TO NO LONGER BE RECOGNIZED BY THE WEBISODE CHANNEL.

For those who are familiar with the format of JSON files, a JSON files called data.json is included in the Resources folder of the channel to allow users to add multiple shows as well as customize the images and titles for each show. You only have to add a URL to the "url" field and provide a value of rss, youtube, vimeo, dailymotion or live for the "type" field for each JSON entry for the show to work in the channel. The channel is designed to pull the image and title metadata offered on the webpage for each URL. But since live feeds are not accessing a web page that contains metadata, you will need to add a "name" field or the entry will show up as a blank listing.

If you choose the JSON data file to update the shows for this channel there are a few things to keep in mind. YOU MUST ENTER A FULL AND ACCURATE URL IF USING THE JSON URL. All shows and their data are saved to a local dictionary file, not the JSON data file provided. The JSON data file uses the same format as the local dictionary to ensure entries are added correctly. So you can add the necessary data for the show to the JSON file but would then need to either choose the Replace Show list with JSON or Add Shows from the JSON to my Currrent List options in the Channel Tools section for any changes or additions you make to the JSON data file to show up in the Webisode channel. 

If the show data in the channel becomes corrupt, it is best to delete all shows by using the "Clear All Shows" option in the Channel Tools section. But if issues arise with the channel and you must access or delete the dictionary file used by the channel, it is located in the /Plex Media Server/Plug-in Support/Data/com.plexapp.plugins.webisodes/ folder. 
