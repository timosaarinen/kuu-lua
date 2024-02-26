DEPRECATED: Unless at some point will come back to this for some reason, this project is now cancelled. This step was not taken lightly, as Lua is a beautiful and minimalistic language - and would have been ready to use.

# kuu-lua

* *Why?* ..Need it myself, open-sourced in case if someone else needs it (MIT license)
* *What?* ..WebAssembly port of the Lua C interpreter for web environment (including limited runtime support)
* *How?* ..Emscripten and lots of tweaking

## Kuu?

"Lua" is "moon" in Portuguese, "Kuu" is "moon" in Finnish.

## Interpreter? LuaJIT is faster, it's has a JIT!

While LuaJIT is nice (have used it myself in some projects) - and “Mike Pall is a robot from the future” - direct Just-In-Time compiling has a problem in web environment. For starters, it doesn't work at all.

Indirect JIT compiling, taking advantage of JS/WASM JIT compilers built into browsers is one option, but most approaches require you to statically compile Lua to JS/WASM, which brings its own can of worms. Following the KISS principle, interpreter is *good enough*.
