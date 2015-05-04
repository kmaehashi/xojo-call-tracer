Call Tracer for Xojo
============================

This is a tiny hack to automatically insert code that prints its name for every method and event call.

How To Use
----------------

1. Open the Xojo binary (``Xojo.app/Contents/MacOS/Xojo``) with a binary editor and replace ``const CurrentMethodName = "`` with ``#if CALL_TRACE Then Trace "``.  Make sure to take a backup before doing this!
2. Add the CallTracer folder to your project.
3. Just build and run.
   Now method and event calls are automatically printed to the system log.

Downsides
----------------

* Execution speed slows down significantly.
* ``CurrentMethodName`` constant becomes unavailable.
