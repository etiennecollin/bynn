---
layout: default
title: LabelMe Configuration File Example
parent: Support
---

# LabelME Configuration File Example

This is how our `~/.labelmerc` file was setup to label the images for the mitosis neural network.
If you want, you may replace the content of your own `~./labelmerc` with the following code:

```
auto_save: true
display_label_popup: true
store_data: false
keep_prev: true
keep_prev_scale: false
keep_prev_brightness: false
keep_prev_contrast: false
logger_level: info

flags: null
label_flags: null
labels: null
file_search: null
sort_labels: true
validate_label: exact

default_shape_color: [0, 255, 0]
shape_color: auto # null, 'auto', 'manual'
shift_auto_shape_color: 0
label_colors: null

shape:

# drawing

line_color: [0, 255, 0, 128]
fill_color: [0, 255, 0, 0] # transparent
vertex_fill_color: [0, 255, 0, 255]

# selecting / hovering

select_line_color: [255, 255, 255, 255]
select_fill_color: [0, 255, 0, 155]
hvertex_fill_color: [255, 255, 255, 255]
point_size: 8

# main

flag_dock:
show: true
closable: true
movable: true
floatable: true
label_dock:
show: true
closable: true
movable: true
floatable: true
shape_dock:
show: true
closable: true
movable: true
floatable: true
file_dock:
show: true
closable: true
movable: true
floatable: true

# label_dialog

show_label_text_field: true
label_completion: startswith
fit_to_content:
column: true
row: false

# canvas

epsilon: 10.0
canvas:

# None: do nothing

# close: close polygon

double_click: close

# The max number of edits we can undo

num_backups: 25

shortcuts:
close: Ctrl+W
open: Ctrl+O
open_dir: Ctrl+U
quit: Ctrl+Q
save: Ctrl+S
save_as: Ctrl+Shift+S
save_to: null
delete_file: Ctrl+Delete

open_next: [D, Ctrl+Shift+D]
open_prev: [A, Ctrl+Shift+A]

zoom_in: [Ctrl+Shift+=, Ctrl+=]
zoom_out: [Ctrl+Shift+-, Ctrl+-]
zoom_to_original: Ctrl+0
fit_window: Ctrl+F
fit_width: Ctrl+Shift+F

create_polygon: Ctrl+N
create_rectangle: W
create_circle: Q
create_line: null
create_point: null
create_linestrip: null
edit_polygon: E
delete_polygon: [Delete, Backspace]
duplicate_polygon: Ctrl+D
copy_polygon: Ctrl+C
paste_polygon: Ctrl+V
undo: Ctrl+Z
undo_last_point: Ctrl+Z
add_point_to_edge: Ctrl+Shift+P
edit_label: Ctrl+E
toggle_keep_prev_mode: Ctrl+P
remove_selected_point: [Meta+H, Shift+Backspace]
```