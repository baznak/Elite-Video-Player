# CCElite-Video-Player-Wordpress
Elite Video Player is stunning, modern, responsive and fully customisable video player that support the most popular video platforms like YouTube, Vimeo or self-hosting videos

### Screenshots
![img](https://github.com/sharan-aithal/Elite-Video-Player/raw/master/css/self_hosted.jpg)

## Demo
[Demos available here.](https://bit.ly/2uzIYy2)
 
# Setup
    $(document).ready(function($)

    {

        videoPlayer = $("#Elite_video_player").Video({           //ALL PLUGIN OPTIONS

	instanceName:"player1",		                      //name of the player instance

	instanceTheme:"dark",					//dark or light

	autohideControls:2,			                     //autohide HTML5 player controls

	hideControlsOnMouseOut:"Yes",		            //hide HTML5 player controls on mouse out of the player: "Yes","No"

	playerLayout: "fixedSize",		                   //Select player layout: "fitToContainer", "fixedSize", "fitToBrowser"

	videoPlayerWidth:746,			                  //fixed total player width

	videoPlayerHeight:420,			                  //fixed total player height

			lightBox:false,	                               //lightbox mode :true/false
			lightBoxAutoplay: false,                     //autoplay video when lightbox opens: true/false
			lightBoxThumbnail:"images/preview_images/poster.jpg", //lightbox thumbnail image
			lightBoxThumbnailWidth: 400,                 //lightbox thumbnail image width
			lightBoxThumbnailHeight: 220,                //lightbox thumbnail image height
			lightBoxCloseOnOutsideClick: true,           //close lightbox when clicked outside of player area

		playlist:"Off",              //choose playlist type: "Right playlist", "Off"

		playlistScrollType:"light",                  //choose scrollbar type: "light","minimal","light-2","light-3","light-thick","light-thin","inset","inset-2","inset-3","rounded","rounded-dots","3d"

		playlistBehaviourOnPageload:"opened (default)",		 //choose playlist behaviour when webpage loads: "closed", "opened (default)" (not apply to Vimeo player)

		autoplay:false,                         //autoplay when webpage loads: true/false

		colorAccent:"#a2a5a7",                  //plugin colors accent (hexadecimal value - http://www.colorpicker.com/)

		vimeoColor:"00adef",                    //set "hexadecimal value", default vimeo color is "00adef"

	youtubeControls:"custom controls",			 //choose youtube player controls: "custom controls", "default controls"

		youtubeSkin:"dark",                     //youtube theme: light,dark

            	youtubeColor:"red",                     //youtube color: red, white

		youtubeQuality:"default",                    //choose youtube quality: "small", "medium", "large", "hd720", "hd1080", "highres", "default"

	videoPlayerShadow:"effect3",            //choose player shadow:  "effect1" , "effect2", "effect3", "effect4", "effect5", "effect6", "off"

	loadRandomVideoOnStart:"No",            //choose to load random video when webpage loads: "Yes", "No"

	shuffle:"No",				            //choose to shuffle videos when playing one after another: "Yes", "No" (shuffle button enabled/disabled on start)

	posterImg:"",//player poster image 

	onFinish:"Play next video",             //"Play next video","Restart video", "Stop video",

	nowPlayingText:"Yes",                   //enable disable now playing title: "Yes","No"

	fullscreen:"Fullscreen native",         //choose fullscreen type: "Fullscreen native","Fullscreen browser"

	rightClickMenu:true,                    //enable/disable right click over player: true/false

		hideVideoSource:false,					//option to hide self hosted video sources (to prevent users from download/steal your videos): true/false

		showAllControls:true,					//enable/disable all HTML5 player controls: true/false

		allowSkipAd:true,                            //enable/disable "Skip advertisement" option: true/false

	infoShow:"Yes",                         //enable/disable info option: "Yes","No"

	shareShow:"Yes",                        //enable/disable all share options: "Yes","No"

		facebookShow:"Yes",                     //enable/disable facebook option individually: "Yes","No"

		twitterShow:"Yes",                      //enable/disable twitter option individually: "Yes","No"

		mailShow:"Yes",                         //enable/disable mail option individually: "Yes","No"

            facebookShareName:"Elite video player",      //first parametar of facebook share in facebook feed dialog is title

			facebookShareLink:"http://codecanyon.net/item/elite-video-player-wordpress-plugin/10496434",  //second parametar of facebook share in facebook feed dialog is link below title

			facebookShareDescription:"Elite Video Player is stunning, modern, responsive, fully customisable high-end video player for WordPress that support advertising and the most popular video platforms like YouTube, Vimeo or self-hosting videos (mp4).", //third parametar of facebook share in facebook feed dialog is description below link

			facebookSharePicture:"https://0.s3.envato.com/files/123866118/preview.jpg", //fourth parametar in facebook feed dialog is picture on left side

            twitterText:"Elite video player",			 //first parametar of twitter share in twitter feed dialog is text

            	twitterLink:"http://codecanyon.net/item/elite-video-player-wordpress-plugin/10496434", //second parametar of twitter share in twitter feed dialog is link

            	twitterHashtags:"wordpressvideoplayer",		 //third parametar of twitter share in twitter feed dialog is hashtag

            	twitterVia:"Creative media",				 //fourth parametar of twitter share in twitter feed dialog is via (@)

            googlePlus:"http://codecanyon.net/item/elite-video-player-wordpress-plugin/10496434", //share link over Google +

            logoShow:"Yes",                         //"Yes","No"

            logoClickable:"Yes",                    //"Yes","No"

            logoPath:"images/logo/logo.png",        //path to logo image

            logoGoToLink:"http://codecanyon.net/",  //redirect to page when logo clicked

            logoPosition:"bottom-left",            //choose logo position: "bottom-right","bottom-left"

            embedShow:"Yes",                        //enable/disable embed option: "Yes","No"

            embedCodeSrc:"www.yourwebsite.com/videoplayer/index.html", //path to your video player on server

            embedCodeW:"746",                       //embed player code width

            embedCodeH:"420",                       //embed player code height

            embedShareLink:"www.yourwebsite.com/videoplayer/index.html", //direct link to your site (or any other URL) you want to be "shared"

			youtubePlaylistID:"", //automatic youtube playlist ID (leave blank "" if you want to use manual playlist) 

			youtubeChannelID:"", //automatic youtube channel ID (leave blank "" if you want to use manual playlist) UCHqaLr9a9M7g9QN6xem9HcQ

			//manual playlist

            videos:[

                {

                    videoType:"HTML5",                                     //choose video type: "HTML5", "youtube", "vimeo"

                    title:"i Create",                                            //video title

                    youtubeID:"XMGoYNoMtOQ",                                          //https://www.youtube.com/watch?v=XMGoYNoMtOQ

                    vimeoID:"46515976",                                               //http://vimeo.com/46515976

                    mp4:"http://creativeinteractivemedia.com/player/videos/i_Create.mp4",//HTML5 video mp4 url

                    imageUrl:"images/preview_images/poster2.jpg",               

					imageTimer:4,

					prerollAD:"yes",                                                 //show pre-roll "yes","no"

                    prerollGotoLink:"http://codecanyon.net/",                          //pre-roll goto link

                    preroll_mp4:"http://creativeinteractivemedia.com/player/videos/Oceans.mp4",   //pre-roll video mp4 format

					prerollSkipTimer:5,													   //seconds when to show skip advertisement button

					midrollAD:"no",                                                                  

					midrollAD_displayTime:"00:10",                                                    

					midrollGotoLink:"http://codecanyon.net/",                                         

					midroll_mp4:"http://creativeinteractivemedia.com/player/videos/Logo_Explode.mp4", 

					midrollSkipTimer:5,	

					postrollAD:"no",                                                                

					postrollGotoLink:"http://codecanyon.net/",                                        

					postroll_mp4:"http://creativeinteractivemedia.com/player/videos/Logo_Light.mp4",  

					postrollSkipTimer:5,

					popupImg:"images/preview_images/popup.jpg",                        			  

					popupAdShow:"no",                                                                

					popupAdStartTime:"00:03",                                                         

					popupAdEndTime:"00:07",                                                          

					popupAdGoToLink:"http://codecanyon.net/",

                    description:"Video by InlifeThrill design.",                        //video description

                    thumbImg:"images/thumbnail_images/pic1.jpg",                       //path to playlist thumbnail image

                    info:"Video info goes here.<br>This text can be <i>HTML formatted</i>, <a href='http://codecanyon.net/user/_zac_' target='_blank'><font color='008BFF'>find out more</font></a>.<br>You can disable this info window in player options. <br><br>Lorem ipsum dolor sit amet ne qui nulla debitis sententiae."                                                                   //video info

                }

            ]

        });

    });



