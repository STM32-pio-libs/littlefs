# littlefs — PlatformIO package

> **This repository does not contain original code.**
> The source files (`lfs.c`, `lfs.h`, `lfs_util.c`, `lfs_util.h`) are copied
> verbatim from the official
> [littlefs-project/littlefs](https://github.com/littlefs-project/littlefs)
> release **v2.11.3** and are the work of the littlefs authors and Arm Limited.
> The only additions in this repo are the PlatformIO manifest (`library.json`),
> this README, and the example integration for W25Q64.

---

## What is LittleFS?

LittleFS is a small, power-loss-resilient filesystem designed for
microcontrollers backed by NOR flash.  Key properties:

- **Wear levelling** — spreads writes evenly across sectors automatically.
- **Power-loss resilience** — a sudden reset will never corrupt the filesystem;
  at worst the last unsynced write is lost.
- **No dynamic allocation required** — all working buffers are caller-supplied.

Upstream repository: <https://github.com/littlefs-project/littlefs>  
Upstream documentation: <https://github.com/littlefs-project/littlefs/blob/master/README.md>

---

## License

The littlefs source code is licensed under the **BSD 3-Clause License**:

```
Copyright (c) 2022, The littlefs authors.  
Copyright (c) 2017, Arm Limited. All rights reserved.

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

-  Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
-  Redistributions in binary form must reproduce the above copyright notice, this
   list of conditions and the following disclaimer in the documentation and/or
   other materials provided with the distribution.
-  Neither the name of ARM nor the names of its contributors may be used to
   endorse or promote products derived from this software without specific prior
   written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

The PlatformIO manifest, README, and example code in this repository are
released under the **MIT License** by Anurag Kumar Singh.

---

## Repository layout

```
include/
    lfs.h           ← upstream, unmodified
    lfs_util.h      ← upstream, unmodified
src/
    lfs.c           ← upstream, unmodified
    lfs_util.c      ← upstream, unmodified
library.json
README.md
```
