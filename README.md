# CodeLupo
A variety Streamer. Stay Awesome, Stay Safe, Good Meow.

[Twitch](https://www.twitch.tv/codelupo), [YouTube](https://www.youtube.com/@codelupo), [Discord](https://discord.com/invite/B6dZ9DZS7q), [BlueSky](https://bsky.app/profile/codelupo.bsky.social), [Twitter/X](https://www.twitter.com/codelupo)

# YouTube/Twitch Chat Commands
| Command | Description | AllowedUser | 
| -------- | ------- | ------- |
| !help | Show help text and link to this GitHub Repo | all |
| !vote (reg poll) | Vote on Active Poll. You will be given 25 bisucits when you vote and 75 biscuits + poll_duration when the poll finishes. You can vote one of the following ways. If you don't provide a poll_name, the poll must be showing on the screen. <br />**Template**:  <br /> !vote {poll_name} {choice_num}. <br /> !vote {choice_num}  <br /> {choice_num} <br /> **E.g.** <br /> !vote game 2 <br /> !vote 2 <br /> 2 | all |
| !vote (pred poll) | Vote on Active Prediction Poll. You will be given 25 bisucits when you vote for free. You must use at least 50 biscuits to vote. You can vote one of the following ways. If you don't provide a poll_name, the poll must be showing on the screen. <br /> **Template**: <br />  !vote {poll_name} {choice_num} {biscuits} <br /> !vote {choice_num} {biscuits} <br /> {choice_num} {biscuits} <br /> **E.g.** <br /> !vote win 2 1500 <br /> !vote 2 1500  <br /> 2 1500  | all |
| !lurk | Let everyone know you're here but afk or won't be writing in chat. <br />**E.g.** !lurk | all |

# Biscuit/Point Usage
| Command | Description | Biscuits | AllowedUser | 
| -------- | ------- | ------- | ------- |
| !biscuits <br/> !points | Bot will replay with how many biscuits you have. <br/> **Template**: !biscuits <br/> **E.g.** !biscuits | 0 | all |
| !stats | Bot will replay with how many biscuits you have, All Time Biscuits and how much biscuits you lost to roulette. Each of the numbers will come back with ranking. The numbers are recalculated every 5min. <br/> **Template**: !stats <br/> **E.g.** !stats | 0 | all |
| !tts | Text To Speech app will read out your message. Available alias name: default, fool, zeus. <br/> **Template**: !tts {alias_name} "{message}" <br/> !tts {message} <br/> **E.g.** !tts fool "Hey, little cat. Do you want an apple?" <br/> !tts Meow!  | -1000 | all |
| !roulette | Gamble your biscuits for a chance to win more. <br/> **Template**: !roulette {biscuits} <br/> **E.g.** !roulette 100, !roulette all | x | all |
| !rmeme | Will display a random meme. <br/> **Template**: !rmeme <br/> **E.g.** !rmeme | -1000 | all |
| !soundboard <br/> !sb   | Play some audio from given list. Each viewer can use !soundboard meow once for free every stream.  <br/> **Template**: !soundboard {audio_name} <br/> **E.g.** !soundboard meow, !sb 9000 <br/> [All options](soundboard/README.md) Available audio_name: meow, wawa, 9000, xeno | -500 | all |


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

# Mod Chat Commands
| Command | Description | AllowedUser | 
| -------- | ------- | ------- |
| !so | Shoutout another streamer. Only on Twitch. <br/> **Template**: !so {tw_streamer_name} <br/> **E.g.** !so codelupo | mod |
| !newpoll | Create new poll. <br />**Template**: !newpoll {poll_name} "{description}" "{option_name_1}" ... "{option_name_5}" {active_hr}{day\|hr\|min}. <br />**E.g.** !newpoll game "Next Game codeLupo Plays" "Rain World" "Hollow Knight" "Wasteland 3" 168hr  | mod |
| !newpred | Create new prediction poll. Viewers can user points to predict the outcome. <br />**Template**: !newpred {poll_name} "{description}" "{option_name_1}" ... "{option_name_5}" {active_hr}{day\|hr\|min}. <br />**E.g.** !newpred win "Is codeLupo Him?" "Less than 30 tries" "More than 30 tries" 10min | mod |
| !endpoll | End an active poll. Use this to end a poll early. <br />**Template**: !endpoll {poll_name} <br />**E.g.** !endpoll game | mod |
| !endpred | Tell the system which prediction won. Viewers will be paid out afterwards. <br />**Template**: !endpred {poll_name} {won_option} <br />**E.g.** !endpred win 2 | mod |
| !cancelpred | Cancel a prediction if it has not been payed out yet. Biscuits will be returned back to the viewers. <br />**Template**: !endpred {poll_name} <br />**E.g.** !endpred win | mod |
| !showpolls | Use this command to make polls appear on the screen. The polls will be on the screen for few mins, afterwards will disappear for 20~ mins. So it doesn't get in the way of the game. <br /> **Template**: !showpolls <br />**E.g.** !showpolls | mod |

# Suggestions/Feedback
codeLupo is always happy to receive any and all feedback/suggsetion. **E.g.** 
- Allow us to get channel points by ...
- Allows us to use channel point for ...
- Please post more shorts
- Please talk less and play more. Or, play less and talk more.
- You play one game too long, play more games.
