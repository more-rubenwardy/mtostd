---
title: Groups
version: proposal-20151114
layout: default
root: ../../
links:
- text: mtostd-groups
  url: index.html
  hr: true
- text: List of Known Groups
  url: list.html
---

## 0. mtostd-groups

### 0.1. Aims

* To define standard groups that mods can use without having to know about
  mods which implement it.
* To provide groups that content creators should add to their items.
* To document and summarize groups used by API mods.

### 0.2. Implementations

This is a proposal, and some/most of the groups may not be used yet.
However, you can install [mtstdlib]({{ page.root }}mtstdlib.html#requiring-a-group) to solve this.

### 0.3. List of Known Groups

See [list of known groups](list.html).

## 1. General Conventions

* Group names should be a description of what a single item is.
  eg: fancy stone should be in group:stone and not group:stones.
* Words should have underscores between them, eg: foo_bar.

## 2. Categories

### 2.1. Food

Edible items should all a food group with a value, rather arbitrarily defined as so:

* food=1 - small snacks, such as apples and chocolate bars.
* food=2 - small meals, such as sandwiches (lunch).
* food=3 - normal meals, such as pasta bakes and normal cakes.
* food=4 - large meals, such as large roast dinners and cakes.

The number is only a suggestion to a hunger mod what your food should be worth.

<aside class="warning">Warning: You will still need to add minetest.item_eat() to on_use</aside>

Foods should also have a group to represent what they are. The group name should
be prefixed with food_.

* food_pasta_bake
* food_baked_potato
* food_mash_potato_and_peas

### 2.2. Raw Resources

Raw resources don't need a prefix.

For example:

* wood
* stone
* wool

See the [list of known groups](list.html).
