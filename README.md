cloudinary-scala-play-repo
==========================

Compiled Cloudinary Scala sources for Play Framework

In Build.scala add:
```
val main = play.Project(appName, appVersion, appDependencies).settings( 
  resolvers += Resolver.url("Andrew Boss Custom Cloudinary Core", url("https://raw.github.com/andrewboss/cloudinary-scala-core-repo/master"))(Resolver.ivyStylePatterns),
  resolvers += Resolver.url("Andrew Boss Custom Cloudinary Play Plugin", url("https://raw.github.com/andrewboss/cloudinary-scala-play-repo/master"))(Resolver.ivyStylePatterns) 
)
```
