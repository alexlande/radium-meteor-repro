A reproduction to test an issue with Meteor builds + Radium 0.17.0.

## Instructions

1. Install Meteor (https://www.meteor.com/install)
2. Clone this repo
3. Run `meteor npm install` to install dependencies
4. Run `meteor build ./build --architecture os.linux.x86_64 --allow-incompatible-update` to attempt to build.

## Result

You should see this error:

```
❯ meteor build ./build --architecture os.linux.x86_64 --allow-incompatible-update

WARNING: The output directory is under your source tree.
         Your generated files may get interpreted as source code!
         Consider building into a different directory instead
         meteor build ../output

Errors prevented bundling:
While linking the program:
error: this app is not compatible with architecture 'os.linux.x86_64'
```
