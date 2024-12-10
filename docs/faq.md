---
title: Frequently Asked Questions
layout: page
description: Frequently Asked Questions
permalink: "/docs/faq/"
intro_image_absolute: true
intro_image_hide_on_mobile: false
---

#### Where should I ask questions on Slang?

If you run into any questions with the Slang language, the compilation API or the reflection API, please post it on our [GitHub discussion page](https://github.com/shader-slang/slang/discussions).

#### How do I report a compiler bug?

Please post your issues on our [GitHub issues page](https://github.com/shader-slang/slang/issues).


#### Does Slang use LLVM?

No. The Slang compiler itself is not built on the LLVM tech stack, and does not depend on LLVM.
If you are using Slang to generate textual or SPIRV code, no LLVM binaries are required. If you are using Slang to produce standalone executables or dynamically linked
libraries, then a prebuilt LLVM wrapper library called `slang-llvm` is required.

#### What's the distribution size of Slang?

The Slang compiler binary is around 5-10 MB depending on build configuration and target architecture.

#### Can I add another code generation target to Slang?

Absolutely! Slang is open and everyone is welcomed to contribute! Slang supports two types of targets: textual targets such as HLSL/GLSL/WGSL/C++ or binary targets such as SPIRV. Generally, adding support for textual targets is simpler and a lot of the infrastructure can be reused between the targets. We recently added support for Metal and WGSL, and more backends can be added following the similar process. Please create a discussion thread on the [Slang GitHub repo](https://github.com/shader-slang/slang/discussions) to start working with the dev team on adding a new target.