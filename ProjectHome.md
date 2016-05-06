Lets you see your Python program's execution as a tree of function invocations, each tree node exposing the real time, and CPU time (user/sys) of that call.

This project consists of two main components:
A Python tracer that can run your Python programs (much like "cProfile" and friends).
A Gtk+ based GUI that can show the trace results.

It uses a tiny auxiliary library written for it "graphfile" to allow append-only writing and reading static DAG's directly from file without reading it whole into memory at any stage.