=== Plugin Name ===
Contributors: esiteq
Donate link: http://www.esiteq.com/donate/
Tags: embed, video, youtube, responsive
Requires at least: 3.0.1
Tested up to: 4.5.2
Stable tag: 4.5.2
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-3.0.html

A simple but powerful plugin to embed videos responsively into your Wordpress site. Works with both videos and playlists.

== Description ==

This plugin adds a button to post editor to insert videos and video playlists easily. Simply click the button, paste YoutubeURL
and kick Insert Video. Support for other video hostings will be added later. Video embedding can be used as a shortcode in posts
and pages, including custom post types.

A few notes about the sections above:

*   Simple button in editor to add videos to your pages and posts
*   Video is embedded responsively - will fit the container, keeping aspect ratio
*   Supports the following parameters: controls (on/off), autoplay (on/off), autohide controls (on/off), loop (on/off)

By clicking > Insert Video button it opens a popup window where you can paste video URL and set parameters. You can also set start time,
or just leave it 0:00 if you want to play video from the beginning. Playlists are also supported.

It also stores a list of recent videos where you can chose one of the videos you have used before (or saved for future). In later versions,
there will be something like a video library to access and share videos between multiple wordpress administrators and editors.

This plugin was a part of another bigger project. It was handy and easy to use, so I decided to extract the code to a stand-alone
plugin and make it available for free for public.

== Installation ==

1. Upload the plugin files to the `/wp-content/plugins/Responsive-Video-Embedder` directory, or install the plugin through the WordPress plugins screen directly.
2. Activate the plugin through the 'Plugins' screen in WordPress.
3. Open page or post for editing, you will see Insert video button next to Add Media button.

== Usage ==

When you use > Insert Video button in post / page editor, it adds a shortcode automatically. Alternatively, you can put a shortcode manually:

[rem_video id="XXXXX" list="YYYYY" autplay=0 controls=1 autohide=0 loop=0]

XXXXX is a video ID from Youtube URL, it comes after `v=`, like https://www.youtube.com/watch?v=mbBmc8RC_S8
YYYYY is a playlist ID (for playlists), like https://www.youtube.com/watch?v=mbBmc8RC_S8&list=PLCF042F294768BFD1
autoplay=(0|1): if 1, video will start automatically when your page is loaded. Default is 0 - video will not start automatically.
autohide=(0|1): if 1, it will hide controls when video is played. Default is 0 - controls will be always visible.
controls=(0|1): if 1, controls will be shown, if 0 - hidden. Default is 1.
    loop=(0|1): if 1, when video is ended, it will start from the beginning. If it is a playlist, it will loop from first video in the list.

	== Frequently Asked Questions ==

= Can I add videos directly to theme files? =

If you want to utilize the functionality in theme code, use do_shortcode('[rem_video id="XXXXX"]');

= What about foo bar? =

Answer to foo bar dilemma.

== Screenshots ==

1. A pop up window where you can set video URL and parameters, or chose one of previously used videos.

2. Button added to post / page / custom post editor.

3. Videos embedded responsively, matching container size.

== Changelog ==

= 0.1 =

Initial release.