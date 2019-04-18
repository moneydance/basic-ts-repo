# basic-ts-repo

npm install
npm run start
go to http://localhost:8080/

you can remove the lodash dep. I was just testing that bundling libraries works as expected.


at some point you might want top level imports it allows you to avoid doing annoying relative path sytax

ex:
    ~/src/test instead of ../../../test

tsconfig supports that with
compilerOptions: {
  "paths": {
    "~*": ["./src/*"]
  }
}

Browserify doesn't have good support for this. The more modern bundler like webpack, fuse-box and parcel do though!
