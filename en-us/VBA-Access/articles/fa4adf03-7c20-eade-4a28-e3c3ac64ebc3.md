
# TextBox.IMEMode Property (Access)

 **Last modified:** July 28, 2015






## Syntax

 _expression_. **IMEMode**

 _expression_A variable that represents a  **TextBox** object.


## Remarks

The  **IMEMode** property uses the following settings.



|**Setting**|**Description**|**Visual Basic**|
|:-----|:-----|:-----|
|No Control|Kanji Conversion Mode not set (default).|0|
|On|Turns on Kanji Conversion Mode.|1|
|Off|Turns off Kanji Conversion Mode.|2|
|Disable|Disables Kanji Conversion Mode.|3|
|Hiragana|Sets full pitch hiragana|4|
|Full pitch Katakana|Sets full pitch katakana.|5|
|Half pitch Katakana|Sets half pitch katakana.|6|
|Full pitch Alpha/Num|Sets full pitch letters/numbers.|7|
|Half pitch Alpha/Num|Sets half pitch letters/numbers.|8|
|HangulFull|Sets full pitch hangul.|9|
|Hangul|Sets half pitch hangul.|10|
You can specify the Kanji Conversion Mode when the focus shifts to control by setting the  **IMEMode** property. If set to No Control (default) the setting before the focus shifted to that control is used. For any other setting, the Kanji Conversion Mode setting for that control is used. For example, if the **IMEMode** property is set to Off, the Kanji Conversion Mode is turned off, and if the **IMEMode** property is set to On, the Kanji Conversion Mode is turned on. The Kanji Conversion Mode automatically changes each time the focus shifts between controls.


 **Note**   If set to Disable, the Kanji Conversion Mode settings cannot be changed. If any other setting is used, the Kanji Conversion Mode can be changed, but when the focus changes, the settings are lost. If you want to save the settings before the control loses the focus, set the **IMEHold/HoldKanjiConversionMode**property.


## See also


#### Concepts


 [TextBox Object](d74fbe9a-0d40-7d28-956f-a2bfd0cfee45.md)
#### Other resources


 [TextBox Object Members](bb55abbc-902e-fc2d-bdff-063c55426cd0.md)
