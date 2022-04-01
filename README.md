## NOTE!

This repository is work in progress. I seem to recall that it may require
something else than just this to get a Bridge.NET project to work, and I haven't
yet tested this one on a fresh Windows install or Wine prefix.

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

## Why not provide an installer instead?

Yeah, Bridge.NET had one. That would be more reliable. The reason is, I have
probably deleted mine. I probably should compile a new one from the source but
avoiding learning to do that is the very reason I'm saving this binary here. I
may add the installer later if I find one still sitting on my hard disk.

## Any license?

The Apache license of the compiler itself applies. See the link to source I
provided. No additional conditions from me.
