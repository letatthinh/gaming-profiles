
Title: Gaming Profiles 2025 (Steam, PlayStation, Xbox)

Author: Artyom Kruglov on Kaggle https://www.kaggle.com/datasets/artyomkruglov/gaming-profiles-2025-steam-playstation-xbox

Additional cleaning by: Thinh Le and Tara Jacobsen

Dashboard url: https://app.powerbi.com/links/UpfI5J1SWn?ctid=bb0fe58b-be24-419c-b689-7b624bae76d8&pbi_source=linkShare

Presentation url: https://docs.google.com/presentation/d/1HE57_e19hRmgc-AGhAY96G9wcbpy8MAtlGtvoBqzkpA/edit?usp=sharing 

PowerBI file: https://drive.google.com/file/d/1lr2TcnOUSgiD-cM7aFMa8bU_1oEDca1F/view?usp=sharing

Cleaned data: https://drive.google.com/drive/folders/1yPKENZmfXokdhLorBTYNetdhCTc-SI7I?usp=sharing

# Data Overview

"This dataset was created for a comprehensive analysis of gaming platforms, user behavior, and pricing trends. It brings together real-world data from Steam, PlayStation, and Xbox, allowing researchers, analysts, and developers to explore player activity, game popularity, and price dynamics. The dataset enables insights into game market trends." (Kruglov). 

# Column Descriptions

## Playstation

### `achievements`

| Column | Description | Data Type |
|----------|----------|----------|
| `achievementid` | unique achievementID, constructed as gameID + '_' + achievementNotUniqueID | integer | 
| `gameid` | unique gameID on the PlayStation platform | integer |
| `title` |  achievement title | string |
| `description` | description of how to unlock the achievement | string |
| `rarity` | value of the achievement received | string |

### `games` 

| Column | Description | Data Type |
|----------|----------|----------|
| `gameid` | unique gameID on the PlayStation platform | integer |
| `title` | full title of the game | string |
| `platform` | the platform the game was released on | string |
| `developers` | a list of developers | string |
| `publishers` | a list of publishers | string |
| `genres` | a list of game genres | string |
| `supported_languages` | languages available in the game as subtitles or voice-over | string |
| `release_date` | game release date | datetime |

### `history`

| Column | Description | Data Type |
|----------|----------|----------|
| `playerid` | unique userID on the PlayStation platform who earned achievementID | integer |
| `achievementid` | unique achievementID, constructed as gameID + '_' + achievementNotUniqueID | integer |
| `date_acquired` | timestamp of when the achievement was earned | datetime |

### `players`

| Column | Description | Data Type |
|----------|----------|----------|
| `playerid` | unique userID on the PlayStation platform | integer |
| `nickname` | user nickanme | string |
| `country` | the country in which the user resides | string |

### `prices`

| Column | Description | Data Type |
|----------|----------|----------|
| `gameid` | unique gameID on the PlayStation platform | integer |
| `usd` | game price in USD | float |
| `eur` | game price in EUR | float |
| `gbp` | game price in GBP | float |
| `jpy` | game price in JPY | float |
| `rub` | game price in RUB | float |
| `date_acquired` | date of when the price information was recorded | datetime |

### `purchased_games`

| Column | Description | Data Type |
|----------|----------|----------|
| `playerid` | unique userID on the PlayStation platform | integer |
| `library` | a list of purchased games for the entire usage period | string |

## Steam

### `achievements`

| Column | Description | Data Type |
|----------|----------|----------|
| `achievementid` | unique achievementID, constructed as gameID + '_' + achievementNotUniqueID | string | 
| `gameid` | unique gameID on the Steam platform | integer |
| `title` |  achievement title | string |
| `description` | description of how to unlock the achievement | string |

### `friends`

| Column | Description | Data Type |
|----------|----------|----------|
| `playerid` | unique userID on the Steam platform | integer | 
| `friends` | a list of user friendships | string |

### `games`

| Column | Description | Data Type |
|----------|----------|----------|
| `gameid` | unique gameID on the Steam platform | integer |
| `title` | full title of the game | string |
| `platform` | the platform the game was released on | string |
| `developers` | a list of developers | string |
| `publishers` | a list of publishers | string |
| `genres` | a list of game genres | string |
| `supported_languages` | languages available in the game as subtitles or voice-over | string |
| `release_date` | game release date | datetime |

### `history`

| Column | Description | Data Type |
|----------|----------|----------|
| `playerid` | unique userID on the Steam platform who earned achievementID | integer |
| `achievementid` | unique achievementID, constructed as gameID + '_' + achievementNotUniqueID | string |
| `date_acquired` | timestamp of when the achievement was earned | datetime |

### `players`

| Column | Description | Data Type |
|----------|----------|----------|
| `playerid` | unique userID on the Steam platform | integer |
| `country` | the country in which the user resides | string |
| `created` | date of creation of the gaming profile | datetime |

### `prices`

| Column | Description | Data Type |
|----------|----------|----------|
| `gameid` | unique gameID on the Steam platform | integer |
| `usd` | game price in USD | float |
| `eur` | game price in EUR | float |
| `gbp` | game price in GBP | float |
| `jpy` | game price in JPY | float |
| `rub` | game price in RUB | float |
| `date_acquired` | date of when the price information was recorded | datetime |

### `private_steamids`

| Column | Description | Data Type |
|----------|----------|----------|
| `playerid` | unique userID with hidden profiles on Steam platform | integer |

### `purchased_games`

| Column | Description | Data Type |
|----------|----------|----------|
| `playerid` | unique userID on the Steam platform | integer |
| `library` | a list of purchased games for the entire usage period | string |

### `reviews`

| Column | Description | Data Type |
|----------|----------|----------|
| `reviewid` | unique reviewID (Serial Key) | integer |
| `playerid` | userID on the Steam platform who submitted the review | integer |
| `gameid` | gameID for which the review was written | integer |
| `review` | user-submitted review for the game | string |
| `helpful` | number of users who found the review helpful | integer |
| `funny` | number of users who found the review funny | integer |
| `awards` | number of awards given to the review | integer |
| `posdted` | timestamp of when the review was posted | datetime |


## Xbox

### `achievements`

| Column | Description | Data Type |
|----------|----------|----------|
| `achievementid` | unique achievementID, constructed as gameID + '_' + achievementNotUniqueID | string | 
| `gameid` | unique gameID on the Xbox platform | integer |
| `title` |  achievement title | string |
| `description` | description of how to unlock the achievement | string |
| `point` | number of points awarded for earning the achievement | float |

### `games`

| Column | Description | Data Type |
|----------|----------|----------|
| `gameid` | unique gameID on the Xbox platform | integer |
| `title` | full title of the game | string |
| `platform` | the platform the game was released on | string |
| `developers` | a list of developers | string |
| `publishers` | a list of publishers | string |
| `genres` | a list of game genres | string |
| `supported_languages` | languages available in the game as subtitles or voice-over | string |
| `release_date` | game release date | datetime |

### `history`

| Column | Description | Data Type |
|----------|----------|----------|
| `playerid` | unique userID on the Xbox platform who earned achievementID | integer |
| `achievementid` | unique achievementID, constructed as gameID + '_' + achievementNotUniqueID | string |
| `date_acquired` | timestamp of when the achievement was earned | datetime |

### `players`

| Column | Description | Data Type |
|----------|----------|----------|
| `playerid` | unique userID on the PlayStation platform | integer |
| `nickname` | user nickanme | string |

### `prices`

| Column | Description | Data Type |
|----------|----------|----------|
| `gameid` | unique gameID on the Xbox platform | integer |
| `usd` | game price in USD | float |
| `eur` | game price in EUR | float |
| `gbp` | game price in GBP | float |
| `jpy` | game price in JPY | float |
| `rub` | game price in RUB | float |
| `date_acquired` | date of when the price information was recorded | datetime |

### `purchased_games`

| Column | Description | Data Type |
|----------|----------|----------|
| `playerid` | unique userID on the Xbox platform | integer |
| `library` | a list of purchased games for the entire usage period | string |


