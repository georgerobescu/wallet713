# Setting up wallet713

# Option 1: Using a pre-compiled binary

## Requirements

* [OpenSSL](https://www.openssl.org).
   * macOS with Homebrew:
      ```
      $ brew install openssl
      ``` 
   * Linux:
      ```
      $ sudo apt-get install openssl
      ``` 

## Download binary

From [releases](https://github.com/vault713/wallet713/releases) section.

## Run

Unzip and then from the same directory run: 
```
$ ./wallet713
```

# Option 2: Building your own binary

## Requirements
wallet713 has the [same requirements](https://github.com/mimblewimble/grin/blob/master/doc/build.md#requirements) as Grin.

## Installation

```
$ git clone https://github.com/vault713/wallet713
$ cd wallet713
$ cargo build --release
```
And then to run:
```
$ cd target/release
$ ./wallet713
```

If you'd like to run against floonet, use:
```
$ cd target/release
$ ./wallet713 --floonet
```