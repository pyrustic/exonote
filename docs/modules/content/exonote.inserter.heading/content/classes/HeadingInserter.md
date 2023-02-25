Back to [All Modules](https://github.com/pyrustic/blob/master/docs/modules/README.md#readme)

# Module Overview

**exonote.inserter.heading**
 
No description

> **Classes:** &nbsp; [HeadingInserter](https://github.com/pyrustic/blob/master/docs/modules/content/exonote.inserter.heading/content/classes/HeadingInserter.md#class-headinginserter)
>
> **Functions:** &nbsp; None
>
> **Constants:** &nbsp; None

# Class HeadingInserter
No description.

## Base Classes
object

## Class Attributes
No class attributes.

## Class Properties


# All Methods
[\_\_init\_\_](#__init__) &nbsp;&nbsp; [insert](#insert) &nbsp;&nbsp; [\_bind\_on\_click\_heading](#_bind_on_click_heading) &nbsp;&nbsp; [\_bind\_on\_hover\_heading](#_bind_on_hover_heading) &nbsp;&nbsp; [\_insert\_bottom\_margin](#_insert_bottom_margin) &nbsp;&nbsp; [\_insert\_top\_margin](#_insert_top_margin) &nbsp;&nbsp; [\_on\_button\_1\_press\_heading](#_on_button_1_press_heading) &nbsp;&nbsp; [\_on\_button\_1\_release\_heading](#_on_button_1_release_heading) &nbsp;&nbsp; [\_on\_button\_3\_press\_heading](#_on_button_3_press_heading) &nbsp;&nbsp; [\_on\_button\_3\_release\_heading](#_on_button_3_release_heading) &nbsp;&nbsp; [\_on\_enter\_heading](#_on_enter_heading) &nbsp;&nbsp; [\_on\_leave\_heading](#_on_leave_heading)

## \_\_init\_\_
Initialize self.  See help(type(self)) for accurate signature.



**Signature:** (self, viewer)





**Return Value:** None

[Back to Top](#module-overview)


## insert
No description



**Signature:** (self, index, data)





**Return Value:** None

[Back to Top](#module-overview)


## \_bind\_on\_click\_heading
No description



**Signature:** (self, sid, generic\_tag, tag)





**Return Value:** None

[Back to Top](#module-overview)


## \_bind\_on\_hover\_heading
handler = (lambda e, editor=editor, h=h, hover_info=hover_info:
           _on_enter_heading(editor, h, hover_info))
editor.tag_bind(tag, "<Enter>", handler, True)
# on pointer leaves link
handler = (lambda e, editor=editor, h=h:
           _on_leave_heading(editor, h))
editor.tag_bind(tag, "<Leave>", handler, True)



**Signature:** (self, hover\_info, tag)





**Return Value:** None

[Back to Top](#module-overview)


## \_insert\_bottom\_margin
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_insert\_top\_margin
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_button\_1\_press\_heading
No description



**Signature:** (self, generic\_tag, tag)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_button\_1\_release\_heading
No description



**Signature:** (self, sid, generic\_tag, tag)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_button\_3\_press\_heading
No description



**Signature:** (self, generic\_tag, tag)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_button\_3\_release\_heading
No description



**Signature:** (self, sid, generic\_tag, tag)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_enter\_heading
h.enter_event("hover", **hover_info)
editor.config(cursor="hand1")



**Signature:** (self, hover\_info)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_leave\_heading
No description



**Signature:** (self, h)





**Return Value:** None

[Back to Top](#module-overview)



