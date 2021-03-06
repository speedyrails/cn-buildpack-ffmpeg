# cn-buildpack-ffmpeg

A Cloud Native Buildpack for FFmpeg.

This buildpack is mainly adapted from [buildpack-ffmpeg](https://github.com/kitcast/buildpack-ffmpeg).

## Usage

1- Clone the repository:

```bash
git clone https://github.com/speedyrails/cn-buildpack-ffmpeg.git
```

2- Add the buildpack to the project:

```bash
pack build myapp --builder heroku/buildpacks:18 --buildpack /path/to/cn-buildpack-ffmpeg --path /path/to/myapp
```

**NOTE:**

- The FFmpeg version installed is 3.4.2-64bit-static.
- The `ffmpeg` binaries will be available from the `PATH` environment variable.
