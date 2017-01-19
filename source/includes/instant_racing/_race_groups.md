# Instant Racing: RaceGroups

## RaceGroup Object

```json
{
  "id":1,
  "name": "San Francisco",
  "description": "City by the bay",
  "locked": false,
  "current_points": 100,
  "unlock_points":100,
  "unlock_cost":0,
  "wager_count": 6,
  "race_count": 1,
  "winning_win_count": 1,
  "winning_place_count": 1,
  "winning_show_count": 1,
  "winning_exacta_count": 1,
  "winning_trifecta_count": 1,
  "winning_superfecta_count": 1,
  "biggest_win": 1000.0
}
```

Field | Description
----- | -----------
id |
name |
description |
locked | boolean indicating if this group is locked or unlocked for the user
current_points | current points awarded to unlock this group
unlock_points | total points to unlock this group
unlock_cost | coin cost to unlock group
wager_count | total number of wagers a user has placed on this race group
race_count | total number of races a user has played on this race group
winning_win_count | number of winning win bets a user has placed on this race group
winning_place_count | number of winning place bets a user has placed on this race group
winning_show_count | number of winning show bets a user has placed on this race group
winning_exacta_count | number of winning exacta bets a user has placed on this race group
winning_trifecta_count | number of winning trifecta bets a user has placed on this race group
winning_superfecta_count | number of winning superfecta bets a user has placed on this race group
biggest_win | biggest payout for a wager on this race group
## Get all Race Groups

Returns all the race groups, ordered as they should be shown to the user.

<aside class="warning">
This endpoint subject to change soon.
</aside>

> Example

```curl
curl -H "Application-Name: super-fun-game" \
  -H "Authorization: Bearer ABC123" \
  https://api.derbygames.com/api/instant_racing/race_groups
```

`GET /instant_racing/race_groups`

### Returns

An array of `RaceGroup` objects.