CVE-2018-7600 | Drupal 8.5.x < 8.5.1 / 8.4.x < 8.4.6 / 8.x < 8.3.9 / 7.x? < 7.58 / < 6.x? - 'Drupalgeddon2' RCE (SA-CORE-2018-002)
Drupalggedon2 ~ https://github.com/dreadlocked/Drupalgeddon2/ (https://www.drupal.org/sa-core-2018-002)

Supports:

Drupal < 8.3.9 / < 8.4.6 / < 8.5.1 ~ user/register URL, attacking account/mail & #post_render parameter, using PHP's passthru function
Drupal < 7.58 ~ user/password URL, attacking triggering_element_name form & #post_render parameter, using PHP's passthru function
Works with direct commands (aka File-Less Method) or writes a PHP shell to the web root (./) or sub-directories (./sites/default/ & ./sites/default/files/)
Support Linux & Windows targets
Auto detects Drupal version (or takes a good guess!)
The user/register method was chosen for Drupal v8.x, as it will return HTTP 200, and render the output in the data JSON response (un-comment the code for timezone/#lazy_builder method, which will return HTTP 500 & blind!) (More Information)

Authors:

Hans Topo (@_dreadlocked)
g0tmi1k (@g0tmi1k)
Notes:

For advance users/setups there is a more customizable exploit. See the drupalgeddon2-customizable-beta.rb section
Before opening an issue, please, read the troubleshooting section at the end. Thanks!
