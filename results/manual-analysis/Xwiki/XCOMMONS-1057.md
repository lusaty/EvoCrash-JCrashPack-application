# XCOMMONS-1057
```
java.lang.ClassCastException: org.xwiki.extension.job.plan.internal.DefaultExtensionPlanNode cannot be cast to org.xwiki.extension.job.internal.AbstractInstallPlanJob$ModifableExtensionPlanNode
    at org.xwiki.extension.job.internal.AbstractInstallPlanJob$ModifableExtensionPlanTree.clone(AbstractInstallPlanJob.java:84)
    at org.xwiki.extension.job.internal.UpgradePlanJob.tryInstallExtension(UpgradePlanJob.java:152)
    at org.xwiki.extension.job.internal.UpgradePlanJob.upgradeExtension(UpgradePlanJob.java:136)
    at org.xwiki.extension.job.internal.UpgradePlanJob.upgradeExtension(UpgradePlanJob.java:85)
    at org.xwiki.extension.job.internal.UpgradePlanJob.upgrade(UpgradePlanJob.java:202)
    at org.xwiki.extension.job.internal.UpgradePlanJob.runInternal(UpgradePlanJob.java:268)
    at org.xwiki.job.AbstractJob.runInContext(AbstractJob.java:206)
    at org.xwiki.job.AbstractJob.run(AbstractJob.java:189)
    at java.util.concurrent.ThreadPoolExecutor.runWorker(ThreadPoolExecutor.java:1142)
    at java.util.concurrent.ThreadPoolExecutor$Worker.run(ThreadPoolExecutor.java:617)
    at java.lang.Thread.run(Thread.java:745)
```

## Frame  2 & 3 & 4 & 5 & 6

Injecting target method is hard. EvoCrash can not do it because it can not find the generator for the genetic type which is needed for initializing the target class (`UpgradePlanJob`)


## Frame  7 & 8

The target class (`AbstractJob`) is an abstract class with lots of abstract methods.
