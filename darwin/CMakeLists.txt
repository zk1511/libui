# 3 june 2016

list(APPEND _LIBUI_SOURCES
	darwin/aat.m
	darwin/alloc.m
	darwin/area.m
	darwin/areaevents.m
	darwin/attrstr.m
	darwin/autolayout.m
	darwin/box.m
	darwin/button.m
	darwin/checkbox.m
	darwin/colorbutton.m
	darwin/combobox.m
	darwin/control.m
	darwin/datetimepicker.m
	darwin/debug.m
	darwin/draw.m
	darwin/drawtext.m
	darwin/editablecombo.m
	darwin/entry.m
	darwin/fontbutton.m
	darwin/fontmatch.m
	darwin/fonttraits.m
	darwin/fontvariation.m
	darwin/form.m
	darwin/future.m
	darwin/graphemes.m
	darwin/grid.m
	darwin/group.m
	darwin/image.m
	darwin/label.m
	darwin/main.m
	darwin/map.m
	darwin/menu.m
	darwin/multilineentry.m
	darwin/opentype.m
	darwin/progressbar.m
	darwin/radiobuttons.m
	darwin/scrollview.m
	darwin/separator.m
	darwin/slider.m
	darwin/spinbox.m
	darwin/stddialogs.m
	darwin/tab.m
	darwin/text.m
	darwin/undocumented.m
	darwin/util.m
	darwin/window.m
	darwin/winmoveresize.m
)
set(_LIBUI_SOURCES ${_LIBUI_SOURCES} PARENT_SCOPE)

# TODO is this correct?
list(APPEND _LIBUI_INCLUDEDIRS
	darwin
)
set(_LIBUI_INCLUDEDIRS _LIBUI_INCLUDEDIRS PARENT_SCOPE)

set(_LIBUI_LIBS
	objc "-framework Foundation" "-framework AppKit"
PARENT_SCOPE)
