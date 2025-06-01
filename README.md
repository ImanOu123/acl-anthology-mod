# Modified ACL Anthology (with Translation Feature)

This is the repo for the web demonstration of "Towards Global AI Inclusivity:
A Large-Scale Multilingual Terminology Dataset (GIST)". The web demonstration is
to show how the translation method introduced in the paper can be implemented
in a real-world context. For the sake of ease of building/running, the page is
restricted to papers from 2024-2025.

The original home of this repository is <https://github.com/acl-org/acl-anthology>,
checkout the original repo for details on how to build and run the ACL anthology
locally in order to preview this demo.

**TLDR** of running/building server:
```
make clean
make all
make serve
```

There are no special requirments that this modified version of the website needs - some 
features have been disabled in this repo's Make file because they aren't relevant to the demo.

For the translation feature to work, you need to run the server from
<https://github.com/jiarui-liu/MultilingualAITerminology/tree/main/server>
first. This demonstration relies on the server being run from http://127.0.0.1:8765.

The main changes of the translation feature are implemented in
[/hugo/layouts/papers/single.html](https://github.com/ImanOu123/acl-anthology-mod/blob/master/hugo/layouts/papers/single.html).
Most of the other changes to the original repo are to remove the other papers not included
in this demo.
