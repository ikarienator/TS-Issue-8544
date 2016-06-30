# TS-Issue-8544

This repo is here to reproduce the issues reported in [Microsoft/TypeScript#8544](https://github.com/Microsoft/TypeScript/issues/8544) regarding TypeScript hinting.

- Checkout `master` branch and open it in VSC, and open `ts/main.ts`, and it hints fine.
- Checkout `failure` branch and open it in VSC, and open `ts/main.ts`, and it cannot hint.

The only difference is that in `/ts/main/main.ts`, the ref comment wrongly refers to the folder instead of the file.
The problem IMO is that the user is not notified with the error.