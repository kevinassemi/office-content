
# ToggleButton.ForeTint Property (Access)

 **Last modified:** July 28, 2015

 **In this article**
 [Syntax](#sectionSection0)
 [Remarks](#sectionSection1)
 [Example](#sectionSection2)


Gets or sets the tint that is applied to the theme color in the  **ForeColor** property of the specified object. Read/write **Single**.


## Syntax
<a name="sectionSection0"> </a>

 _expression_. **ForeTint**

 _expression_A variable that represents a  **ToggleButton** object.


## Remarks
<a name="sectionSection1"> </a>

The  **ForeTint** property contains a numeric expression that can be used to lighten the theme color in the **ForeColor** property. The default value of the **ForeTint** property is 100, which is neutral, and does not change the theme color. To lighten the color, first determine the percentage by which to lighten from 1 to 100, then subtract that value as a whole number from 100 and use the remainder. For example, to lighten the theme color by 75%, subtract 75 from 100 and use the remainder, which is 25.

This property is not surfaced in the property sheet. 


## Example
<a name="sectionSection2"> </a>

The following code example lightens the  **ForeColor** by 75%.


```
Me.ctl.ForeTint=25
```


## See also
<a name="sectionSection2"> </a>


#### Concepts


 [ToggleButton Object](1c20d809-d7db-e096-4328-ebb4d79e770e.md)
#### Other resources


 [ToggleButton Object Members](487101e7-c090-eb79-3671-5c9ce86cb6b0.md)
