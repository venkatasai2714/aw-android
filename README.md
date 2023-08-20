# aw-android

A very work-in-progress ActivityWatch app for Android.

## Cloning the repository and submodules

Since the main ActivityWatch android repository uses git submodules to manage its modules, you first need to clone the repo and then the submodules.
You can do both in one step with:

```bash
git clone --recursive https://github.com/venkatasai2714/activitywatch.git
```

Or, if you've already cloned normally, you can clone the submodules using:

```bash
git submodule update --init --recursive
```

If you want to ensure you have the latest version of all submodules, preserving any feature branches you have

```bash
git submodule foreach --recursive git pull`
```

## Installing dependencies

- Install rust

```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

- Install nightly

```bash
rustup default nightly
```

- Install Make

```bash
sudo apt-get install make
```

- Install Clang

```bash
sudo apt-get install clang
```

- Install npm

```bash
sudo apt-get install npm
```

## Building

Build

```bash
    make build
```

## Running in android studio

- install the NDK from the `Tools -> SDK Tools` (version: "21.4.7075529")
