Back to [All Modules](https://github.com/pyrustic/exonote/blob/master/docs/modules/README.md#readme)

# Module Overview

**exonote.viewer**
 
No description

> **Classes:** &nbsp; [Viewer](https://github.com/pyrustic/exonote/blob/master/docs/modules/content/exonote.viewer/content/classes/Viewer.md#class-viewer)
>
> **Functions:** &nbsp; None
>
> **Constants:** &nbsp; None

# Class Viewer
No description.

## Base Classes
object

## Class Attributes
No class attributes.

## Class Properties
|Property|Type|Description|Inherited from|
|---|---|---|---|
|anchors|getter|List of anchors||
|cache|getter|None||
|coords|getter|None||
|data|getter|None||
|dossier|getter|None||
|editor|getter|None||
|filename|getter|None||
|history|getter|None||
|inserter|getter|None||
|on_open|getter|None||
|on_open|setter|None||
|pages|getter|None||
|readonly|getter|None||
|restriction|getter|None||
|root|getter|None||
|scroll_step|getter|None||
|sids|getter|Ordered list of SIDs (Section IDs)||
|statusbar|getter|None||
|style|getter|None||
|update_sys_path|getter|None||



# All Methods
[\_\_init\_\_](#__init__) &nbsp;&nbsp; [clear](#clear) &nbsp;&nbsp; [clear\_section](#clear_section) &nbsp;&nbsp; [compute\_index](#compute_index) &nbsp;&nbsp; [del\_heading](#del_heading) &nbsp;&nbsp; [del\_section](#del_section) &nbsp;&nbsp; [disable\_edit\_mode](#disable_edit_mode) &nbsp;&nbsp; [edit\_heading](#edit_heading) &nbsp;&nbsp; [edit\_section](#edit_section) &nbsp;&nbsp; [enable\_edit\_mode](#enable_edit_mode) &nbsp;&nbsp; [extend\_section](#extend_section) &nbsp;&nbsp; [get\_heading](#get_heading) &nbsp;&nbsp; [get\_index](#get_index) &nbsp;&nbsp; [get\_section](#get_section) &nbsp;&nbsp; [goto](#goto) &nbsp;&nbsp; [look\_ahead](#look_ahead) &nbsp;&nbsp; [look\_behind](#look_behind) &nbsp;&nbsp; [make\_scrollable](#make_scrollable) &nbsp;&nbsp; [next\_id](#next_id) &nbsp;&nbsp; [open](#open) &nbsp;&nbsp; [read\_heading](#read_heading) &nbsp;&nbsp; [read\_section](#read_section) &nbsp;&nbsp; [refresh](#refresh) &nbsp;&nbsp; [register\_anchor](#register_anchor) &nbsp;&nbsp; [register\_section](#register_section) &nbsp;&nbsp; [render](#render) &nbsp;&nbsp; [\_bind\_handlers\_to\_tags](#_bind_handlers_to_tags) &nbsp;&nbsp; [\_compute\_single\_index](#_compute_single_index) &nbsp;&nbsp; [\_create\_top\_bottom\_anchors](#_create_top_bottom_anchors) &nbsp;&nbsp; [\_define\_alignment\_tags](#_define_alignment_tags) &nbsp;&nbsp; [\_define\_caption\_tag](#_define_caption_tag) &nbsp;&nbsp; [\_define\_centered\_component\_tags](#_define_centered_component_tags) &nbsp;&nbsp; [\_define\_codeblock\_tag](#_define_codeblock_tag) &nbsp;&nbsp; [\_define\_emphasis\_tags](#_define_emphasis_tags) &nbsp;&nbsp; [\_define\_gap\_tag](#_define_gap_tag) &nbsp;&nbsp; [\_define\_headings\_tags](#_define_headings_tags) &nbsp;&nbsp; [\_define\_hidden\_tag](#_define_hidden_tag) &nbsp;&nbsp; [\_define\_highlighting\_tags](#_define_highlighting_tags) &nbsp;&nbsp; [\_define\_link\_tags](#_define_link_tags) &nbsp;&nbsp; [\_define\_tags](#_define_tags) &nbsp;&nbsp; [\_finalize\_rendering](#_finalize_rendering) &nbsp;&nbsp; [\_get\_section\_end](#_get_section_end) &nbsp;&nbsp; [\_look](#_look) &nbsp;&nbsp; [\_look\_part\_1](#_look_part_1) &nbsp;&nbsp; [\_look\_part\_2](#_look_part_2) &nbsp;&nbsp; [\_on\_key\_down](#_on_key_down) &nbsp;&nbsp; [\_on\_key\_left](#_on_key_left) &nbsp;&nbsp; [\_on\_key\_right](#_on_key_right) &nbsp;&nbsp; [\_on\_key\_up](#_on_key_up) &nbsp;&nbsp; [\_on\_mouse\_wheel](#_on_mouse_wheel) &nbsp;&nbsp; [\_render](#_render) &nbsp;&nbsp; [\_set\_editor\_config](#_set_editor_config) &nbsp;&nbsp; [\_setup](#_setup) &nbsp;&nbsp; [\_update\_style](#_update_style)

## \_\_init\_\_
Initialize self.  See help(type(self)) for accurate signature.



**Signature:** (self, editor, dossier=None, style=<exonote.style.Style object at 0x7fcd16b26940>, inserter=<class 'exonote.inserter.Inserter'>, scroll\_step=25, restriction=0, statusbar=<class 'exonote.statusbar.DefaultStatusBar'>, on\_open=None, on\_press\_left=None, on\_press\_right=None, on\_press\_up=None, on\_press\_down=None, update\_sys\_path=True)





**Return Value:** None

[Back to Top](#module-overview)


## clear
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## clear\_section
No description



**Signature:** (self, sid)





**Return Value:** None

[Back to Top](#module-overview)


## compute\_index
Example: char_spec='+1' or '-1' or '=1' or None 



**Signature:** (self, index, line\_spec=None, char\_spec=None)





**Return Value:** None

[Back to Top](#module-overview)


## del\_heading
No description



**Signature:** (self, sid)





**Return Value:** None

[Back to Top](#module-overview)


## del\_section
No description



**Signature:** (self, sid)





**Return Value:** None

[Back to Top](#module-overview)


## disable\_edit\_mode
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## edit\_heading
No description



**Signature:** (self, sid, text)





**Return Value:** None

[Back to Top](#module-overview)


## edit\_section
No description



**Signature:** (self, sid, source)





**Return Value:** None

[Back to Top](#module-overview)


## enable\_edit\_mode
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## extend\_section
Position is either top or bottom 



**Signature:** (self, sid, source, side='bottom')





**Return Value:** None

[Back to Top](#module-overview)


## get\_heading
No description



**Signature:** (self, sid, include\_text=False)





**Return Value:** None

[Back to Top](#module-overview)


## get\_index
No description



**Signature:** (self, anchor)





**Return Value:** None

[Back to Top](#module-overview)


## get\_section
return a tuple (heading, body)



**Signature:** (self, sid, include\_text=False)





**Return Value:** None

[Back to Top](#module-overview)


## goto
No description



**Signature:** (self, index)





**Return Value:** None

[Back to Top](#module-overview)


## look\_ahead
the argument 'levels' is either an integer or None.
Examples:
     levels=None (look for sids without caring about their levels)
     levels=">" (look for sids with levels > to the reference sid)
     levels="<" (look for sids with levels < to the reference sid)
     levels="=" (look for sids with levels = to the reference sid)
     levels="=3" (look for sids with levels = to 3)
     levels="<=3" (look for sids with levels <= to 3)



**Signature:** (self, sid, level\_spec=None, maxcount=None)





**Return Value:** None

[Back to Top](#module-overview)


## look\_behind
the argument 'levels' is either a string or None.
Examples:
     levels=None (look for sids without caring about their levels)
     levels=">" (look for sids with levels > to the reference sid)
     levels="<" (look for sids with levels < to the reference sid)
     levels="=" (look for sids with levels < to the reference sid)
     levels="=3" (look for sids with levels = to 3)
     levels="<=3" (look for sids with levels <= to 3)



**Signature:** (self, sid, level\_spec=None, maxcount=None)





**Return Value:** None

[Back to Top](#module-overview)


## make\_scrollable
No description



**Signature:** (self, widget)





**Return Value:** None

[Back to Top](#module-overview)


## next\_id
Generate ID ! Generate and return a unique identifier (int)



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## open
target shouldn't be an absolute filesystem path but relative to the dossier



**Signature:** (self, target)





**Return Value:** None

[Back to Top](#module-overview)


## read\_heading
No description



**Signature:** (self, sid)





**Return Value:** None

[Back to Top](#module-overview)


## read\_section
No description



**Signature:** (self, sid)





**Return Value:** None

[Back to Top](#module-overview)


## refresh
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## register\_anchor
No description



**Signature:** (self, name, index)





**Return Value:** None

[Back to Top](#module-overview)


## register\_section
No description



**Signature:** (self, sid, index, level, tags)





**Return Value:** None

[Back to Top](#module-overview)


## render
Render and insert the source at a specific index inside the viewer widget
source = text or structure returned by parser



**Signature:** (self, source, index='insert')





**Return Value:** None

[Back to Top](#module-overview)


## \_bind\_handlers\_to\_tags
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_compute\_single\_index
No description



**Signature:** (self, index, spec)





**Return Value:** None

[Back to Top](#module-overview)


## \_create\_top\_bottom\_anchors
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_define\_alignment\_tags
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_define\_caption\_tag
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_define\_centered\_component\_tags
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_define\_codeblock\_tag
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_define\_emphasis\_tags
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_define\_gap\_tag
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_define\_headings\_tags
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_define\_hidden\_tag
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_define\_highlighting\_tags
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_define\_link\_tags
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_define\_tags
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_finalize\_rendering
No description



**Signature:** (self, cache)





**Return Value:** None

[Back to Top](#module-overview)


## \_get\_section\_end
No description



**Signature:** (self, sid)





**Return Value:** None

[Back to Top](#module-overview)


## \_look
No description



**Signature:** (self, sid, level\_spec, maxcount, backward=False)





**Return Value:** None

[Back to Top](#module-overview)


## \_look\_part\_1
No description



**Signature:** (self, sid, level\_spec, backward)





**Return Value:** None

[Back to Top](#module-overview)


## \_look\_part\_2
No description



**Signature:** (self, sid, sids, comparison, comparison\_target, maxcount)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_key\_down
No description



**Signature:** (self, event)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_key\_left
No description



**Signature:** (self, event)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_key\_right
No description



**Signature:** (self, event)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_key\_up
No description



**Signature:** (self, event)





**Return Value:** None

[Back to Top](#module-overview)


## \_on\_mouse\_wheel
No description



**Signature:** (self, event)





**Return Value:** None

[Back to Top](#module-overview)


## \_render
No description



**Signature:** (self, structure, index)





**Return Value:** None

[Back to Top](#module-overview)


## \_set\_editor\_config
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_setup
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)


## \_update\_style
No description



**Signature:** (self)





**Return Value:** None

[Back to Top](#module-overview)



