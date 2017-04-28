
# towebp

**Just a simplifying wrapper around [Google's cwebp command](https://developers.google.com/speed/webp/docs/cwebp)**


## Requirements
This bash script requires the [cwebp encoding tool](https://developers.google.com/speed/webp/docs/cwebp). For information about webp, see Google's article [“A new image format for the Web”](https://developers.google.com/speed/webp/) and their [webp encoding guide](https://developers.google.com/speed/webp/docs/cwebp)

## Installation

### Homebrew / OSX:

```bash
$ brew install germaniakg/images/towebp
```

### Linux

Clone the repo somewhere. Do not forget to add the **towebp** directory to your local **$PATH** variable.

```bash
$ git clone https://github.com/GermaniaKG/towebp.git towebp
```

## Usage

Pass an input file and optionally a quality parameter:

```bash
$ towebp <image>
$ towebp <image> [quality]
```

### Example

```bash
$ towebp photo.jpg
$ towebp photo.jpg 75
```

## What happens inside?

towebp calls `cwebp` with these parameters:

- `-quiet`
- `-alpha_cleanup on`
- `-q 85` or, the quality factor passed, respectively








