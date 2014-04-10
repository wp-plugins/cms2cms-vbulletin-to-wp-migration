=== CMS2CMS: Automated vBulletin to WordPress Migration  ===
Contributors: cms2cms
Tags: vbulletin to wordpress, vbulletin to wordpress mirgation, convert vbulletin to wordpress, migrate vbulletin to wordpress
Requires at least: 3.0.0
Tested up to: 3.8
Stable tag: 3.6.2
License: GPLv2
License URI: http://www.gnu.org/licenses/gpl-2.0.html

Move your website content from vBulletin to WordPress quickly and easily without programming skills.

== Description ==

CMS2CMS is an automated service which will help you to migrate your data from vBulletin to WordPress. 

= You will be able to convert the following items: =
* Forums/Categories
* Posts/Replies
* Topic/Threads
* Users
* Tags
* Polls

*Supported WordPress versions:* 3.x (new software versions are constantly being added).

= Why CMS2CMS? =

* There is no need to have coding knowledge. The only thing you should do is to follow simple migration wizard. 
* You don’t have to install additional software in order to perform the migration due to the fact that CMS2CMS service is web based. 
* You will be provided with the technical support before, during and after conversion. 
* There is a possibility to try a free Demo Migration in order to see how the service works and make sure that it is what you need. 


= Additional Migration Options =
- Fix broken relationships in the database.
- clear WordPress data before migration


**Note.** *This plugin installs connection bridge on WordPress website, which is necessary for data exchange between vBulletin and WordPress websites. After activation, you’ll be redirected to CMS2CMS website in order to complete the migration.*

**Website design (styles, themes) isn’t migrated.**

= Steps to Take before Migration =
1. Install WordPress and make sure that vBulletin and WordPress websites are available online.
1. Have vBulletin website FTP access details at hand (host, username, password) - you use them to install connection bridge on vBulletin website.
1. Set up custom URL structure for WordPress (it should be set before the migration for internal links to work correctly, if you change them after migration, site navigation will be broken).

For more information follow this link: http://www.cms2cms.com/supported-cms/vbulletin-to-wordpress-migration/. 



== Installation ==

1. Download the plugin zip file
1. Extract plugin zip file to your PC
1. Upload extracted file to wp-content/plugin directory
1. Go to Admin -> Plugins, find “CMS2CMS vBulletin to WordPress Migration” and click Activate
1. You’ll be redirected to CMS2CMS website in order to complete your migration

== Frequently Asked Questions ==

= Your website is unreachable =
If your website cannot be reached, pay attention to the following points:
1. Make sure your site is available online at the moment.
2. It’s possible that your firewall blocks certain IP requests. Contact your system administrator or hosting provider support for details about this issue.

= Your server responds with 401 Unauthorized =
If you get this error, try the following solutions:
1. Ensure that access to your site content is not blocked by HTTP Basic Authentication (http://en.wikipedia.org/wiki/Basic_access_authentication). HTTP Basic Authentication is a protection method which requests additional login and password to access webpage or other resource.
2. Make sure that your website content is available on the Internet during the Migration process.

= Your server responds with 403 Forbidden =
This error means that access to certain files or folders is limited. Find below the possible solutions:
1. Your firewall may be causing this by blocking access to the server for our IP addresses. Please, contact your hosting provider and ask them to add the following IPs to the white-list:
92.52.129.82
204.62.12.42
Port 80.
This is done to enable data exchange between your websites. After the migration is complete, you’ll be able to remove our IPs from the white list.
2. Check the access permissions. For ‘cms2cms’ folder specify the file permissions 755. For files in the ‘cms2cms’ folder specify permissions 644.
3. Find out whether there are access restrictions for bridge file. Usually, restrictions are specified in .htaccess file. Contact your system administrator for details.

= Your server responds with 413 Request Entity Too Large =
It indicates that the request is too large for your server. These are possible solutions:
Increase values for the following parameters: ‘memory_limit’ and ‘post_max_size’ in PHP configuration.
If the module suhosin for PHP is installed on the server, increase the parameter ‘suhosin.post.max_value_length’. Usually, the value of 32 Mb is enough.

= Your server responds with 500 Server Error =
Incorrect permissions for bridge folder are the most common reason of this internal server error.
1. for \'cms2cms\' folder, specify the file permissions 755
2. for \'index.php\', \'bridge.php\' and \'key.php\' files in \'cms2cms\' folder, specify the permissions 644
3. If it won’t help, contact your system administrator who can provide you with server logs access for further error detection. You can also request technical assistance from your hosting provider.

= Failed to connect to host / Operation timed out / Nothing was returned from the server / The connection to your server has timed out =
Each of these errors indicates that your website cannot be reached online. Solutions are as follows:
1. Make sure your site is available online at the moment.
2. It’s possible that your firewall blocks certain IP requests. Contact your system administrator or hosting provider support for details about this issue.

= POST Method Not Allowed =
This is a server error. Contact your system administrator or your hosting provider support to have POST method allowed for your server.

= Site is connected already by another account =
Each CMS2CMS user has the unique key which can be found in the Bridge file. So, the Bridge of user A is different from the Bridge of user B. If you have downloaded a bridge using one account, but you try to migrate with this bridge under another account, you get this error.

To fix it, you should either download the bridge again under the account you are going to use for migration or login to the account you used previously to download the Bridge file.

= Invalid response received =
Сontact us at support@cms2cms.com.

= An error occurred when trying to connect to your site =
Сontact us at support@cms2cms.com.

= An unknown error occurred =
Сontact us at support@cms2cms.com.


== Screenshots ==

1. /assets/screenshot-1.png
2. /assets/screenshot-2.png
3. /assets/screenshot-3.png
4. /assets/screenshot-4.png
5. /assets/screenshot-5.png

== Changelog ==

= 2.0.2 =
* Bug fixes

= 2.0.1 =
* Improved Connection Bridge

= 1.0.3 =
* Bug fixes

= 1.0.2 =
* Bug fixes

= 1.0.1 =
* Added German Language
* Minor fixes of html

= 1.0 =
* Initial commit