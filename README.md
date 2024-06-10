# Backported Webpack Config for Flarum JS/TS Compilation

This fork of the Flarum Webpack config backports key changes from Flarum 2.x to 1.x.

## Background

In Flarum 2.x, the JavaScript compilation process was streamlined by removing unnecessary ES5 polyfills, resulting in a reduced bundle size and modernized ES6 output. These changes can be found in the original [PR #3699](https://github.com/flarum/framework/pull/3699).

## Key Changes

- Outputs ES6 JavaScript instead of ES5.
- Reduces bundle size by excluding unnecessary ES5 polyfills.
- Requires recompilation of all extension JS source code with the updated Webpack config.

These changes aim to future-proof the codebase and enhance performance by utilizing modern JavaScript features.
