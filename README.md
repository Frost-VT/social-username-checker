# Social Username Availability Checker

This project quickly checks the availability of usernames in the following Services without the need for API connections::

- YouTube
- Twitch
- Instagram
- TikTok
- Threads
- BlueSky
- Twitter / X (New!)

## Platform Support

The original creator tested it on MacOS
It worked for me on Linux

## How to use

Clone the repository:
```bash
$ git clone https://github.com/Frost-VT/social-username-checker.git
```

Run your search using the `check.sh` file that exists in the project:
```bash
$ check.sh testingusername
```

You can alternately create a symbolic link:
```bash
$ sudo ln -s <PROJECT_FOLDER>/check.sh /usr/local/bin/social-check
```

And use the project:
```bash
$ social-check testingusername
```

Output:
<p>
  <img src="https://i.ibb.co/pRTL0D6/testing-social-username-checker.png" />
</p>

If you need to check multiple usernames, you can pass a list of usernames as follows:
```bash
$ social-check /tmp/usernames_to_test.txt
```
P.S.: After each username, the script will insert a random sleep between 2 and 15 seconds.

### Mode of Operation

### Limitations

## Social Media Username Rules

1. As far as I'm aware, every one of them is case insensitive || https://www.twitch.tv/FrostVT__ is the same as https://www.twitch.tv/frostvt__ 
2. I don't know which symbols are allowed and which aren't across these. If you find out, please update the README through a Pull Request.

### Youtube Channel Link
1. Prefixed with an @
2. Allowed characters are alphanumeric as well as some symbols. Period("."), Hyphen("-") and Underscore("_")
3. Cannot end the name with symbols

### Tiktok
1. Prefixed with an @

### BlueSky
1. Suffixed with .bsky.social

### Twitch, Instagram, X
(No rules outside of the general ones as far as I'm aware)

### Threads
Idk I don't use it

### Social Media Handled
- [x] YouTube  
- [x] Twitch  
- [x] Instagram  
- [x] TikTok  
- [x] Threads  
- [x] BlueSky  
- [x] X/Twitter  

### TODO
1. Add checks for invalid usernames for all the above social media, and update the README with exhaustive limits on the usernames
2. Create a more holistic check for X/Twitter that is able to account for usernames that are illegal due to banning (since they appear to be available but *aren't*)

Please open a new issue for things that I wasn't able to document in the README, or fix it and send a Pull Request and I'll merge it in ^^
