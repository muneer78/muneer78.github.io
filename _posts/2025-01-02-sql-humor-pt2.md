---
date: 2025-01-02
title: SQL humor, pt. 2
tags: coding
layout: post
---

Ingredients for 21 year old Muneer to have a great time:

~~~SQL
WITH strip_club AS 
(SELECT *
FROM world.gentlemansclubs
WHERE dancer.status != 'pregnant'
	AND cover.charge IS NULL),
WITH shawtys AS
(SELECT *
FROM world.women
WHERE bitchy IS NULL
	AND MAX(DTF)
	AND MIN(commitment)
	AND clinger.stage < 5)
liquor AS
(SELECT *
FROM world.drinks
WHERE liquor.type NOT IN(‘wine’,’tequila’),
WITH video_games AS
(SELECT *
FROM games.systems
WHERE systems.type NOT IN(‘Atari 2600’, ‘Commodore 64’)
	AND game.title != ‘Battletoads’),
SELECT *
FROM tear_da_club_up
LEFT JOIN shawtys
LEFT JOIN strip_club
LEFT JOIN liquor
LEFT JOIN video_games
ORDER BY fun DESC
~~~