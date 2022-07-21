# mobile

Files and documentation relevant to all of the mobile projects at Customer.io. 

# What this project is good for:

* Writing of general documentation that is relevant to all mobile projects at Customer.io. If there is documentation that is relevant to only 1 type of technology (for example talking about setting up XCode for just the iOS SDK), it might be good to belong there instead of in this project. However, a document talking about linting of Kotlin code (relevant to *all* of the Android projects in the company) then the documentation is welcome here. 

* Configuration files that other projects can reference. Some tools allow you to reference a file by URL to execute instead of having to copy and paste the file. However, this can cause projects to break. Let's say that a linting tool is setup to use a config file from `https://github.com/customerio/mobile/ktlint.config`. If you make a git tag today for 1.0 of your project, the tool is configured to reference that remote file at the URL. Let's say 6 months goes by and you have made many changes to `ktlint.config` file. If you ever try and build v1.0 of your project that you wrote 6 months ago, you may experience errors because of breaking changes you introduced to your config file! 

To avoid this, it's best to reference a git commit hash or a git tag of this project to reference. Then, v1.0 of your software will always reference a config file that it was setup to use at that time. 

