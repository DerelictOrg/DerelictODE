DerelictODE
===========

A dynamic binding to version 0.13.1 of the [Open Dynamics Engine][1] physics library for the D Programming Language.

Please see the pages [Building and Linking Derelict][2] and [Using Derelict][3], in the Derelict documentation, for information on how to build DerelictODE and load the ODE libraries at run time. In the meantime, here's some sample code.

```D
import derelict.ode.ode;

void main() {
    // Load the ODE library.
    DerelictODE.load();

    // Now ODE functions can be called.
    ...
}
```

NOTE: Because of a bug in the ODE API, dPrintMatrix is not properly exported from the shared library. As such, it is disabled in this version of DerelictODE. It is fixed in the ODE repository and will be available in a future release of DerelictODE.

dInfiniteAABB is also disabled in this version of DerelictODE, as it is not exported in the ODE 13.1 shared library.

By default, DerelictODE is configured to load the double-precision version of ODE. If you want to load the single-precision version, declare "DerelictODE_Single" as a version in the build settings of your dub.json.

[1]: https://bitbucket.org/odedevs/ode
[2]: http://derelictorg.github.io/compiling.html
[3]: http://derelictorg.github.io/using.html