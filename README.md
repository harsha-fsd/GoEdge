# Cross-compiling from x86_64 to ARM with Go


if your environment is under x86_64 and you want to cross-compile for ARMv7
support, execute the following commands:

```env GOOS=linux GOARM=7 GOARCH=arm go build example.go<code>```

or for ARMv8 64-bit support, execute the following command
 ``` env GOOS=linux GOARCH=arm64 go build example.go ```

Copy the generated binary (./example) to your ARM device and test if it works.
