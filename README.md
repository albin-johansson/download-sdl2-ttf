# download-sdl2-ttf

This is an action for downloading SDL2_ttf sources and runtime binaries on Windows using MSVC.

The downloaded headers will be stored under `sources_destination`, in a separate `SDL2_ttf-X.Y.Z` folder, where X.Y.Z corresponds to the version, e.g. `2.0.15`. The `binaries_destination` is the folder where all of the runtime binaries (`.dll` files) will be stored.

Note, you will have to make sure that the destination folders exist before invoking the action.

## Usage

```yml
- name: Download SDL2_ttf
  uses: albin-johansson/download-sdl2-ttf@v1
  with:
    sources_destination: .
    binaries_destination: bin
```
