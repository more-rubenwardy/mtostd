---
title: List - Groups
tagline: WIP. Last compiled 14th November 2015
layout: default
root: ../../
links:
- text: mtostd-groups
  url: index.html
  hr: true
- text: List of Known Groups
  url: list.html
---

## About this list

This is a collection of groups that fit mtostd-groups and are known to exist
in the wild. Most of the food_* ones are added

Also see [dev_wiki/Groups](http://dev.minetest.net/Groups)
and [dev_wiki/Custom_groups](http://dev.minetest.net/Groups/Custom_groups).

## Digging Groups

From [lua_api.txt](http://rubenwardy.com/minetest_modding_book/lua_api.html#known-damage-and-digging-time-defining-groups):

* crumbly - dirt, sand
* cracky - tough but crackable stuff like stone.
* snappy - something that can be cut using fine tools; e.g. leaves, smallplants, wire, sheets of metal
* choppy - something that can be cut using force; e.g. trees, wooden planks
* fleshy - Living things like animals and the player. This could imply some blood effects when hitting.
* explody - Especially prone to explosions
* oddly_breakable_by_hand - Torches, etc, quick to dig

## Nodes

### Classifications

* liquid - node is a liquid. Ratings - water=3, lava=2.
* water - node is water.
* lava - node is lava.
* sand - node is sand
* stone - node is stone
* wood - node is wood

### Behaviour

* flammable - can be set on fire. Higher values mean more flammable.
* puts_out_fire - if in a node with this group is near fire the fire gets extinguished.
* igniter - sets flammable nodes on fire. Rating defines the radius.
* leafdecay - node decays if no tree is in a radius of the rating.
* not_in_creative_inventory - the item is not added to the creative inventory.
* melty - node can be melted (used by steelblock, rating 3).
* hot - node is hot (used by lava, rating 3).

## Items

* vessel - item is a vessel.
* dye - for all groups that are defined by the dye mod see the init.lua of it.

## Living

### Plants

* Classifications:
    * tree - node is a tree. Leaves don't decay nearby.
    * flora - node is a flower
    * plant - node is a small-sized plant
* Naturally growing:
    * cocoa
    * orange
* Farmed:
    * carrot
    * flour
    * potato
    * rhubarb
    * strawberry
    * tomato
    * wheat

### Animal Products

* Diary
    * egg
    * butter
    * cheese
    * cream
    * milk
    * yogurt
* Meats
    * meat - any cooked meat.
    * raw_meat - uncooked meat.
    * food_beef
    * food_chicken
    * food_pork
    * food_venison - deer and wild game.

### Inedible

* wool - node is wool (default rating: 1)

## Minerals and Spices

* food_sugar

## Food

* food. See the [specification](index.html#food).
* food_chocolate - any chocolate
	* dark_chocolate
	* milk_chocolate
* food_baked_potato
