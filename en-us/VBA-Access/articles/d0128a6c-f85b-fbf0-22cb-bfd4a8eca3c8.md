
# Call Procedures in a Subform or Subreport

 **Last modified:** July 28, 2015

 _**Applies to:** Access 2013_

You can call a procedure in a module associated with a subform or subreport in one of two ways. If the form containing the subform is open in Form view, you can refer to the procedure as a method on the subform. The following example shows how to call the procedure GetProductID in the Orders subform, which is bound to a subform control on the Orders form:

In the Orders Subform class module, enter this code:



```
Public Function GetProductID() As Variant 
 ' Return current productID. 
 GetProductID = ProductID 
End Function 
```

The following code illustrates how to call the GetProductID procedure.



```
Forms!Orders![Orders Subform].Form.GetProductID
```

