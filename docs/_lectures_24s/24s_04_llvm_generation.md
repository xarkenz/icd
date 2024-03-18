---
layout: page
slug: "04"
title: "04. LLVM Generation"
---

You can find the example implementation for this lecture
[here](https://github.com/xarkenz/icd-example/tree/03_llvm-generation).

## Lecture Recording

<iframe
    src="https://www.youtube-nocookie.com/embed/8fgO8fI_jJA?si=X4OwJJgMuND9hg1T"
    title="YouTube video player"
    frameborder="0"
    width="560"
    height="315"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share"
    allowfullscreen
    style="width: 100%; height: 100%; aspect-ratio: 16 / 9;"
></iframe>

## Lecture Slides

<iframe
    src="https://docs.google.com/presentation/d/e/2PACX-1vSCUVPhszjpys1AICT0CDwqbwxR_UYI6VGyFzQe9WKp2ZgbD36pYRC_w07Aj5_ZMPE81FgaWohm-2rq/embed?start=false&loop=false&delayms=3000"
    frameborder="0"
    width="960"
    height="569"
    allowfullscreen="true"
    mozallowfullscreen="true"
    webkitallowfullscreen="true"
    style="width: 100%; height: 100%; aspect-ratio: 16 / 9;"
></iframe>

## Resources

### Program Preamble

```llvm
; ModuleID = 'examples/test1'
source_filename = "examples/test1"
target datalayout = "e-m:e-p270:32:32-p271:32:32-p272:64:64-i64:64-f80:128-n8:16:32:64-S128"
target triple = "x86_64-pc-linux-gnu"

@print_int_fstring = private unnamed_addr constant [4 x i8] c"%d\0A\00", align 1

; Function Attrs: noinline nounwind optnone uwtable
define dso_local i32 @main() #0 {
```

### Program Postamble

```llvm
    ret i32 0
}

declare i32 @printf(i8*, ...) #1

attributes #0 = { noinline nounwind optnone uwtable "frame-pointer"="all" "min-legal-vector-width"="0" "no-trapping-math"="true" "stack-protector-buffer-size"="8" "target-cpu"="x86-64" "target-features"="+cx8,+fxsr,+mmx,+sse,+sse2,+x87" "tune-cpu"="generic" }
attributes #1 = { "frame-pointer"="all" "no-trapping-math"="true" "stack-protector-buffer-size"="8" "target-cpu"="x86-64" "target-features"="+cx8,+fxsr,+mmx,+sse,+sse2,+x87" "tune-cpu"="generic" }

!llvm.module.flags = !{!0, !1, !2, !3, !4}
!llvm.ident = !{!5}

!0 = !{i32 1, !"wchar_size", i32 4}
!1 = !{i32 7, !"PIC Level", i32 2}
!2 = !{i32 7, !"PIE Level", i32 2}
!3 = !{i32 7, !"uwtable", i32 1}
!4 = !{i32 7, !"frame-pointer", i32 2}
!5 = !{!"Ubuntu clang version 10.0.0-4ubuntu1"}
```
