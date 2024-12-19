# CodeLupo
A variety Streamer. Stay Awesome, Stay Safe, Good Meow.

[Twitch](https://www.twitch.tv/codelupo), [YouTube](https://www.youtube.com/@codelupo), [Discord](https://discord.com/invite/B6dZ9DZS7q), [BlueSky](https://bsky.app/profile/codelupo.bsky.social), [Twitter/X](https://www.twitter.com/codelupo)

# YouTube/Twitch Chat Commands
| Command | Description | AllowedUser | 
| -------- | ------- | ------- |
| !help | Show help text and link to this GitHub Repo | all |
| !vote | Vote on Active Poll. You will be given 50 bisucits when you vote, also 50 biscuits + poll_duration when the poll finishes. <br />Template: !vote {poll_name} {choice_num}. <br />E.g. !vote game 2 | all |
| !newpoll | Create new poll. <br />Template: !newpoll {poll_name} "{option_name_1}" ... "{option_name_5}" {multi} {pred} {active_hr}hr. <br />E.g. !newpoll game "Rain World" "Hollow Knight" "Wasteland 3" 168hr | codeLupo |
| !endpoll | End an active poll. <br />Template: !endpoll {poll_name} <br />E.g. !endpoll game | codeLupo |
| !lurk | Let everyone know you're here but afk or won't be writing in chat. | all |
| !so | Shoutout another streamer. Only on Twitch. <br/> Template: !so {tw_streamer_name} <br/> E.g. !so codelupo | mod |

# Biscuit/Point Usage
| Command | Description | Biscuits | AllowedUser | 
| -------- | ------- | ------- | ------- |
| !biscuits <br/> !points | Bot will replay with how many biscuits you have. <br/> Template: !biscuits <br/> E.g. !biscuits | 0 | all |
| !tts | Text To Speech app will read out your message. <br/> Template: !tts {message} <br/> E.g. !tts Meow!  | -1000 | all |
| !roultete | Gamble your biscuits for a chance to win more. <br/> Template: !roulette {biscuits} <br/> E.g. !roulette 100, !roulette all | x | all |
| !rmeme | Will display a random meme. <br/> Template: !rmeme <br/> E.g. !rmeme | -1000 | all |
| !soundboard <br/> !sb   | Play some audio from given list. Each viewer can use !soundboard meow once for free every stream.  <br/> Template: !soundboard {audio_name} <br/> E.g. !soundboard meow, !sb 9000 <br/> [All options](soundboard/README.md) Available audio_name: meow, wawa, 9000, xeno | -500 | all |


Viewer must chat for the system recognise that the given viewer is watching. Viewer gets 5 biscuits / 1 min. The system tries to estimate for how long the viewer has watched the stream.
- Individual message: System assume viewer has watched the stream for 10min.
- 2 individual messages where gap is less than an hour:
  - System assume the viewer has watched the stream for the time between the two messages. 
  - Msg2 - Msg1 => time * biscuits 
- 2 individual messages where gap is more than an hour:
  - System assume the viewer has partially watched the stream.
  - Msg2 - Msg1 => time * biscuits * 0.75
- Viewer uses !lurk
  - System assume the viewer is watching the stream for the next 2 hours
  - Viewer gets full points for next 2 hours.  

# Suggestions/Feedback
codeLupo is always happy to receive any and all feedback/suggsetion. E.g. 
- Allow us to get channel points by ...
- Allows us to use channel point for ...
- Please post more shorts
- Please talk less and play more. Or, play less and talk more.
- You play one game too long, play more games.
