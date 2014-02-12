DerelictODE
===========

A dynamic binding to the [Open Dynamics Engine][1] physics library for the D Programming Language.

For information on how to build DerelictODE and link it with your programs, please see the post [Building and Using Packages in DerelictOrg][2] at the Derelict forums.

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
[2]: http://dblog.aldacron.net/forum/index.php?topic=841.0
[3]: https://github.com/DerelictOrg/DerelictUtil/wiki/DerelictUtil-for-Users
