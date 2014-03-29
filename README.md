cloudinary-scala-play-repo
==========================

cloudinary-scala-play 0.9.3-SNAPSHOT for Play Framework

In your Play Framework Build.scala add:
```
val appDependencies = Seq(
  "com.cloudinary" %% "cloudinary-scala-play" % "0.9.3-SNAPSHOT"
)

val main = play.Project(appName, appVersion, appDependencies).settings( 
  resolvers += Resolver.url("Andrew Boss Custom Cloudinary Core", url("https://raw.github.com/andrewboss/cloudinary-scala-core-repo/master"))(Resolver.ivyStylePatterns),
  resolvers += Resolver.url("Andrew Boss Custom Cloudinary Play Plugin", url("https://raw.github.com/andrewboss/cloudinary-scala-play-repo/master"))(Resolver.ivyStylePatterns) 
)
```

In Play.plugins add:
```
10007:cloudinary.plugin.CloudinaryPlugin
```
