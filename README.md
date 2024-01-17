# SonoBoss: Siri Shortcut for ChatGPT-smart Sonos Speaker Control

## Overview
SonoBoss is a Siri Shortcut designed for seamless voice control of Sonos speakers. It acts as a virtual assistant for a hands-free music experience.

## Functionality
- **Voice Command Activation:** Simply say, "Hey Siri, SonoBoss" to activate.
- **Music Playback:** Supports playing songs, artists, albums, playlists, or Sonos favorites from Apple Music, Spotify, Deezer, and local Music Libraries.
- **Custom Clips and Announcements:** Play custom MP3 clips or make announcements through Sonos speakers.
- **Speaker Control:** Perform basic commands like play, pause, volume adjustment, muting, and more for designated rooms.

## Sample of what you can ask SonoBoss
- “Play Dancing Queen by Abba in the Kitchen”
- “Play clip doorbell in the Living Room”
- “Announce dinner is ready in the Office”
- “Pause the Living Room”
- “Resume playing in the Living Room”
- “Increase volume in the Living Room [by ten]”
- “Set volume in the Living Room to fifteen”
- “Mute / unmute the Living Room”
- “Previous / next / skip track in the Living Room”
- “Shuffle queue of the Living Room”
- “Clear queue of the Living Room”
- “Kitchen join Living Room”
- “Kitchen leave”

## Technical Integration & credits
- **Siri Shortcuts:** Leverages Siri for voice and chat commands.
- **node-sonos-http-api:** Enables music search and the discovery and control of Sonos speakers on your network.
- **OpenAI API Integration:** Enhances command processing with two models:
  - **gpt-4:** Advanced, with flexible search terms.
  - **gpt-3.5-turbo:** Capable amd more cost-effective, requires specific search terms.

## Music Service Compatibility
Compatible with Spotify, Apple Music, Deezer, and local Music Libraries.

## Preparation for Installation
- Install and configure [node-sonos-http-api](https://github.com/jishi/node-sonos-http-api/) on your local network.
- Ensure access to [OpenAI API](https://api.openai.com).
- Sign up and obtain an API key from [OpenAI's platform](https://platform.openai.com).
- Ensure there is enough pay-as-you-go balance in your OpenAI account.
- Configure Siri for accurate speech recognition.
- Enable iCloud Drive for storing data.

## Setup and Configuration
1. Have your Sonos HTTP API bridge URL and OpenAI API key ready.
2. Choose your preferred Music source.
3. Choose your preferred OpenAI model.
4. Decide on your logging preferences.
5. [Download the SonoBoss Siri Shortcut](https://www.icloud.com/shortcuts/1e06c2b1f4b14df187aa7c0a7b97001a).
6. At first, run the Shortcut without invoking Siri. This trains Siri that a Shortcut named SonoBoss exists.  
7. Allow connections to your Sonos HTTP API bridge, to api.openai.com and allow for additions to the Notes app.
-  If notifiation "file x.TXT does not exist" appears, your iCloud drive connection is stale. open Files -> iCloud -> Shortcuts -> SonoBoss -> today's date to resolve.

## Siri prompt guidelines
- **First Run:** Include the room name when you open a conversation
- **Include room name:** Include the room name when you open a conversation
- **Elaborate:** Whereas OpenAI gpt-4 is more capable at determining if Abba is an artist, a song or a playlist; gpt-3.5-turbo is not. 

## Advanced Usage
- Be aware of OpenAI API token pricing.
- SonoBoss tracks token consumption and costs, with logs available in iCloud Drive.

## Optimization
- The system prompt can be edited for performance and token consumption optimization.

## Conclusion
SonoBoss simplifies Sonos speaker management with intuitive voice commands, bridging advanced technology and everyday convenience.


