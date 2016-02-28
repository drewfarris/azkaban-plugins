## Azkaban Plugins

The [3.0.0-jdk7 branch](https://github.com/drewfarris/azkaban-plugins/tree/3.0.0-jdk7)
of this repo is a based on the tagged 3.0.0 release of the
[LinkedIn Azkaban Plugins Repository](https://github.com/azkaban/azkaban-plugins/tree/3.0.0)

It can be built with

```
ant package
```

This has been modified to target JDK 1.7. Some of the azkaban 3.0.0 jars that are
checked in have been rebuilt to contain 1.7 compatible classes.

Currently, a JUnit test for `azkaban.jobtype.TestHadoopJobUtilsExecutionJar` in
the JobType plugin is failing. As a result, the junit task in
`plugins/jobtype/build.xml` has been temporary skipped, although it can be run
by hand.

This build requires `dustc` and `lessc`, from Dust.js and Less.js be installed
and available on the path. 

```
npm install --global dustjs-linkedin
npm install --global less
```

These have been build with dustjs-linkedin 2.7.2 and less 1.7.4

For all Azkaban Plugins documentation, please go to 
[Azkaban Project Site](https://azkaban.github.io/)

