
# Application.LoadWebPane Event (Project)

 **Last modified:** July 28, 2015

Occurs when Project loads a Web pane for  **Task Drivers**,  **Deliverables**, or the  **Project/Resource Import Wizard**.

## Syntax

 _expression_. **LoadWebPane**( **_Window_**,  **_TargetPage_**)

 _expression_A variable that represents an  **Application** object.


### Parameters



|**Name**|**Required/Optional**|**Data Type**|**Description**|
|:-----|:-----|:-----|:-----|
|Window|Required| **Window**|The window from where the  **LoadWebBrowserControl** method was called.|
|TargetPage|Required| **String**|The same TargetPage parameter that was used to call the  **LoadWebBrowserControl** method.|

### Return Value

nothing


## Remarks

Project events do not occur when the project is embedded in another document or application.

