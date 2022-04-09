# Bridge.NET Windows binary

## What's this?

Bridge.NET. It is an open-source discontinued C#-to-JavaScript transpiler whose
primary github repository has disappeared. There are are still forks of
it's source code [available](https://github.com/dtsudo/Bridge.NET), for it's
[CLI](https://github.com/dtsudo/Bridge.NET-CLI) too. However, Those forks do not
contain the precompiled binaries of the traspiler, meaning you'd have to compile
them yourselves.

What you see here is an installed Windows (Well, [Wine](https://www.winehq.org/)
in my case) binary of Bridge.NET, callable from the terminal. Extract these
contents to `C:\Program Files (x86)\Object.NET\Bridge.NET CLI\` and hope it
works.

I did test this myself once on a clean wineprefix (a clean Wine environment)
and it worked. You should have working Internet connection, because the
compiler will need to download the runtime NuGet libraries when you initialise
your project.

The needed NuGet packages are still available, as of writing. But just in case
they disappear I copied the ones I personally use to the packages directory,
plus the config for them (`packages.config`). They include the necessary
Bridge.NET runtime and HTML5 functionality. If `bridge new` can't fetch the
packages from the Internet it'll still initialise the project skeleton
otherwise. Just copy `packages` and `packages.config` from here to your project
skeleton and then you can `bridge build`.

## Why not provide an installer instead?

Yeah, Bridge.NET had one. That would be more reliable. The reason is, I have
probably deleted mine. I probably should compile a new one from the source but
avoiding learning to do that is the very reason I'm saving this binary here. I
might add the installer later if I find one still sitting on my hard disk.

## Any license?

The Apache license of the compiler itself applies. See the link to source I
provided. No additional conditions from me.
