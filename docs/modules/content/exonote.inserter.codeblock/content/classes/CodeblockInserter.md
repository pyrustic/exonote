Back to [All Modules](https://github.com/pyrustic/exonote/blob/master/docs/modules/README.md#readme)

# Module Overview

**exonote.inserter.codeblock**
 
No description

> **Classes:** &nbsp; [CodeblockInserter](https://github.com/pyrustic/exonote/blob/master/docs/modules/content/exonote.inserter.codeblock/content/classes/CodeblockInserter.md#class-codeblockinserter)
>
> **Functions:** &nbsp; None
>
> **Constants:** &nbsp; None

# Class CodeblockInserter
No description.

## Base Classes
object

## Class Attributes
No class attributes.

## Class Properties


# All Methods
[\_\_init\_\_](#__init__) &nbsp;&nbsp; [insert](#insert) &nbsp;&nbsp; [\_bind\_on\_click\_codeblock](#_bind_on_click_codeblock) &nbsp;&nbsp; [\_bind\_on\_hover\_codeblock](#_bind_on_hover_codeblock) &nbsp;&nbsp; [\_on\_button\_3\_press\_codeblock](#_on_button_3_press_codeblock) &nbsp;&nbsp; [\_on\_button\_3\_release\_codeblock](#_on_button_3_release_codeblock) &nbsp;&nbsp; [\_on\_enter\_codeblock](#_on_enter_codeblock) &nbsp;&nbsp; [\_on\_leave\_codeblock](#_on_leave_codeblock)

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


## \_bind\_on\_click\_codeblock
No description



**Signature:** (self, text, tag)





**Return Value:** None

[Back to Top](#module-overview)


## \_bind\_on\_hover\_codeblock
handler = (lambda e, editor=editor, h=h, hover_info=hover_info:
           _on_enter_codeblock(editor, h, hover_info))
editor.tag_bind(tag, "<Enter>", handler, True)
# on pointer leaves codeblock
handler = (lambda e, editor=editor, h=h:
           _on_leave_codeblock(editor, h))
editor.tag_bind(tag, "<Leave>", handler, True)



**Signature:** (self, status\_info, tag, statusbar)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_button\_3\_press\_codeblock
No description



**Signature:** (self, tag)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_button\_3\_release\_codeblock
No description



**Signature:** (self, text, tag)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_enter\_codeblock
h.enter_event("hover", **hover_info)
editor.config(cursor="hand1")



**Signature:** (self, statusbar, status\_info)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_leave\_codeblock
No description



**Signature:** (self, statusbar)





**Return Value:** None

[Back to Top](#module-overview)



