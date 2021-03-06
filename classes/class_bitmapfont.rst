.. Generated automatically by doc/tools/makerst.py in Godot's source tree.
.. DO NOT EDIT THIS FILE, but the BitmapFont.xml source instead.
.. The source is found in doc/classes or modules/<name>/doc_classes.

.. _class_BitmapFont:

BitmapFont
==========

**Inherits:** :ref:`Font<class_font>` **<** :ref:`Resource<class_resource>` **<** :ref:`Reference<class_reference>` **<** :ref:`Object<class_object>`

**Category:** Core

Brief Description
-----------------

Renders text using ``\*.fnt`` fonts.

Member Functions
----------------

+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                 | :ref:`add_char<class_BitmapFont_add_char>` **(** :ref:`int<class_int>` character, :ref:`int<class_int>` texture, :ref:`Rect2<class_rect2>` rect, :ref:`Vector2<class_vector2>` align=Vector2( 0, 0 ), :ref:`float<class_float>` advance=-1 **)** |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                 | :ref:`add_kerning_pair<class_BitmapFont_add_kerning_pair>` **(** :ref:`int<class_int>` char_a, :ref:`int<class_int>` char_b, :ref:`int<class_int>` kerning **)**                                                                                 |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                 | :ref:`add_texture<class_BitmapFont_add_texture>` **(** :ref:`Texture<class_texture>` texture **)**                                                                                                                                               |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                 | :ref:`clear<class_BitmapFont_clear>` **(** **)**                                                                                                                                                                                                 |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                | :ref:`create_from_fnt<class_BitmapFont_create_from_fnt>` **(** :ref:`String<class_string>` path **)**                                                                                                                                            |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Vector2<class_vector2>`        | :ref:`get_char_size<class_BitmapFont_get_char_size>` **(** :ref:`int<class_int>` char, :ref:`int<class_int>` next=0 **)** const                                                                                                                  |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`BitmapFont<class_bitmapfont>`  | :ref:`get_fallback<class_BitmapFont_get_fallback>` **(** **)** const                                                                                                                                                                             |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                | :ref:`get_kerning_pair<class_BitmapFont_get_kerning_pair>` **(** :ref:`int<class_int>` char_a, :ref:`int<class_int>` char_b **)** const                                                                                                          |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`Texture<class_texture>`        | :ref:`get_texture<class_BitmapFont_get_texture>` **(** :ref:`int<class_int>` idx **)** const                                                                                                                                                     |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| :ref:`int<class_int>`                | :ref:`get_texture_count<class_BitmapFont_get_texture_count>` **(** **)** const                                                                                                                                                                   |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                 | :ref:`set_ascent<class_BitmapFont_set_ascent>` **(** :ref:`float<class_float>` px **)**                                                                                                                                                          |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                 | :ref:`set_distance_field_hint<class_BitmapFont_set_distance_field_hint>` **(** :ref:`bool<class_bool>` enable **)**                                                                                                                              |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                 | :ref:`set_fallback<class_BitmapFont_set_fallback>` **(** :ref:`BitmapFont<class_bitmapfont>` fallback **)**                                                                                                                                      |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+
| void                                 | :ref:`set_height<class_BitmapFont_set_height>` **(** :ref:`float<class_float>` px **)**                                                                                                                                                          |
+--------------------------------------+--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------+

Member Variables
----------------

  .. _class_BitmapFont_ascent:

- :ref:`float<class_float>` **ascent** - Ascent (number of pixels above the baseline).

  .. _class_BitmapFont_chars:

- :ref:`PoolIntArray<class_poolintarray>` **chars** - The characters in the BitmapFont.

  .. _class_BitmapFont_distance_field:

- :ref:`bool<class_bool>` **distance_field** - If ``true`` distance field hint is enabled.

  .. _class_BitmapFont_fallback:

- :ref:`BitmapFont<class_bitmapfont>` **fallback** - The fallback font.

  .. _class_BitmapFont_height:

- :ref:`float<class_float>` **height** - Total font height (ascent plus descent) in pixels.

  .. _class_BitmapFont_kernings:

- :ref:`PoolIntArray<class_poolintarray>` **kernings** - The font's kernings as :ref:`PoolIntArray<class_poolintarray>`.

  .. _class_BitmapFont_textures:

- :ref:`Array<class_array>` **textures** - The font's :ref:`Texture<class_texture>`\ s.


Description
-----------

Renders text using ``\*.fnt`` fonts containing texture atlases. Supports distance fields. For using vector font files like TTF directly, see :ref:`DynamicFont<class_dynamicfont>`.

Member Function Description
---------------------------

.. _class_BitmapFont_add_char:

- void **add_char** **(** :ref:`int<class_int>` character, :ref:`int<class_int>` texture, :ref:`Rect2<class_rect2>` rect, :ref:`Vector2<class_vector2>` align=Vector2( 0, 0 ), :ref:`float<class_float>` advance=-1 **)**

Adds a character to the font, where ``character`` is the unicode value, ``texture`` is the texture index, ``rect`` is the region in the texture (in pixels!), ``align`` is the (optional) alignment for the character and ``advance`` is the (optional) advance.

.. _class_BitmapFont_add_kerning_pair:

- void **add_kerning_pair** **(** :ref:`int<class_int>` char_a, :ref:`int<class_int>` char_b, :ref:`int<class_int>` kerning **)**

Adds a kerning pair to the ``BitmapFont`` as a difference. Kerning pairs are special cases where a typeface advance is determined by the next character.

.. _class_BitmapFont_add_texture:

- void **add_texture** **(** :ref:`Texture<class_texture>` texture **)**

Adds a texture to the ``BitmapFont``.

.. _class_BitmapFont_clear:

- void **clear** **(** **)**

Clears all the font data and settings.

.. _class_BitmapFont_create_from_fnt:

- :ref:`int<class_int>` **create_from_fnt** **(** :ref:`String<class_string>` path **)**

Creates a BitmapFont from the ``\*.fnt`` file at ``path``.

.. _class_BitmapFont_get_char_size:

- :ref:`Vector2<class_vector2>` **get_char_size** **(** :ref:`int<class_int>` char, :ref:`int<class_int>` next=0 **)** const

Returns the size of a character, optionally taking kerning into account if the next character is provided.

.. _class_BitmapFont_get_fallback:

- :ref:`BitmapFont<class_bitmapfont>` **get_fallback** **(** **)** const

Returns the fallback BitmapFont.

.. _class_BitmapFont_get_kerning_pair:

- :ref:`int<class_int>` **get_kerning_pair** **(** :ref:`int<class_int>` char_a, :ref:`int<class_int>` char_b **)** const

Returns a kerning pair as a difference.

.. _class_BitmapFont_get_texture:

- :ref:`Texture<class_texture>` **get_texture** **(** :ref:`int<class_int>` idx **)** const

Returns the font atlas texture at index ``idx``.

.. _class_BitmapFont_get_texture_count:

- :ref:`int<class_int>` **get_texture_count** **(** **)** const

Returns the number of textures in the BitmapFont atlas.

.. _class_BitmapFont_set_ascent:

- void **set_ascent** **(** :ref:`float<class_float>` px **)**

Sets the font ascent (number of pixels above the baseline).

.. _class_BitmapFont_set_distance_field_hint:

- void **set_distance_field_hint** **(** :ref:`bool<class_bool>` enable **)**

If ``true`` distance field hint is enabled.

.. _class_BitmapFont_set_fallback:

- void **set_fallback** **(** :ref:`BitmapFont<class_bitmapfont>` fallback **)**

Sets the fallback BitmapFont.

.. _class_BitmapFont_set_height:

- void **set_height** **(** :ref:`float<class_float>` px **)**

Sets the total font height (ascent plus descent) in pixels.


