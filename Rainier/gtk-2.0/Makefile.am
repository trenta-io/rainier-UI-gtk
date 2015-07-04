enginedir = $(libdir)/gtk-2.0/$(GTK2_VERSION)/engines
engine_LTLIBRARIES = libadwaita.la

libadwaita_la_CFLAGS = $(GTK2_ENGINE_CFLAGS)
libadwaita_la_SOURCES = adwaita_engine.c
libadwaita_la_LDFLAGS = -module -avoid-version -no-undefined
libadwaita_la_LIBADD =  $(GTK2_ENGINE_LIBS)

themedir = $(datadir)/themes/Adwaita/gtk-2.0
theme_DATA = gtkrc

asset_dirs = "Arrows" "Buttons" "Check-Radio" "Entry" "Expanders" \
	"Handles" "Lines" "Menu-Menubar" "Others" "ProgressBar" \
	"Range" "Scrollbars" "Shadows" "Spin" "Tabs" "Toolbar"
asset_data = \
	Arrows/arrow-down.png \
	Arrows/arrow-down-insens.png \
	Arrows/arrow-down-prelight.png \
	Arrows/arrow-down-small.png \
	Arrows/arrow-down-small-insens.png \
	Arrows/arrow-down-small-prelight.png \
	Arrows/arrow-left.png \
	Arrows/arrow-left-insens.png \
	Arrows/arrow-left-prelight.png \
	Arrows/arrow-right.png \
	Arrows/arrow-right-insens.png \
	Arrows/arrow-right-prelight.png \
	Arrows/arrow-up.png \
	Arrows/arrow-up-insens.png \
	Arrows/arrow-up-prelight.png \
	Arrows/arrow-up-small.png \
	Arrows/arrow-up-small-insens.png \
	Arrows/arrow-up-small-prelight.png \
	Arrows/menu-arrow.png \
	Arrows/menu-arrow-prelight.png \
	Buttons/button-default.png \
	Buttons/button-insensitive.png \
	Buttons/button-prelight.png \
	Buttons/button-pressed.png \
	Buttons/button-default-nohilight.png \
	Buttons/button-insensitive-nohilight.png \
	Buttons/button-prelight-nohilight.png \
	Buttons/button-pressed-nohilight.png \
	Check-Radio/checkbox-checked.png \
	Check-Radio/checkbox-unchecked.png \
	Check-Radio/checkbox-checked-insensitive.png \
	Check-Radio/checkbox-unchecked-insensitive.png \
	Check-Radio/menucheck.png \
	Check-Radio/menucheck_prelight.png \
	Check-Radio/menuoption.png \
	Check-Radio/menuoption_prelight.png \
	Check-Radio/option-checked.png \
	Check-Radio/option-unchecked.png \
	Check-Radio/option-checked-insensitive.png \
	Check-Radio/option-unchecked-insensitive.png \
	Entry/combo-entry-border-bg.png \
	Entry/combo-entry-border-rtl-bg.png \
	Entry/combo-entry-border-active-bg.png \
	Entry/combo-entry-border-active-rtl-bg.png \
	Entry/combo-entry-border-disabled-bg.png \
	Entry/combo-entry-border-disabled-rtl-bg.png \
	Entry/combo-entry-border-notebook.png \
	Entry/combo-entry-border-rtl-notebook.png \
	Entry/combo-entry-border-active-notebook.png \
	Entry/combo-entry-border-active-rtl-notebook.png \
	Entry/combo-entry-border-disabled-notebook.png \
	Entry/combo-entry-border-disabled-rtl-notebook.png \
	Entry/combo-entry-button.png \
	Entry/combo-entry-button-rtl.png \
	Entry/combo-entry-button-active.png \
	Entry/combo-entry-button-active-rtl.png \
	Entry/combo-entry-button-disabled.png \
	Entry/combo-entry-button-disabled-rtl.png \
	Entry/entry-border-fill.png \
	Entry/entry-border-fill-plain.png \
	Entry/entry-border-fill-solid.png \
	Entry/entry-border-bg.png \
	Entry/entry-border-active-bg.png \
	Entry/entry-border-bg-solid.png \
	Entry/entry-border-active-bg-solid.png \
	Entry/entry-border-disabled-bg.png \
	Entry/entry-border-notebook.png \
	Entry/entry-border-active-notebook.png \
	Entry/entry-border-disabled-notebook.png \
	Expanders/minus.png \
	Expanders/plus.png \
	Handles/handle-h.png \
	Handles/handle-v.png \
	Lines/line-h.png \
	Lines/line-v.png \
	Lines/menu_line_h.png \
	Menu-Menubar/menubar_button.png \
	Menu-Menubar/menubar.png \
	Others/focus.png \
	Others/null.png \
	Others/tree_header.png \
	ProgressBar/progressbar.png \
	ProgressBar/progressbar_v.png \
	ProgressBar/trough-progressbar.png \
	ProgressBar/trough-progressbar_v.png \
	Range/slider-horiz.png \
	Range/slider-horiz-prelight.png \
	Range/slider-vert.png \
	Range/slider-vert-prelight.png \
	Range/trough-horizontal.png \
	Range/trough-vertical.png \
	Scrollbars/slider-horiz-active.png \
	Scrollbars/slider-horiz.png \
	Scrollbars/slider-vert-active.png \
        Scrollbars/slider-vert.png \
	Scrollbars/slider-horiz-insens.png \
	Scrollbars/slider-horiz-prelight.png \
	Scrollbars/slider-vert-insens.png \
	Scrollbars/slider-vert-prelight.png \
        Scrollbars/trough-scrollbar-horiz.png \
	Scrollbars/trough-scrollbar-vert.png \
	Shadows/frame.png \
	Shadows/frame-gap-start.png \
	Shadows/frame-gap-end.png \
	Spin/down-background.png \
	Spin/up-background.png \
	Spin/down-background-disable.png \
	Spin/up-background-disable.png \
	Spin/down-background-rtl.png \
	Spin/up-background-rtl.png \
	Spin/down-background-disable-rtl.png \
	Spin/up-background-disable-rtl.png \
	Tabs/notebook-gap-horiz.png \
	Tabs/notebook-gap-vert.png \
	Tabs/notebook.png \
	Tabs/tab-bottom.png \
	Tabs/tab-left.png \
	Tabs/tab-right.png \
	Tabs/tab-top.png \
	Tabs/tab-bottom-active.png \
	Tabs/tab-left-active.png \
	Tabs/tab-right-active.png \
	Tabs/tab-top-active.png \
	Toolbar/inline-toolbar.png

install-data-local:
	for dir in $(asset_dirs); do \
		for file in `cd $(srcdir)/$$dir && find . -maxdepth 1 \( -name "*.png" \)`; do \
			$(mkdir_p) $(DESTDIR)$(datadir)/themes/Adwaita/gtk-2.0/$$dir; \
			$(install_sh_DATA) $(srcdir)/$$dir/$$file $(DESTDIR)$(themedir)/$$dir/$$file; \
		done; \
	done

uninstall-local:
	for dir in $(asset_dirs); do \
		for file in `cd $(srcdir)/$$dir && find . -maxdepth 1 \( -name "*.png" \)`; do \
			rm -f $(DESTDIR)$(datadir)/themes/Adwaita/gtk-2.0/$$dir/$$file; \
		done; \
	done

EXTRA_DIST = $(theme_DATA) $(asset_data)
