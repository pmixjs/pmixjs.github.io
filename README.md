# pmixjs.github.io
Main repo/website for project pmix.

## Another bloated library - until it's not
It's common nowadays to use libraries to ease the load of the development process. One major drawback is that libraries tend to get bloated and huge, and often riddled with dependencies. Some say this is not good, especially since the client's browser needs to download all those assets, which is bad on users on slow connections, on limited data plans, and for loading times in general.

That's what pmix is designed to deal with. The core concept of pmix is to **pick and mix** the assets you need and nothing else, and in the process decrease the size of the project, and also remove as many dependenccies as possible.

## Basic concept
First step is to download the library and its control file. These are stored in the root of the working directory of your project. Preferably you link to the library in your project so you have full access to all the functions and tools the library hjas to offer. Then you simply use the functions as needed in your JS. When you're ready to push to production you run the compiler. The compiler scans through the working tree and reads through your JS. It spots which functions you use and keeps a log of them. When it has finished scanning everything it refers to the main file and cuts out what's needed and creates a new file with only the assets you need, so you get the perks of a small file but also a single file with your assets, webpack style.

## The main file
The main file provides the actual code. It's a big file with a plethora of utility functions, compact libraries, and polyfills. Its core function is to extend and streamline JS, which includes providing useful libraries like modals, math utilities, etc. Every function is designed to be fast, minimal, and compatible with as many browsers as possible, going back to old versions of Internet Explorer.

## The control file
The control file controls the hierarchy of the library. It also serves as a directory that makes it easy to get an overview of the function set.
