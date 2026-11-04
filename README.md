# LoL-match-predictor
Using statistical tools, this project aims to try make an accurate prediction of the winning odds of both teams based on the characters picked for the game League of Legends

## Goals
League of Legends is an amazingly complex game, with 10 players choosing from 171 characters each with unique abilities and tens of thousands of decisions to made each game. It is no wonder no game is the same. Despite this, the overall community understands that some characters are counters (more likely to win into an enemy champion) or synergises (more likely to win when paired together) well together.

As an example of counters, If all the enemy players pick physical damaging characters then Malphite, who is an armour stacking tank, will do amazingly into them.

Despite the community knowing of lane matchups being important, many players disregard how important the whole draft is to who they decide to play. 

Hence, the goal of this project is to investigate the statistical differences in character picks and thus help players make more informed decisions on who to play when

## Scope

In this project I plan to show:

-A proof of concept that there is a statistical significant connection between all character choices in a game 
-Develop a interface where players can input the current champion picks and it will suggest champions to play
-Investigate other factors of champion drafting such as what makes a character safe to pick first with no information (blinding) 

A larger Scope for a V2 would include:

-A GUI app which would be able to read the current draft and suggest characters to play with an overlay, taking into consideration what characters you are strong in
-An investigation into item statistics (Inspired by zPetu's paper)
-Training a ML model for more accurate predictions of game state.

## Limitations

As of now the RiotAPI only allows for harvesting data at rates of 100 games every 2 minutes. As a result harvesting a significant amount of data to test for other factors such as winrates differing in different elo (skill level) brackets will not be included in the main scope. As of now my limitations are

-Data harvesting, One API key will mean either relying on second hand data or slow personal gathering. Second hand data is a valid option however I have decided against it due to reasons listed below
-Working patch, League of Legends gets balance updates every 2 weeks which will change how strong or weak certain characters and items are. The difference in each patch is small but after a few months the characters who are strong and weak can dramatically change, especially around Decemeber and January when major gameplay updates occur.
-Compute Power, This type of problem could fit a ML approach very well however due to limited hardware I will only pursue this after my initial investigation

## Acknowledgements

This project is heavily inspired by projects such as Draft.AI which can read your LoL client and suggest champions you can pick. This is what i want to recreate with my own trained ML if possible. Additionally zPetu's was my personal inspiration for approaching games in a statistical way due to his own youtube videos and masters paper talking about similar topics on item statistics. 
