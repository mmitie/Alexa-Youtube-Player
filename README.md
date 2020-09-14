
# Alexa-Youtube-Player
Amazon Alexa skill to play audio from YouTube

The purpose of this project is to enable users to listen to audio from Youtube on their Alexa devices. This skill searches for a set of YouTube videos based on a search term provided by the user, and then plays the audio from the most relevant video, while enqueueing the next most-relevant tracks to be played after. There are also several options provided to manage playback settings, namely: previous, next, pause, resume, and repeat mode (which is looping the audio).

## Usage
As noted at the end of the previous section, your first invocation of the skill, started by telling an Alexa device to "Alexa launch youtube player" will result in a response informing you that the database is being configured. After waiting about 10 seconds, the skill should be ready to use.

### Commands:
:boom: General Commands
* "Alexa open youtube player"
	* Starts the skill, which will prompt you for the name of a song (or other audio) that you would like to hear
* "Alexa ask youtube player to play {Song Name}"
	* Loads the requested audio from YouTube and begins playback
* "Alexa ask youtube player for help"
	* Returns a short help message with some possible commands to use

2. Commands to use during playback
* "Alexa ask youtube player Play", or "Alexa ask youtube player Resume", "Alexa ask youtube player Stop", "Alexa ask youtube player Previous", "Alexa ask youtube player Next", and "Alexa ask youtube player Start Over"
	* These commands are mostly self-explanatory.  "Previous" and "Next" will change the currently playing song to either the one playing before it , or the next song in the queue. There are 20 songs by default in each queue, and after the 20th song, playback will loop back to the 1st song. "Start Over" will replay the current song from the beginning.
* "Alexa ask youtube player to repeat"
	* Turns on Single Repeat Mode. This will result in the currently playing song to repeat indefinitely (until a Stop/Previous/Next/Start Over command is given, or a new song is requested to play).
* "Alexa ask youtube player to stop repeating" of "Alexa ask youtube player to turn repeat off"
	* Turns off Single Repeat Mode
* "Alexa ask youtube player what song this is" or "Alexa ask youtube player for song info"
	* Returns the title of the YouTube video that the currently playing audio was sourced from
