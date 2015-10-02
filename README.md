## FileMime

While Go does already include a [mime.TypeByExtension](https://golang.org/pkg/mime/#TypeByExtension) function, this FileMime package is more complete (for use in web apps), works with filename, path or extension, and it's much faster.

## Usage

    extension := []byte(`html`)
    mimetype := filemime.Bytes(extension) // text/html
    extension2 := `/home/mystuff/work.pdf`
    mimetype = filemime.String(extension2) // application/pdf
