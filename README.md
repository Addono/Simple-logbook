# Simple logbook
A simple logbook package to track and display the amount of time spend during a project.
![screenshot-of-the-application](https://raw.githubusercontent.com/Addono/Simple-logbook/master/screen-shot.png)

## Usage
Start by copying `logbook.sty` and `nth.sty` to the root of your LaTeX project. 

*Note: `nth` might be optional, if your package manager includes it, however we observed that it generally isn't.*

```tex
\begin{logbookTable}{table-name}
  %\logEntry{Month}{Day}{# minutes}{Description}

  % Initial phase
  \logEntry{02}{02}{120}{Did something.}
  \logEntry{02}{04}{120}{And more things.}
  \logSubtotal{Initial phase}  % Using logSubtotal is optional

  % Second phase
  \logEntry{02}{14}{50}{Started on the second phase.}
  \logEntry{02}{16}{60}{Did things.}
  \logSubtotal{Second phase}
  
  % Add a row summing the amount of time spent during the whole project.
  \logTotal
\end{logbookTable}
```

See `example.tex` for a complete example on how to use this package.
