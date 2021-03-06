
# ShapeRange.Flip Method (Publisher)

 **Last modified:** July 28, 2015

 **In this article**
 [Syntax](#sectionSection0)
 [Remarks](#sectionSection1)
 [Example](#sectionSection2)


Flips the specified shape around its horizontal or vertical axis, or flips all the shapes in the specified shape range around their horizontal or vertical axes.


## Syntax
<a name="sectionSection0"> </a>

 _expression_. **Flip**( **_FlipCmd_**)

 _expression_A variable that represents a  **ShapeRange** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
|FlipCmd|Required| **MsoFlipCmd**| Specifies whether the shape is flipped horizontally or vertically.|

## Remarks
<a name="sectionSection1"> </a>

The FlipCmd parameter can be one of the following  **MsoFlipCmd** constants declared in the Microsoft Office type library.



| **msoFlipHorizontal**|
| **msoFlipVertical**|

## Example
<a name="sectionSection2"> </a>

This example adds a triangle to the first page of the active publication, duplicates the triangle, and then flips the duplicate triangle vertically and makes it red.


```
With ActiveDocument.Pages(1).Shapes _ 
 .AddShape(Type:=msoShapeRightTriangle, _ 
 Left:=10, Top:=10, Width:=50, Height:=50) _ 
 .Duplicate 
 .Fill.ForeColor.RGB = RGB(255, 0, 0) 
 .Flip msoFlipVertical 
End With 

```

