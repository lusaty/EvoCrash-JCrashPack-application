# MATH-38b

## Stacktrace

```
org.apache.commons.math.optimization.direct.BOBYQAOptimizer$PathIsExploredException: If this exception is thrown, just remove it from the code prelim (at line 1752)
	at org.apache.commons.math.optimization.direct.BOBYQAOptimizer.prelim(BOBYQAOptimizer.java:1752)
	at org.apache.commons.math.optimization.direct.BOBYQAOptimizer.bobyqb(BOBYQAOptimizer.java:407)
	at org.apache.commons.math.optimization.direct.BOBYQAOptimizer.bobyqa(BOBYQAOptimizer.java:332)
	at org.apache.commons.math.optimization.direct.BOBYQAOptimizer.doOptimize(BOBYQAOptimizer.java:244)
	at org.apache.commons.math.optimization.direct.BaseAbstractMultivariateOptimizer.optimize(BaseAbstractMultivariateOptimizer.java:125)
	at org.apache.commons.math.optimization.direct.BaseAbstractMultivariateSimpleBoundsOptimizer.optimize(BaseAbstractMultivariateSimpleBoundsOptimizer.java:138)
```

## Frame 1 to 4

Best fitness: failed

Method is complex with a lot of lines and nested if statements.
