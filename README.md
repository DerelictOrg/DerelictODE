DerelictODE
===========

A dynamic binding to version 0.13 of the [Open Dynamics Engine][1] physics library for the D Programming Language.

For information on how to build DerelictODE and link it with your programs, please see the post [Using Derelict][2] at The One With D.

For information on how to load the ODE library via DerelictDE see the page [DerelictUtil for Users][3] at the DerelictUtil Wiki. In the meantime, here's some sample code.

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

[1]: http://www.ode.org/
[2]: http://dblog.aldacron.net/derelict-help/using-derelict/
[3]: https://github.com/DerelictOrg/DerelictUtil/wiki/DerelictUtil-for-Users
