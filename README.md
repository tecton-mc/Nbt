# Nbt

NBT (Named Binary Tag) library for Zig 0.17.0

## Installation

Add the dependency with `zig fetch`:

```sh
zig fetch --save git+https://github.com/tecton-mc/Nbt.git
```

Then in your `build.zig`:

```zig
const nbt_dep = b.dependency("nbt", .{
    .target = target,
    .optimize = optimize,
});

exe.root_module.addImport("nbt", nbt_dep.module("nbt"));
```

## Usage

```zig
const nbt = @import("nbt");
```

## License

[MIT](LICENCE)
