# SqlCipher4Unity3D

## What's this?

 This project was insprited in [codecoding/SQLite4Unity3d](https://github.com/codecoding/SQLite4Unity3d).

 When I started with Unity3d development I needed to use SQLite in my project and it was very hard to me to find a place with simple instructions on how to make it work. All I got were links to paid solutions on the Unity3d's Assets Store and a lot of different and complicated tutorials.

 At the end, I decided that there should be a simpler way and I created **SqlCipher4Unity3D**, a plugin that helps you to use SqlCipher in your Unity3d projects in a clear and easy way.

 It uses the great [sqlite-net](https://github.com/praeclarum/sqlite-net) library as a base so you will have **Linq besides sql**. For a further reference on what possibilities you have available with this library I encourage you to visit [its github repository](https://github.com/praeclarum/sqlite-net).

- Note: _SQLite4Unity3d uses only the synchronous part of sqlite-net, so all the calls to the database are synchronous._

## Support Platforms

| Platforms |             | Support? | SQLCipherVersion                                                                          |
|-----------|-------------|----------|-------------------------------------------------------------------------------------------|
| Windows   | x86         | O        | v4.4.0                                                                                    |
| Windows   | x86_64      | O        | v4.4.0                                                                                    |
| Linux     | x86_64      | O        | v4.4.0                                                                                    |
| macOS     | x86_64      | O        | [v4.4.0](https://github.com/jfcontart/SqlCipher4Unity3D_Apple)                            |
| iOS       | 64bit       | O        | [v4.4.0](https://github.com/jfcontart/SqlCipher4Unity3D_Apple)                            |
| tvOS      | 64bit       | O        | [v4.4.0](https://github.com/jfcontart/SqlCipher4Unity3D_Apple)                            |
| Android   | armeabi-v7a | O        | [v4.4.0](https://mvnrepository.com/artifact/net.zetetic/android-database-sqlcipher/4.4.0) |
| Android   | arm64_v8a   | O        | [v4.4.0](https://mvnrepository.com/artifact/net.zetetic/android-database-sqlcipher/4.4.0) |
| Android   | x86         | O        | [v4.4.0](https://mvnrepository.com/artifact/net.zetetic/android-database-sqlcipher/4.4.0) |
| Android   | x86_64      | O        | [v4.4.0](https://mvnrepository.com/artifact/net.zetetic/android-database-sqlcipher/4.4.0) |
| Linux     | x86         | X        |                                                                                           |
| WebGL     |             | X        |                                                                                           |

## Watchout

- Check [Issues](https://github.com/netpyoung/SqlCipher4Unity3D/issues)
- If You are on iOS, need to modify [link.xml](https://docs.unity3d.com/Manual/iphone-playerSizeOptimization.html) for prevent stripping by Unity.

## Compatibility

From `1.1.0` I removed `v` prefix for support UPM.

| SqlCipher4Unity3D tag | sqlcipher version                                                                                                |
|-----------------------|------------------------------------------------------------------------------------------------------------------|
| 1.1.x                 | 4.x.x                                                                                                           |
| v1.0.x                | [3.x.x](https://github.com/netpyoung/SqlCipher4Unity3D/blob/2c642b3f0387dadfb4a145cb7236e99c9109fb94/README.md) |

## The fast track

All you have to do to start using it in your project:

1. Download unitypackage, then extract its content on your Unity3D Project. It contains the dlls that Unity3d will need to access sqlite.
   - [v1.0.2.unitypackage](https://github.com/netpyoung/SqlCipher4Unity3D/releases/download/v1.0.2/SqlCipher4Unity3D-v1.0.2.unitypackage) (for sqlcipher 3.x.x)
   - [1.1.0.unitypackage](https://github.com/netpyoung/SqlCipher4Unity3D/releases/download/1.1.0/SqlCipher4Unity3D-1.1.0.unitypackage) (for sqlcipher 4.x.x)
2. **You’re done!**

## Examples & Tests

- [./SqlCipher4Unity3D/Assets/example/](./SqlCipher4Unity3D/Assets/example/)
- [./SqlCipher4Unity3D/Assets/test/](./SqlCipher4Unity3D/Assets/test/)

## UPM

``` json
"com.netpyoung.sqlcipher4unity3d": "https://github.com/netpyoung/SqlCipher4Unity3D.git?path=SqlCipher4Unity3D/Assets/SqlCipher4Unity3D#1.1.0"
```

## Contributer(❤️)

- [@jfcontart]

## LICENCE

| project                                                                                   | license                                                                 |
|-------------------------------------------------------------------------------------------|-------------------------------------------------------------------------|
| [netpyoung/SqlCipher4Unity3d](./)                                                         | [MIT](./LICENSE)                                                        |
| [jfcontart/SqlCipher4Unity3D_Apple](https://github.com/jfcontart/SqlCipher4Unity3D_Apple) | [copyleft](https://github.com/jfcontart/SqlCipher4Unity3D_Apple)        |
| [robertohuertasm/SQLite4Unity3d](https://github.com/robertohuertasm/SQLite4Unity3d)       | [MIT](https://github.com/codecoding/SQLite4Unity3d/blob/master/LICENSE) |
| [praeclarum/Sqlite-net](https://github.com/praeclarum/sqlite-net)                         | [MIT](https://github.com/praeclarum/sqlite-net/blob/master/LICENSE.txt) |
| [SQLite](sqlite370_banner.gif)                                                            | [SQLite's License](https://sqlite.org/copyright.html)                   |
| [SQLCipher](https://www.zetetic.net/sqlcipher/)                                           | [SQLCipher's License](https://www.zetetic.net/sqlcipher/license/)       |

### SQLite's Licnese

``` license
All of the code and documentation in SQLite has been dedicated to the public domain by 
the authors. All code authors, and representatives of the companies they work for, have
 signed affidavits dedicating their contributions to the public domain and originals of 
 those signed affidavits are stored in a firesafe at the main offices of Hwaci. Anyone 
 is free to copy, modify, publish, use, compile, sell, or distribute the original SQLite
  code, either in source code form or as a compiled binary, for any purpose, commercial 
  or non-commercial, and by any means.

The previous paragraph applies to the deliverable code and documentation in SQLite - 
those parts of the SQLite library that you actually bundle and ship with a larger 
application. Some scripts used as part of the build process (for example the "configure"
 scripts generated by autoconf) might fall under other open-source licenses. Nothing 
 from these build scripts ever reaches the final deliverable SQLite library, however, 
 and so the licenses associated with those scripts should not be a factor in assessing 
 your rights to copy and use the SQLite library.

All of the deliverable code in SQLite has been written from scratch. No code has been 
taken from other projects or from the open internet. Every line of code can be traced 
back to its original author, and all of those authors have public domain dedications on 
file. So the SQLite code base is clean and is uncontaminated with licensed code from 
other projects.
```

### SQLCipher's Licnese

``` license
Copyright (c) 2008-2012 Zetetic LLC
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:
    * Redistributions of source code must retain the above copyright
      notice, this list of conditions and the following disclaimer.
    * Redistributions in binary form must reproduce the above copyright
      notice, this list of conditions and the following disclaimer in the
      documentation and/or other materials provided with the distribution.
    * Neither the name of the ZETETIC LLC nor the
      names of its contributors may be used to endorse or promote products
      derived from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY ZETETIC LLC ''AS IS'' AND ANY
EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL ZETETIC LLC BE LIABLE FOR ANY
DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

----------------

[@jfcontart]: https://github.com/jfcontart