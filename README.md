DerelictODE
===========

A dynamic binding to version 0.12 of the [Open Dynamics Engine][1] physics library for the D Programming Language. Note that version 0.12 of ODE is outdated and new projects should use version 0.13. This branch of DerelictODE is reported to work with version 0.13, but unless you need to maintain an existing codebase you would be better off with the the 0.13 branch of DerelictODE. You can download version 0.12 of the ODE source from the old project page at [Sourceforge][4]

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

[1]: http://www.ode.org/
[2]: http://dblog.aldacron.net/derelict-help/using-derelict/
[3]: https://github.com/DerelictOrg/DerelictUtil/wiki/DerelictUtil-for-Users
[4]: http://sourceforge.net/projects/opende/files/ODE/0.12/
