# Happy Hunting Grounds :stadium:
 > *I'm sorry, you can sit there and look and play with your silly machines as much as you like.*

Inspired by the game played on the [Football Cliches](https://open.spotify.com/show/6U4LfcF1ymFwxRDEsUq3Gd) podcast, this repository is a Web App that allows you to play the game for yourself.

## The Game :soccer:
Happy Hunting Grounds is a game creating by the Football Cliches podcast where players have to guess goalscorers for Premier League teams at away grounds, and therefore allowing the ground to be a **happy hunting ground** for that player.

In the game, you play three rounds and select a difficulty level before each round, determining how difficult the team and ground combination is to get a correct answer for.

In each round, you will guess a player and a season. If the player scored for that team at that ground in that season. You get the number of points based on the level you select.

If the player didn't score for that team in that season, but did score for that team in another season, you receive half the point based on the level you selected.

The difficulty level a team and ground combination is placed in is based on the number of unique player-season answers.

Manchester United at Goodison Park has the most such combinations, so would be Level 1. A fixture such as Manchester City at Boundary Park that has only one correct answer would be a level 10.

## The Repository :desktop_computer:
This Web App uses JavaScript to power the game, based on JSON data that contains the relevant teams, grounds, players, and fixtures required.

This data has been curated via a Python script to get it into the required format. That script is not included in this repository.

The data contained in the JSON is as follows

- Teams
  - Team ID and display name
- Grounds
  - Ground ID, display name, and compiled data of player-team combinations that have scored at that ground
- Players
  - Player ID, display name, and Opta ID (used for the headshots)
- Fixtures
  - Combined ground and team slug, then the date, scoreline, and scorers for each game that team played at that ground in each season

_Disclaimer: I do not own the rights to the Premier League player headshots, these are hosted on the Premier League's website._

### Future improvements I'd like to make :white_check_mark:
- [ ] Improve the difficulty level scoring. Likely something more clever that takes into account the player's career goals, perhaps
- [ ] Allow for multiplayer in the same window - this can currently be done by just having another tab/window open, but is difficult on mobile
- [ ] General UI improvements, it's definitely not my strong suit!

> [!NOTE]
> This Web App is not affiliated with the Football Cliches podcast