# Does Xenia run on Linux or macOS?

The project is designed to support non-Windows platforms but until it's running
games it's not worth the maintenance burden. MacOS will likely remain unsupported
until Apple supports Vulkan.

There's only a few major pieces that need cleanup before a Linux port can
proceed in earnest, listed with the [cross-platform tag](https://github.com/xenia-project/xenia/labels/cross-platform).
Most of the code compiles with the latest Clang, and very few files have
dependencies on Windows APIs (all of that is isolated to `_win.cc` files).
Though the codebase is ready for the port, it's not a trivial task and anyone
seeking to port it will need a deep understanding of Linux, X11, Vulkan, and
Win32 (to ensure matching semantics).


# You should port it to Linux, then tons of developers will contribute!

No, they won't, and that's not how things work. (I'm seriously told this once
a week...)

Think of it this way: the most important kind of contributor in this phase of
the project is one who is capable of performing the porting work. If someone
has this capability and feels so strongly about Linux support then they would be
contributing to the porting efforts already. But otherwise they are nothing
more than hypothetical members of our collective dreams.


# Why did you do X? Why not just use Y? You should use Y. NIH NIH NIH!

Trust that I either have a good reason for what I did or have absolutely no
reason for what I did. This is a large project that I've been working on
for almost 5 years and in that time new compilers and language specs have
been released, libraries have been created and died, and I've learned a lot.
Constructive contributions and improvements are welcome.


# Have you heard of LLVM/asmjit/jitasm/luajit/etc?

Yes, I have heard of them. In fact, I spent a long time trying them out:
[LLVM](https://github.com/xenia-project/xenia/tree/85bdbd24d1b5923cfb104f45194a96e7ac57026e/src/xenia/cpu/codegen),
[libjit](https://github.com/xenia-project/xenia/tree/eee856be0499a4bc721b6097f5f2b9446929f2cc/src/xenia/cpu/libjit),
[asmjit](https://github.com/xenia-project/xenia/tree/ca208fa60a0285d396409743064784cc2320c094/src/xenia/cpu/x64).
I did not find them acceptable for use in this project for various reasons. If
for some reason you feel strongly otherwise, feel free to either contribute a
[new CPU backend](https://github.com/xenia-project/xenia/tree/master/src/xenia/cpu/backend).


# (some argument over an unimportant technical choice)

In general: *I don't care*.
That means I either really don't care and something is they way it is because
that was convenient or that I don't care because it's not material to the goal
of the project. There are a million important things that need to be done to get
games running and going back and forth about unimportant orthogonal issues does
not help. If you really do have a better way of doing something and can show it,
contributions are welcome.

Here's a short list of common ones:

* 'Why this xb stuff?' -- I like it, it helps me. If you want to
manually execute commands have fun, nothing is stopping you.
* 'Why not just take the code from project X?' -- the point of this project
is to build something different than previous emulator projects and learn while
doing it. The easy way is almost never the best way and most certainly isn't as
fun.
* 'Why not CMake?' -- I don't like CMake as it generates ugly Visual Studio
projects. Premake does what I want (mostly) how I want it to.


# Hey I'm going to go modify every file in the project, ok?

We welcome contributions, but please try to understand that we cannot accept
changes that radically alter the structure or content of the code, especially
if they are aesthetic and even more so if they are from someone who has not
contributed before. If a pull request of this nature is denied that doesn't
necessarily mean your help is not wanted, just that it may need to be more
carefully applied.
