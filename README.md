# Obsidian Textual Conceptmap

Objective is to have a simple concept map in text form within one Obsidian Note that uses the power of hovering over Obsidian links and seeing other blocks.

Although not as good as a true concept map as a graph it does have the advantage that you
- can explore concepts quickly within the same note
- avoid having to have a separate Obsidian Note for each each concept and messing up your vault

An html page with a javascript that creates an obsidian note that links the concepts together so hovering shows the concept linkages.

The html page has an input textarea where each concept is on one line and structured as

> ```node from // link type // node to```

> > ```*Note 'node from', 'link type' and 'node to' can be obdisian links to other pages if required*```
```
like this

Climate Change // is a // Force Of Nature
Force of Nature // affects // Climate Change
Nature // reacts to // Climate Change
Climate Change // is caused by // Natural Causes
Natural Causes // are a // Force of Nature
Climate Change // is caused by // Human Activities
Human Activities // such as // Population Increase
Human Activities // such as // Burning Fossil Fuels
Rising Sea Levels // are evidence for // Climate Change
Melting Ice Caps // are evidence for // Climate Change
Warming Oceans // are evidence for // Climate Change
Warming Oceans // impact // Animal Habitat
Climate Change // can be managed by // Changing Behavior
Climate Change // can be managed by // Environmental Policies
Environmental Policies // such as // Carbon Taxes
Environmental Policies // such as // Political Sanctions
Climate Change // should be further // Researched
Changing Behavior // such as // Recycling
Changing Behavior // will assist // Carbon Reduction
Carbon Reduction // will stop // Melting Ice Caps
Recycling // hinders // Carbon Reduction
```

The output textarea contains the Obsidian markdown that will show the concepts using block references links ([[#^blockreference]] within the **same** Obsidian note.

block references are the node title followed by -ctm (context map suffix) so as not to conflict with any other block references in the Obsidian note.

Each node from is formatted as follows (note the blank lines)

```
- Changing Behavior
>- such as [[#^recycling|Recycling]]
> - will assist [[#^carbonreduction|Carbon Reduction]]

^changingbehavior-ctm

```




