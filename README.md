------------------------------------------------------------------------------

Title: Gaming Profiles 2025 (Steam, PlayStation, Xbox)

Author: Artyom Kruglov on Kaggle https://www.kaggle.com/datasets/artyomkruglov/gaming-profiles-2025-steam-playstation-xbox

Additional cleaning by: Tara Jacobsen and Thihn Le 

# Data Overview
------------------------------------------------------------------------------

"This dataset was created for a comprehensive analysis of gaming platforms, user behavior, and pricing trends. It brings together real-world data from Steam, PlayStation, and Xbox, allowing researchers, analysts, and developers to explore player activity, game popularity, and price dynamics. The dataset enables insights into game market trends." (Kruglov). 



# Column Descriptions
------------------------------------------------------------------------------
## Playstation

### Achievements
| Column | The column indicates... | Data Type... |
|----------|----------|----------|
| 'achievementid' | unique achievementID, constructed as gameID + '_' + achievementNotUniqueID | integer | 
| 'gameid'  | unique gameID on the PlayStation platform | integer |
| 'title' |  achievement title | string |
| 'description' | description of how to unlock the achievement | string |
| 'rarity' | value of the achievement received | string |

### Games 
| Column | The column indicates... | Data Type... |
|----------|----------|----------|
| 'gameid' | unique gameID on the PlayStation platform | integer |
| 'title' | full title of the game | string |
| 'platform' | the platform the game was released on | string |
| 'developers' | a list of developers | list |
| 'publishers' | a list of publishers | list |
| 'genres' | a list of game genres | list |
| 'supported_languages' | languages available in the game as subtitles or voice-over | list |
| 'release_date' | game release date | datetime.date |
