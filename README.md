# cflint-underscore-test
I did the following to reproduce the error I was experiencing while running CFLint on some of my projects.

I downloaded and used Maven to build the latest dev version of CFLint ([94c9574ac0d688b247d817f5b6695cff9e9c11f5](https://github.com/cflint/CFLint/tree/94c9574ac0d688b247d817f5b6695cff9e9c11f5)).

I ran it on this project folder (`cflint -folder .`), which is a simple index (pulled from one of Ray Camden's old posts: https://gist.github.com/cfjedimaster/3353562#file-gistfile1-cfm).
It uses https://github.com/russplaysguitar/underscorecf, which is a really helpful library.

The generated CFLint report file is included in the repo here.

The errors in parsing mentioned in the issue (https://github.com/cflint/CFLint/issues/269) are still present.

Also of note, the severity of the errors does not appear to be getting logged correctly.
