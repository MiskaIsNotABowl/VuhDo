
# Auras - setting up HoT and Debuff Icons

Due to Blizzard's addon changes for Midnight and Forever, the old debuff, HoT, and HoT bars tabs are no more.
Instead, there's the new Aura system. This combines HoTs and Debuffs.

This will be a (hopefully) quick guide on how this system works and how to set up your things.

## Table Of Contents <!-- omit in toc -->
- [TL:DR - Where'd all my settings go?](#tldr---whered-all-my-settings-go)
- [How Auras get displayed: Panels → Auras](#how-auras-get-displayed-panels--auras)
  - [Aura Icon Setup](#aura-icon-setup)
  - [Aura Bar Setup](#aura-bar-setup)
- [Which Auras to track: Auras → Groups](#which-auras-to-track-auras--groups)
  - [List-Type Auras: Add individual Auras](#list-type-auras-add-individual-auras)
  - [Filter-Type Auras](#filter-type-auras)
  - [Bar Colors (Custom, Dispel, Glow)](#bar-colors-custom-dispel-glow)
- [Global Defaults: Colors → Auras](#global-defaults-colors--auras)



## TL:DR - Where'd all my settings go?

<u>The way you set up Auras:</u>
- Create a Group in [Auras → Groups](#which-auras-to-track-auras--groups)
- Choose where and how your Aura Groups show up in [Panels → Auras](#how-auras-get-displayed-panels--auras) using different Anchors. 

The default Aura Groups can't be edited, but you can make copies of them and edit those. Make sure to also update the corresponding anchor in Panels → Auras

<u>There's two types of Aura Groups:</u>

**List:** Add Auras you want to track by name or SpellID. You can track Buffs on friendly units, and Debuffs on hostile units.

**Filter:** Use filter conditions to show Groups of Auras. The filters are controlled by Blizzard, the tooltips should give you a general idea of what Blizz says is in there.


## How Auras get displayed: Panels → Auras

This is where you can configure which Aura Groups actually show up on your frames, and how.

These settings are per-panel, so to apply them to all of your panels, use the "apply all"-button on the bottom right. Otherwise, only your selected panel  will be impacted by the changes you make here. 

If you're not sure which panel is currently selected, you can see the Panel above the VuhDo Options, e.g. Panel #1. Additionally, if you look at the frames you've set up, each panel will have its label above it, e.g. PANEL 1. The currently selected one will be flashing. You can select a different panel by clicking its label.

<!--
![Panel Number Options](/images/panel-number-panel.png)
 
![Panel Number Options](/images/panel-number-options.png) 
-->

<img src="images/panel-number-panel.png" alt="Panel number displayed on the panel" width="100"/>
<img src="images/panel-number-options.png" alt="Panel number displayed above VuhDo Options" width="110"/>


### Aura Icon Setup

Now for the settings. These look like a lot at first, so I'll go over them bit by bit.

<!--![Radio Buttons](images/auras-top-left.png)-->

<img src="images/auras-top-left.png" alt="Top Left part of Panels→Auras" width="650"/>

Here, you can enable or disable an anchor to toggle its icons showing. (Note that this doesn't affect debuff or custom colors.)

Use the Anchor Dropdown to choose which Anchor to work on. Each Anchor can hold one of your [Aura Groups](#which-auras-to-track-auras--groups). 

The Dropdown right below lets you choose which Aura Group to display on this Anchor, with the Group button taking you to the selected Aura Group's edit page.

<!--![Radio Buttons](images/auras-radio-buttons.png)-->
<img src="images/auras-radio-buttons.png" alt="Radio Points for Anchor Selection" width="650"/>

With these buttons, you can choose where the Aura Group on this anchor shows up.

If you pick a spot from the top example bar, your auras will show up in a line starting at that spot.

Choose one of the presets below it if you prefer a setup where each icon shows up in a different corner of your frames.

I recommend you never choose the same spot for two Anchors, as this will make them overlap.

<img src="images/auras-dropdowns.png" alt="Top Left part of Panels→Auras" width="650"/>

<!--![Aura Dropdown Menus](images/auras-dropdowns.png)-->

These dropdown menus let you choose exactly how your icons are going to show up. Let's go over each one.

<u>Growth:</u> This decides, which direction the icons grow in, starting from the anchor point. I.e. when choosing "right", the second icon appears to the right of the first icon.

<u>Wrap:</u> Choose where icons should start again, once the number set with the "Max Columns"

<u>Sort:</u> Choose how a filter-type Aura Group's icons should be sorted.

<u>Order:</u> Choose whether the sorting order should be applied in ascending or descending order.

<u>Style:</u> Choose whether you'd like the Auras here to show up as icons or bars (similar to the old HoT bars). More about Aura Bars [here](#aura-bar-setup).

<u>Color:</u> Choose if Bar Colors (for Aura Bars) Should have their default color (set in Auras → Colors or [per spell](#filter-type-auras)<!--platzhalter bis das fertig ist, dann link ersetzen-->), dispel colors or class colors.

<u>Icon Type:</u> Use the default icon, a glossy or flat texture, or no icon at all (helpful for bars).

<u>Stack Type:</u> Choose if you want stacks to display as numbers or triangles.
<!-- Didn't Blizz break that? eh, whatever -->

### Aura Bar Setup

<!--hier fehlt alles-->

## Which Auras to track: Auras → Groups

 **None of the premade Groups can be edited**. 
 To still customize them, select the Aura Group you'd like to use as a base, then click "Copy".  This will copy all settings from the original, but make them editable. You may also give this Group a new name.

### List-Type Auras: Add individual Auras

First off: Because of Blizzard's restrictions, this only works for Buffs on friendly, and debuffs on hostile units. For debuffs on your party, you'll have to use a [Filter-Type Aura](#filter-type-auras).

<!--ehh hier fehlt was-->


### Filter-Type Auras

<!--ehh hier fehlt alles-->

 ### Bar Colors (Custom, Dispel, Glow)

 You can then set a **Color Type** for an Aura Group. The choices here are *Custom* and *Debuff*. Additionally, you can configure a bar glow, or a sound that plays, when any of the Auras in this Group are applied.


**Custom:** You may set a custom color for when **any** of the Auras in this Group are active on the player. You can click the example bar shown to change the Colors for both Text and the bar itself for this Aura Group. 
Coloring a bar, when, for example, specifically "Atonement" is on a bar is currently not possible.
 
**Dispel:** This uses the Colors configured under Colors>States. The best use for it is on a debuff-based Group, like "Relevant Debuffs".
 
Changing these Color settings applies the colors **regardless** of whether or not the Aura Group is anchored to any Panels (Anchors will be explained [here](#how-Auras-get-displayed-panels--Auras)). This is useful for when you want your frames to turn certain colors, but not show any icons.

The priority slider controls which Aura Group's color settings take precedence over other Aura Groups. The lower the number, the higher the priority.

Example:
- Aura Group 1 has debuff colors enabled and a priority of 50
- Aura Group 2 has custom colors enabled and a priority of 10

When Auras from both Groups are present, the custom color of Aura Group 2 takes priority
 
*Note that the main default Aura a lot of people will be using to track Debuffs, **"Dispellable Debuffs", already has its bar colors configured** to the "Dispel"-Colors, so **you won't need to do this manually.***
 
If you'd like the color settings of a built-in Group to not apply anymore, simply uncheck the "Enable" Box at the top of the Aura Group. This will also disable this group for selection in Panels → Auras. If you'd like to keep icons without colors, create a copy, disable colors for this copy and anchor it instead.

## Global Defaults: Colors → Auras

<!--hier fehlt noch alles-->

<u>Order of Precedence:</u>

Spell-specific settings you make within an aura group in Auras → Groups will take priority over the settings you make for an anchor in Panels → Auras. 

Any settings you make in Panels->Auras will take priority over Colors → Auras.