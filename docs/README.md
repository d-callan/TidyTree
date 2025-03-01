<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Table of Contents

*   [TidyTree][1]
    *   [Parameters][2]
    *   [setData][3]
        *   [Parameters][4]
    *   [setTree][5]
        *   [Parameters][6]
    *   [draw][7]
        *   [Parameters][8]
    *   [redraw][9]
    *   [recenter][10]
    *   [setLayout][11]
        *   [Parameters][12]
    *   [setColorOptions][13]
        *   [Parameters][14]
    *   [setMode][15]
        *   [Parameters][16]
    *   [setType][17]
        *   [Parameters][18]
    *   [setRotation][19]
        *   [Parameters][20]
    *   [setHStretch][21]
        *   [Parameters][22]
    *   [setVStretch][23]
        *   [Parameters][24]
    *   [setAnimation][25]
        *   [Parameters][26]
    *   [setBranchNodes][27]
        *   [Parameters][28]
    *   [eachBranchNode][29]
        *   [Parameters][30]
    *   [setBranchLabels][31]
        *   [Parameters][32]
    *   [eachBranchLabel][33]
        *   [Parameters][34]
    *   [setBranchDistances][35]
        *   [Parameters][36]
    *   [eachBranchDistance][37]
        *   [Parameters][38]
    *   [setLeafNodes][39]
        *   [Parameters][40]
    *   [eachLeafNode][41]
        *   [Parameters][42]
    *   [setEquidistantLeaves][43]
        *   [Parameters][44]
    *   [setLeafLabels][45]
        *   [Parameters][46]
    *   [eachLeafLabel][47]
        *   [Parameters][48]
    *   [setRuler][49]
        *   [Parameters][50]
    *   [getNodeGUIDs][51]
        *   [Parameters][52]
    *   [search][53]
        *   [Parameters][54]
    *   [on][55]
        *   [Parameters][56]
    *   [off][57]
        *   [Parameters][58]
    *   [trigger][59]
        *   [Parameters][60]
    *   [destroy][61]
    *   [validLayouts][62]
    *   [validTypes][63]
    *   [validModes][64]
    *   [validNodeColorModes][65]
    *   [validBranchColorModes][66]
*   [circularPoint][67]
    *   [Parameters][68]
*   [findNodeColor][69]
    *   [Parameters][70]
*   [findBranchColor][71]
    *   [Parameters][72]
*   [getAllLeaves][73]
    *   [Parameters][74]

## TidyTree

This class function creates a TidyTree object.

### Parameters

*   `data` &#x20;
*   `options` **[Object][75]** A Javascript object containing options to set up the tree
*   `events` &#x20;
*   `newick` **[String][76]** A valid newick string

### setData

Update the TidyTree's underlying data structure
There are two contexts in which you should call this:
1\. You wish to replace the tree with a completely different tree, given by a different newick string
2\. Your underlying tree data has changed (e.g. the tree has been re-rooted)

#### Parameters

*   `data` **[Object][75]** A patristic.Branch object

Returns **[Object][75]** the TidyTree object

### setTree

Update the TidyTree's underlying data structure
There are two contexts in which you should call this:
1\. You wish to replace the tree with a completely different tree, given by a different newick string
2\. Your underlying tree data has changed (e.g. the tree has been re-rooted)

#### Parameters

*   `newick` **[String][76]** A valid newick string

Returns **[Object][75]** the TidyTree object

### draw

Draws a Phylogenetic on the element referred to by selector

#### Parameters

*   `selector` **[String][76]** A CSS selector

Returns **[TidyTree][1]** the TidyTree object

### redraw

Redraws the links and relocates the nodes accordingly

Returns **[TidyTree][1]** The TidyTree Object

### recenter

Recenters the tree in the center of the view

Returns **[TidyTree][1]** The TidyTree object

### setLayout

Set the TidyTree's layout

#### Parameters

*   `newLayout` **[String][76]** The new layout

Returns **[TidyTree][1]** The TidyTree Object

### setColorOptions

Set the TidyTree's colorOptions

#### Parameters

*   `newColorOptions` **[Object][75]** The new colorOptions

Returns **[TidyTree][1]** The TidyTree Object

### setMode

Set the TidyTree's mode

#### Parameters

*   `newMode` **[String][76]** The new mode

Returns **[TidyTree][1]** The TidyTree object

### setType

Set the TidyTree's type

#### Parameters

*   `newType` **[Boolean][77]** The new type

Returns **[TidyTree][1]** the TidyTree object

### setRotation

Set the TidyTree's rotation

#### Parameters

*   `degrees` **[Number][78]** The new number of degrees by which to rotate the tree

Returns **[TidyTree][1]** the TidyTree object

### setHStretch

Set the TidyTree's Horizontal Stretch

#### Parameters

*   `proportion` **[Number][78]** The new proportion by which to stretch the tree

Returns **[TidyTree][1]** the TidyTree object

### setVStretch

Set the TidyTree's Vertical Stretch

#### Parameters

*   `proportion` **[Number][78]** The new proportion by which to stretch the tree

Returns **[TidyTree][1]** the TidyTree object

### setAnimation

Set the TidyTree's animation time. Note that this does not trigger a
redraw.

#### Parameters

*   `time` **[number][78]** The desired duration of an animation, in ms. Set to 0
    to turn animations off completely.

Returns **[TidyTree][1]** The TidyTree object

### setBranchNodes

Shows or hides the Branch Nodes

#### Parameters

*   `show` **[Boolean][77]** Should Branch nodes be shown?

Returns **[TidyTree][1]** the TidyTree object

### eachBranchNode

Restyles Leaf Nodes

#### Parameters

*   `styler` **[Function][79]** A function that restyles each node. `styler`
    receives a reference to the DOM node to be styled, and an associated data
    object.

Returns **[TidyTree][1]** the TidyTree Object

### setBranchLabels

Set the TidyTree's branchLabels

#### Parameters

*   `show` **[Boolean][77]** Should the TidyTree show branchLabels?

Returns **[TidyTree][1]** the TidyTree Object

### eachBranchLabel

Restyles Branch Label

#### Parameters

*   `styler` **[Function][79]** A function that restyles each node. `styler`
    receives a reference to the DOM node to be styled, and an associated data
    object.

Returns **[TidyTree][1]** the TidyTree Object

### setBranchDistances

Shows or hides the TidyTree's branch labels

#### Parameters

*   `show` **[Boolean][77]** Should the TidyTree show branch distances?

Returns **[TidyTree][1]** The TidyTree Object

### eachBranchDistance

Restyles Branch Distances

#### Parameters

*   `styler` **[Function][79]** A function that restyles each node. `styler`
    receives a reference to the DOM node to be styled, and an associated data
    object.

Returns **[TidyTree][1]** the TidyTree Object

### setLeafNodes

Shows or Hides the Leaf Nodes

#### Parameters

*   `show` **[Boolean][77]** Should leaf nodes be visible?

Returns **[TidyTree][1]** The TidyTree Object

### eachLeafNode

Restyles Leaf Nodes

#### Parameters

*   `styler` **[Function][79]** A function that restyles each node. `styler`
    receives a reference to the DOM node to be styled, and an associated data
    object.

Returns **[TidyTree][1]** the TidyTree Object

### setEquidistantLeaves

Set the TidyTree's leaves to be equidistant

#### Parameters

*   `isEquidistant` &#x20;

### setLeafLabels

Shows or Hides the TidyTree's Leaf Labels

#### Parameters

*   `show` **[Boolean][77]** Should the TidyTree show leafLabels?

Returns **[TidyTree][1]** the TidyTree Object

### eachLeafLabel

Restyles Leaf Labels

#### Parameters

*   `styler` **[Function][79]** A function that restyles each node. `styler`
    receives a reference to the DOM node to be styled, and an associated data
    object.

Returns **[TidyTree][1]** the TidyTree Object

### setRuler

Shows or hides the TidyTree's branch labels

#### Parameters

*   `show` **[Boolean][77]** Should the TidyTree show branchLabels?

Returns **[TidyTree][1]** The TidyTree Object

### getNodeGUIDs

Retrieves the GUIDs of the nodes in the TidyTree instance.

#### Parameters

*   `leavesOnly` **[boolean][77]** Whether to retrieve GUIDs only for leaf nodes.
*   `predicate` **[function][79]** A function that returns true if the node should be included

Returns **[Array][80]** An array of GUIDs of the nodes.

### search

Searches the tree, returns Search Results

#### Parameters

*   `test` **[Function][79]** A function which takes a Branch and returns a Truthy
    or Falsy value.

Returns **[Array][80]** The array of results

### on

Attaches a new event listener
Please note that this is not yet functioning.

#### Parameters

*   `events` **[String][76]** A space-delimited list of event names
*   `callback` **[Function][79]** The function to run when one of the `events` occurs.

Returns **[TidyTree][1]** The TidyTree on which this method was called.

### off

Removes all event listeners from the given events

#### Parameters

*   `events` **[String][76]** A space-delimited list of event names

Returns **[TidyTree][1]** The TidyTree on which this method was called.

### trigger

Forces the tree to respond as though an `event` has occurred

#### Parameters

*   `events` **[String][76]** space-delimited list of names of events to trigger.
*   `args` **Spread** Any arguments which should be passed to the event
    handler(s).

Returns **any** The output of the callback run on `event`

### destroy

Destroys the TidyTree

Returns **[undefined][81]**&#x20;

### validLayouts

The available layouts for rendering trees.

Type: [Array][80]

### validTypes

The available types for rendering branches.

Type: [Array][80]

### validModes

The available modes for rendering branches.

Type: [Array][80]

### validNodeColorModes

The available color modes for rendering nodes.

Type: [Array][80]

### validBranchColorModes

The available color modes for rendering branches.

Type: [Array][80]

## circularPoint

Calculate the coordinates of a point transformed onto a circle.

### Parameters

*   `x` **[number][78]** The x-coordinate of the center of the point.
*   `y` **[number][78]** The y-coordinate of the center of the point.

Returns **[Array][80]<[number][78]>** The new x and y coordinates of the point on the circle.

## findNodeColor

Finds the color of a given node based on the color options provided.

### Parameters

*   `node` **[Object][75]** The node for which to find the color.
*   `colorOptions` **[Object][75]** The color options object containing the color mode, leavesOnly, predicate, default color, and highlight color.

Returns **[string][76]** The color of the node.

## findBranchColor

Find the color of a given link based on the provided color options.

### Parameters

*   `link` **[string][76]** The link for which to find the color.
*   `colorOptions` **[object][75]** The options for different link colors.

Returns **[string][76]** The color of the link.

## getAllLeaves

Returns an array of all the child leaf nodes of the given node in a tree.

### Parameters

*   `node` **[Object][75]** A node of the tree.
*   `includeSelf` **[boolean][77]** Whether to include the given node itself as a leaf node. Defaults to false.

Returns **[Array][80]** An array of leaf nodes.

[1]: #tidytree

[2]: #parameters

[3]: #setdata

[4]: #parameters-1

[5]: #settree

[6]: #parameters-2

[7]: #draw

[8]: #parameters-3

[9]: #redraw

[10]: #recenter

[11]: #setlayout

[12]: #parameters-4

[13]: #setcoloroptions

[14]: #parameters-5

[15]: #setmode

[16]: #parameters-6

[17]: #settype

[18]: #parameters-7

[19]: #setrotation

[20]: #parameters-8

[21]: #sethstretch

[22]: #parameters-9

[23]: #setvstretch

[24]: #parameters-10

[25]: #setanimation

[26]: #parameters-11

[27]: #setbranchnodes

[28]: #parameters-12

[29]: #eachbranchnode

[30]: #parameters-13

[31]: #setbranchlabels

[32]: #parameters-14

[33]: #eachbranchlabel

[34]: #parameters-15

[35]: #setbranchdistances

[36]: #parameters-16

[37]: #eachbranchdistance

[38]: #parameters-17

[39]: #setleafnodes

[40]: #parameters-18

[41]: #eachleafnode

[42]: #parameters-19

[43]: #setequidistantleaves

[44]: #parameters-20

[45]: #setleaflabels

[46]: #parameters-21

[47]: #eachleaflabel

[48]: #parameters-22

[49]: #setruler

[50]: #parameters-23

[51]: #getnodeguids

[52]: #parameters-24

[53]: #search

[54]: #parameters-25

[55]: #on

[56]: #parameters-26

[57]: #off

[58]: #parameters-27

[59]: #trigger

[60]: #parameters-28

[61]: #destroy

[62]: #validlayouts

[63]: #validtypes

[64]: #validmodes

[65]: #validnodecolormodes

[66]: #validbranchcolormodes

[67]: #circularpoint

[68]: #parameters-29

[69]: #findnodecolor

[70]: #parameters-30

[71]: #findbranchcolor

[72]: #parameters-31

[73]: #getallleaves

[74]: #parameters-32

[75]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Object

[76]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/String

[77]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Boolean

[78]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Number

[79]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Statements/function

[80]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/Array

[81]: https://developer.mozilla.org/docs/Web/JavaScript/Reference/Global_Objects/undefined
