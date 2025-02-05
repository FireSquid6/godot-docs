:github_url: hide

.. Generated automatically by doc/tools/make_rst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the Line2D.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_Line2D:

Line2D
======

**Inherits:** :ref:`Node2D<class_Node2D>` **<** :ref:`CanvasItem<class_CanvasItem>` **<** :ref:`Node<class_Node>` **<** :ref:`Object<class_Object>`

A 2D line.

Description
-----------

A line through several points in 2D space.

Tutorials
---------

- `Matrix Transform Demo <https://godotengine.org/asset-library/asset/584>`__

- `2.5D Demo <https://godotengine.org/asset-library/asset/583>`__

Properties
----------

+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`bool<class_bool>`                             | :ref:`antialiased<class_Line2D_property_antialiased>`         | ``false``                |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`LineCapMode<enum_Line2D_LineCapMode>`         | :ref:`begin_cap_mode<class_Line2D_property_begin_cap_mode>`   | ``0``                    |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`Color<class_Color>`                           | :ref:`default_color<class_Line2D_property_default_color>`     | ``Color(1, 1, 1, 1)``    |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`LineCapMode<enum_Line2D_LineCapMode>`         | :ref:`end_cap_mode<class_Line2D_property_end_cap_mode>`       | ``0``                    |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`Gradient<class_Gradient>`                     | :ref:`gradient<class_Line2D_property_gradient>`               |                          |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`LineJointMode<enum_Line2D_LineJointMode>`     | :ref:`joint_mode<class_Line2D_property_joint_mode>`           | ``0``                    |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`PackedVector2Array<class_PackedVector2Array>` | :ref:`points<class_Line2D_property_points>`                   | ``PackedVector2Array()`` |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`int<class_int>`                               | :ref:`round_precision<class_Line2D_property_round_precision>` | ``8``                    |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`float<class_float>`                           | :ref:`sharp_limit<class_Line2D_property_sharp_limit>`         | ``2.0``                  |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`Texture2D<class_Texture2D>`                   | :ref:`texture<class_Line2D_property_texture>`                 |                          |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`LineTextureMode<enum_Line2D_LineTextureMode>` | :ref:`texture_mode<class_Line2D_property_texture_mode>`       | ``0``                    |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`float<class_float>`                           | :ref:`width<class_Line2D_property_width>`                     | ``10.0``                 |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+
| :ref:`Curve<class_Curve>`                           | :ref:`width_curve<class_Line2D_property_width_curve>`         |                          |
+-----------------------------------------------------+---------------------------------------------------------------+--------------------------+

Methods
-------

+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`add_point<class_Line2D_method_add_point>` **(** :ref:`Vector2<class_Vector2>` position, :ref:`int<class_int>` at_position=-1 **)**      |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`clear_points<class_Line2D_method_clear_points>` **(** **)**                                                                             |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`         | :ref:`get_point_count<class_Line2D_method_get_point_count>` **(** **)** |const|                                                               |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_Vector2>` | :ref:`get_point_position<class_Line2D_method_get_point_position>` **(** :ref:`int<class_int>` i **)** |const|                                 |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`remove_point<class_Line2D_method_remove_point>` **(** :ref:`int<class_int>` i **)**                                                     |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+
| void                          | :ref:`set_point_position<class_Line2D_method_set_point_position>` **(** :ref:`int<class_int>` i, :ref:`Vector2<class_Vector2>` position **)** |
+-------------------------------+-----------------------------------------------------------------------------------------------------------------------------------------------+

Enumerations
------------

.. _enum_Line2D_LineJointMode:

.. _class_Line2D_constant_LINE_JOINT_SHARP:

.. _class_Line2D_constant_LINE_JOINT_BEVEL:

.. _class_Line2D_constant_LINE_JOINT_ROUND:

enum **LineJointMode**:

- **LINE_JOINT_SHARP** = **0** --- The line's joints will be pointy. If ``sharp_limit`` is greater than the rotation of a joint, it becomes a bevel joint instead.

- **LINE_JOINT_BEVEL** = **1** --- The line's joints will be bevelled/chamfered.

- **LINE_JOINT_ROUND** = **2** --- The line's joints will be rounded.

----

.. _enum_Line2D_LineCapMode:

.. _class_Line2D_constant_LINE_CAP_NONE:

.. _class_Line2D_constant_LINE_CAP_BOX:

.. _class_Line2D_constant_LINE_CAP_ROUND:

enum **LineCapMode**:

- **LINE_CAP_NONE** = **0** --- Don't draw a line cap.

- **LINE_CAP_BOX** = **1** --- Draws the line cap as a box.

- **LINE_CAP_ROUND** = **2** --- Draws the line cap as a circle.

----

.. _enum_Line2D_LineTextureMode:

.. _class_Line2D_constant_LINE_TEXTURE_NONE:

.. _class_Line2D_constant_LINE_TEXTURE_TILE:

.. _class_Line2D_constant_LINE_TEXTURE_STRETCH:

enum **LineTextureMode**:

- **LINE_TEXTURE_NONE** = **0** --- Takes the left pixels of the texture and renders it over the whole line.

- **LINE_TEXTURE_TILE** = **1** --- Tiles the texture over the line. :ref:`CanvasItem.texture_repeat<class_CanvasItem_property_texture_repeat>` of the ``Line2D`` node must be :ref:`CanvasItem.TEXTURE_REPEAT_ENABLED<class_CanvasItem_constant_TEXTURE_REPEAT_ENABLED>` or :ref:`CanvasItem.TEXTURE_REPEAT_MIRROR<class_CanvasItem_constant_TEXTURE_REPEAT_MIRROR>` for it to work properly.

- **LINE_TEXTURE_STRETCH** = **2** --- Stretches the texture across the line. :ref:`CanvasItem.texture_repeat<class_CanvasItem_property_texture_repeat>` of the ``Line2D`` node must be :ref:`CanvasItem.TEXTURE_REPEAT_DISABLED<class_CanvasItem_constant_TEXTURE_REPEAT_DISABLED>` for best results.

Property Descriptions
---------------------

.. _class_Line2D_property_antialiased:

- :ref:`bool<class_bool>` **antialiased**

+-----------+------------------------+
| *Default* | ``false``              |
+-----------+------------------------+
| *Setter*  | set_antialiased(value) |
+-----------+------------------------+
| *Getter*  | get_antialiased()      |
+-----------+------------------------+

If ``true``, the line's border will be anti-aliased.

\ **Note:** Line2D is not accelerated by batching when being anti-aliased.

----

.. _class_Line2D_property_begin_cap_mode:

- :ref:`LineCapMode<enum_Line2D_LineCapMode>` **begin_cap_mode**

+-----------+---------------------------+
| *Default* | ``0``                     |
+-----------+---------------------------+
| *Setter*  | set_begin_cap_mode(value) |
+-----------+---------------------------+
| *Getter*  | get_begin_cap_mode()      |
+-----------+---------------------------+

Controls the style of the line's first point. Use :ref:`LineCapMode<enum_Line2D_LineCapMode>` constants.

----

.. _class_Line2D_property_default_color:

- :ref:`Color<class_Color>` **default_color**

+-----------+--------------------------+
| *Default* | ``Color(1, 1, 1, 1)``    |
+-----------+--------------------------+
| *Setter*  | set_default_color(value) |
+-----------+--------------------------+
| *Getter*  | get_default_color()      |
+-----------+--------------------------+

The line's color. Will not be used if a gradient is set.

----

.. _class_Line2D_property_end_cap_mode:

- :ref:`LineCapMode<enum_Line2D_LineCapMode>` **end_cap_mode**

+-----------+-------------------------+
| *Default* | ``0``                   |
+-----------+-------------------------+
| *Setter*  | set_end_cap_mode(value) |
+-----------+-------------------------+
| *Getter*  | get_end_cap_mode()      |
+-----------+-------------------------+

Controls the style of the line's last point. Use :ref:`LineCapMode<enum_Line2D_LineCapMode>` constants.

----

.. _class_Line2D_property_gradient:

- :ref:`Gradient<class_Gradient>` **gradient**

+----------+---------------------+
| *Setter* | set_gradient(value) |
+----------+---------------------+
| *Getter* | get_gradient()      |
+----------+---------------------+

The gradient is drawn through the whole line from start to finish. The default color will not be used if a gradient is set.

----

.. _class_Line2D_property_joint_mode:

- :ref:`LineJointMode<enum_Line2D_LineJointMode>` **joint_mode**

+-----------+-----------------------+
| *Default* | ``0``                 |
+-----------+-----------------------+
| *Setter*  | set_joint_mode(value) |
+-----------+-----------------------+
| *Getter*  | get_joint_mode()      |
+-----------+-----------------------+

The style for the points between the start and the end.

----

.. _class_Line2D_property_points:

- :ref:`PackedVector2Array<class_PackedVector2Array>` **points**

+-----------+--------------------------+
| *Default* | ``PackedVector2Array()`` |
+-----------+--------------------------+
| *Setter*  | set_points(value)        |
+-----------+--------------------------+
| *Getter*  | get_points()             |
+-----------+--------------------------+

The points that form the lines. The line is drawn between every point set in this array. Points are interpreted as local vectors.

----

.. _class_Line2D_property_round_precision:

- :ref:`int<class_int>` **round_precision**

+-----------+----------------------------+
| *Default* | ``8``                      |
+-----------+----------------------------+
| *Setter*  | set_round_precision(value) |
+-----------+----------------------------+
| *Getter*  | get_round_precision()      |
+-----------+----------------------------+

The smoothness of the rounded joints and caps. Higher values result in smoother corners, but are more demanding to render and update. This is only used if a cap or joint is set as round.

\ **Note:** The default value is tuned for lines with the default :ref:`width<class_Line2D_property_width>`. For thin lines, this value should be reduced to a number between ``2`` and ``4`` to improve performance.

----

.. _class_Line2D_property_sharp_limit:

- :ref:`float<class_float>` **sharp_limit**

+-----------+------------------------+
| *Default* | ``2.0``                |
+-----------+------------------------+
| *Setter*  | set_sharp_limit(value) |
+-----------+------------------------+
| *Getter*  | get_sharp_limit()      |
+-----------+------------------------+

The direction difference in radians between vector points. This value is only used if :ref:`joint_mode<class_Line2D_property_joint_mode>` is set to :ref:`LINE_JOINT_SHARP<class_Line2D_constant_LINE_JOINT_SHARP>`.

----

.. _class_Line2D_property_texture:

- :ref:`Texture2D<class_Texture2D>` **texture**

+----------+--------------------+
| *Setter* | set_texture(value) |
+----------+--------------------+
| *Getter* | get_texture()      |
+----------+--------------------+

The texture used for the line's texture. Uses ``texture_mode`` for drawing style.

----

.. _class_Line2D_property_texture_mode:

- :ref:`LineTextureMode<enum_Line2D_LineTextureMode>` **texture_mode**

+-----------+-------------------------+
| *Default* | ``0``                   |
+-----------+-------------------------+
| *Setter*  | set_texture_mode(value) |
+-----------+-------------------------+
| *Getter*  | get_texture_mode()      |
+-----------+-------------------------+

The style to render the ``texture`` on the line. Use :ref:`LineTextureMode<enum_Line2D_LineTextureMode>` constants.

----

.. _class_Line2D_property_width:

- :ref:`float<class_float>` **width**

+-----------+------------------+
| *Default* | ``10.0``         |
+-----------+------------------+
| *Setter*  | set_width(value) |
+-----------+------------------+
| *Getter*  | get_width()      |
+-----------+------------------+

The line's width.

----

.. _class_Line2D_property_width_curve:

- :ref:`Curve<class_Curve>` **width_curve**

+----------+------------------+
| *Setter* | set_curve(value) |
+----------+------------------+
| *Getter* | get_curve()      |
+----------+------------------+

The line's width varies with the curve. The original width is simply multiply by the value of the Curve.

Method Descriptions
-------------------

.. _class_Line2D_method_add_point:

- void **add_point** **(** :ref:`Vector2<class_Vector2>` position, :ref:`int<class_int>` at_position=-1 **)**

Adds a point at the ``position``. Appends the point at the end of the line.

If ``at_position`` is given, the point is inserted before the point number ``at_position``, moving that point (and every point after) after the inserted point. If ``at_position`` is not given, or is an illegal value (``at_position < 0`` or ``at_position >= [method get_point_count]``), the point will be appended at the end of the point list.

----

.. _class_Line2D_method_clear_points:

- void **clear_points** **(** **)**

Removes all points from the line.

----

.. _class_Line2D_method_get_point_count:

- :ref:`int<class_int>` **get_point_count** **(** **)** |const|

Returns the Line2D's amount of points.

----

.. _class_Line2D_method_get_point_position:

- :ref:`Vector2<class_Vector2>` **get_point_position** **(** :ref:`int<class_int>` i **)** |const|

Returns point ``i``'s position.

----

.. _class_Line2D_method_remove_point:

- void **remove_point** **(** :ref:`int<class_int>` i **)**

Removes the point at index ``i`` from the line.

----

.. _class_Line2D_method_set_point_position:

- void **set_point_position** **(** :ref:`int<class_int>` i, :ref:`Vector2<class_Vector2>` position **)**

Overwrites the position in point ``i`` with the supplied ``position``.

.. |virtual| replace:: :abbr:`virtual (This method should typically be overridden by the user to have any effect.)`
.. |const| replace:: :abbr:`const (This method has no side effects. It doesn't modify any of the instance's member variables.)`
.. |vararg| replace:: :abbr:`vararg (This method accepts any number of arguments after the ones described here.)`
.. |constructor| replace:: :abbr:`constructor (This method is used to construct a type.)`
.. |static| replace:: :abbr:`static (This method doesn't need an instance to be called, so it can be called directly using the class name.)`
.. |operator| replace:: :abbr:`operator (This method describes a valid operator to use with this type as left-hand operand.)`
