Want to contribute to making these setting better for wider system configurations? Fork this repository and make a pull request!


---------------------

We all love being on VRChat, desktop, mobile, Standalone, PCVR, whatever have you.

However, performance comes into question pretty quickly, notably with larger instances.
Here’s what I’ve tested that works on a range of systems in PCVR, with a potato system and a respectable system to create a range for all systems to use.

Updated 05/05/2025 (May 5th, 2025)
Changelog:
This update adjusts some remaining formatting issues, as well as adds in guidance for Avatar Download Prioritization.



Robots? - Shield Settings

The first place to start, and the easiest to change too! When you open your quick menu, you'll see a button named "Change Shield Level" chilling in the bottom right of the main panel, and clicking it brings up a drawer with four options; `Maximum`, `Normal`, `None`, and `Custom`. To set a Custom Shield level, click on "Custom", then expand the view using the "Expand" icon in the upper right-hand corner of the slide-up. This will open the main menu so you can customize the settings for the Custom Shield Level. You can customize the settings here for each rank (& Friends) as you please.

You can toggle an Override using the "Show Avatar" buttons in the user's menu when selecting them from your Quick Menu, either to fully show, or fully hide an avatar.

- Generally, it’s recommended you have the tightest settings for Visitors and New Users to prevent crashers from ruining your day.
- Settings for higher ranks will depend mainly on your system, and what framerate you are comfortable with. Systems with lower overall specs should keep these tight, just like the settings for lower trust ranks.
- It is recommended to keep `Shaders` and `Lights And Particles` disabled for every rank, keeping it to only those you fully show.
- Avatars overridden will not follow shield settings - as they are either fully shown or fully hidden!
	- Having too many avatars overridden to fully show can negatively impact performance.

Diamonds! - Avatar Culling

Here's another quick setting you can adjust on the fly! Culling avatars from view can reduce unnecessary rendering strain on your system, making it a really useful tool.

You can find this setting in your quick menu's Settings tab (it's a cog/gear icon) in an aptly named category "Avatar Culling". You can tune this as much as you wish, show as many or as few as you want!

- While systems do vary, we generally recommend settings of 8m distance and 6 avatars shown for a balance of performance and seeing people.
- There's some extra toggles just below, make sure that both "Always Show Friends" and "Always show overridden avatars" are Off, as these are shown regardless of your culling settings.
- All users outside of the culling area, over the closest avatar count, or both will be diamonds.

There is a neat trick with this setting if you find yourself way over your VRAM usage, set Nearest Avatars to 0 and wait for 5-10 minutes for your VRAM to clear up, revert to where it was before to resume viewing avatars.


It's a wee bit loud? - Earmuff Mode

It's fairly common that during events there are a lot of people talking and cracking jokes in groups small and large throughout the event world. There's one group of settings that you can swiftly enable (or disable) to comfort your ears (or to stir chaos in them)!
These are found in your Quick Menu under the Audio Settings tab (it's a speaker icon) and in there are your normal settings. If you scroll down you will come across the Earmuff Mode settings.

- The settings of `Distance`, `Falloff`, `Outside Volume` and a few others adjust how your earmuff mode behaves. These settings take effect immediately and dynamically as you change them. Adjust these to your comfort, but generally I recommend 1.5m distance, 0.2m falloff, and 5% outside volume.
- Need to quickly take them off or slap them on? Double click the Audio Settings tab to quickly enable or disable them!



Why is it so smooth? - Graphical Settings


Ever wondered why your pixels are being smoothed, even if your per-eye resolution is higher than the headset? That’s a setting called Anti-Aliasing, and while fine on Desktop, generally it’s not fine in VR for most people.

So how do I turn this setting off? - It’s in your big settings menu (open your Quick Menu, and double click the cog icon) and select “Graphics” on the left-hand side. It will be underneath “Graphics Quality”.

	- Anti-Aliasing (also known as “AA”) is an edge-smoothing setting, great for desktop mode! But this performance hit for larger screens is amplified for VR.
- Generally, it is advised to disable this setting if you have anything lower than a 3090/4080Super/5080TI, or AMD equivalent while in VR.
- Other settings in here, like Pixel Light Count, and Particle Limiter also reside in here.
	• Particle Limiter should always be Enabled, even on high-end systems. This is a built-in particle crasher protection.
	• Pixel Light Count is used by quite a few things, like Video Screens for world illumination, flash lights, and of course DPS/TPS/SPS. You can adjust this setting as you wish, but generally you can disable them if you don’t need them.



That's too large! - Avatar Download & Uncompressed Size


There are quite a few avatars out there that are rather rude to take up more resources than they need to, combined with the fact that a lot of people are unable to afford to upgrade their systems. These settings aim to ease your RAM usage, hopefully sparing your system for another day from overstuffing itself on the delectable data-turkey we call avatars.

You can find these settings in the Main Menu, double press your Quick Menu button to open up the Main Menu, then go to the Settings tab (cog/gear icon) and navigate to Avatars. Once you scroll down enough you will see `Maximum Download Size` and `Max Uncompressed Size`, these will depend on your system and your internet connection.

- Max Uncompressed Size is the amount of System RAM the avatar takes up after decompression to appear on your screen. This setting is heavily dependent on how much RAM is installed in your system. Generally, we recommend following this rough guideline;
 	 • 45-65 MB for 16GB or less.
 • 80-100 MB for 32GB
 • 125-175 MB for 64GB or higher
- Using tighter Uncompressed Size limits can also positively affect VRAM usage.
- (Optional) For maximum download size, take your Internet Speed and how long you’d like to wait for avatars to download into account. Generally, we recommend anywhere between 50 and 130MB.

Too many to load! - Download Prioritization

Have slow internet, or just a really crappy PC that can not load too many people at once? There’s a group of settings for that! It’s located near the bottom of the Avatars page in your big settings menu, and it’s a category called “Avatar Download Prioritization”. This group of settings controls how and when avatars are downloaded, starting nearby first then going out. By default this should be on and set to 5m.

 You can disable this setting by toggling the switch to “off” (Not Recommended)
The range of the slider is from 0m to 100m. I generally recommend anywhere between 2m and 10m for the majority of systems.
There’s two settings underneath, “Prioritize Manually Shown” and “Prioritize Friends”, make sure that Friends are prioritized and manually shown are not.
This setting can give you time to activate Safety Mode, same with Shield Mode, incase of crashers being reported in the instance.

Not enough room! - Moving and/or increasing cache size (Advanced, PC Only)
Using the guidelines in the official VRChat Docs we can manipulate the cache’s size and location, great if you need to increase your cache size to reduce load times, extra lag in heavy instances from cache clearing, as well as the increasingly common error robot showings.

Some things to note:
The cache will always default to C:\Users\<username>\AppData\LocalLow\VRChat\vrchat no matter where your game is installed.
The cache defaults to 30GB on PC, and 20GB on Mobile/Standalone. Only the PC version can change their cache size.
The minimum cache size is 30GB, while the max is the size of whatever drive the cache is on.
The cache is recommended to not share the same disk as an active Operating System, as well as being on some sort of speedy NVMe SSD, and be at least 1TB in size.
(Optional) You can set a length of time for cache to “expire” and get cleared out, by default this is 30 days but you can set it to longer than that. Generally, you only should do this with large or very large (=<500GB) cache allocations.

You’ll want to make this file a .json, however you can make it as a config.txt first, then rename the file’s extension. Once created you can then start configuring as you please with anything in the linked above document page, though all you should need is in the following example:

{
cache_size": 500, <- Cache size in GB, 30GB minimum.
"cache_expiry_delay": 30,<- This is redundant, but useful to solve some funky issues.
"cache_directory": "E:\\cache" <- Storage directory for cache, avoid // as it’s a JSON escape symbol.
}

	With it set, you then place it into the listed directory above and then run VRChat to verify everything works, as long as you don’t get tossed into the error world, you’ll be fine.
