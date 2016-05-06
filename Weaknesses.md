# Profiler #

  * It does not calibrate or try to exclude its own overhead from the timings. This may make some timings less accurate.
  * It is somewhat slower than cProfile (it does more, though. Gives more meaningful output about User/System/Real time of each function).

# Viewer #

  * Gtk's TreeView "blocks" for long periods of time when the underlying tree is huge. While great care was taken to allow immediate actions even for really huge trees, Gtk+ makes it very difficult to always read sections of the large tree on demand, or at least not block the entire GUI when its waiting.
  * The few browsing features it has are associated with undocumented key bindings.