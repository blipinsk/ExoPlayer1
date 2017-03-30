ExoPlayer 1
===========

An external packaging of [Google's ExoPlayer version 1.x.x][1].

Although Google thought about releasing ExoPlayer 2 with a different package name, they seemed to
forgot to change the `artifactId` of the published snapshot. That's why you cannot include both
ExoPlayer 1 and ExoPlayer 2 in your project at the same time (using two simple dependency records).
Which would be really useful if you want to gradually migrate an old ExoPlayer 1 project to the newer version.

This project is a simple repackaging of ExoPlayer 1.x.x versions. It contains no code of my own.
Just a bare minimum to upload a snapshot with a different `groupId` and `artifactId`.

Unfortunately, according to [Issue #1842][2] Google has no plans to introduce the second
`artifactId` for the r2.x.x versions. That's why using a solution like this or including a .jar in
your project are pretty much the only choices you have.


Versions
--------

I am keeping the original notation of version numbering. Every version name matches `r1.x.x` pattern.


Download
--------

```groovy
compile 'com.bartoszlipinski:exoplayer1:r1:x.x'
compile 'com.google.android.exoplayer:exoplayer:r2.x.x'
```


Release Notes
-------------

This project contains no code. See [ExoPlayer's release notes][3] instead.


License
-------

This project contains no code. See [ExoPlayer's license][4] instead.


 [1]: https://github.com/google/ExoPlayer/tree/release-v1
 [2]: https://github.com/google/ExoPlayer/issues/1842#issuecomment-248851725
 [3]: https://github.com/google/ExoPlayer/blob/release-v1/RELEASENOTES.md
 [4]: https://github.com/google/ExoPlayer/blob/release-v1/LICENSE