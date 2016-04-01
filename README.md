# adapt-dragAndDrop
A basic drag and drop question component.

[Visit the **DragAndDrop** wiki](https://github.com/BATraining/adapt-dragAndDrop/wiki) for more information about its functionality and for explanations of key properties.

## Installation

* If **DragAndDrop** has been uninstalled from the Adapt framework, it may be reinstalled.
With the [Adapt CLI](https://github.com/adaptlearning/adapt-cli) installed, run the following from the command line:
    `adapt install adapt-dragAndDrop`

    Alternatively, this component can also be installed by adding the following line of code to the *adapt.json* file:  
        `"adapt-dragAndDrop": "*"`  
    Then running the command:  
        `adapt install`  
    (This second method will reinstall all plug-ins listed in *adapt.json*.)  

* If **DragAndDrop** has been uninstalled from the Adapt authoring tool, it may be reinstalled using the [Plug-in Manager](https://github.com/adaptlearning/adapt_authoring/wiki/Plugin-Manager).  
<div float align=right><a href="#top">Back to Top</a></div>

## Usage

This component can be used as part of an assessment.

## Settings overview

A complete example of this components settings can be found in the [example.json](https://github.com/BATraining/adapt-dragAndDrop/blob/master/example.json) file. A description of the core settings can be found at: [Core model attributes](https://github.com/adaptlearning/adapt_framework/wiki/Core-model-attributes)

### Attributes

Further settings for this component are:

**_component** (string): This value must be: `dragAndDrop`

**_classes** (string): CSS class name to be applied to **DragAndDrop**’s containing `div`. The class must be predefined in one of the Less files. Separate multiple classes with a space.

**_layout** (string): This defines the horizontal position of the component in the block. Acceptable values are `full`, `left` or `right`.

**_defaultWidth** (number): Default width of an item.

**_defaultHeight** (number): Default height of an item.

**_shouldScale** (boolean): Select 'true' to scale container based on number of draggable items it contains.

**_draggableItems** (object): This element of the settings contains the draggable items.

>**id** (string): Draggable Item Id naming convention (ex. drag-01).

>**title** (string): Draggable item display title.

>**body** (string): Draggable item body text.

>**_graphic** (object): An optional image which is displayed to the item body. It contains values for **src** and **alt**.

>>**src** (string): File name (including path) of the image. Path should be relative to the *src* folder (e.g., *course/en/images/c-45-1.jpg*).

>>**alt** (string): This text becomes the image’s `alt` attribute.

**_droppableItems** (object): This element of the settings contains the droppable items.

>**id** (string): Droppable Item Id naming convention (ex. drop-01).

>**title** (string): Droppable item display title.

>**body** (string): Droppable item body text.

>**correctItemId** (string): This should match up with the correct Draggable item to go in the drop area (ex. enter 'drag-01' if correct).

>**_graphic** (object): An optional image which is displayed to the item body. It contains values for **src** and **alt**.

>>**src** (string): File name (including path) of the image. Path should be relative to the *src* folder (e.g., *course/en/images/c-45-1.jpg*).

>>**alt** (string): This text becomes the image’s `alt` attribute. 

### Accessibility
**DragAndDrop** has been assigned a label using the [aria-label](https://github.com/adaptlearning/adapt_framework/wiki/Aria-Labels) attribute: **ariaRegion**. This label is not a visible element. It is utilized by assistive technology such as screen readers. Should the region's text need to be customised, it can be found within the **globals** object in [*properties.schema*](https://github.com/BATraining/adapt-dragAndDrop/blob/master/properties.schema).
<div float align=right><a href="#top">Back to Top</a></div>

## Limitations

To be completed

##Browser spec

This component has been tested to the standard Adapt browser specification.
