# Darkroom

## Language
The language I will be using for my DSL is called Darkroom. You can find it at [darkroom-lang.org](http://darkroom-lang.org/index.html).

## Domain
Darkroom is a language for creating _image processing pipelines in Terra_ (Terra itself is a low-level programming language).

## Computational model
Darkroom is actually a very advanced language. While it can efficiently target CPUs, Darkroom can also generate programs for FPGAs and designs for ASICs allowing for extremely fast and efficient image processing. When a program in Darkroom is compiled, the image operations are optimized for the target platform. Actually running Darkroom programs consists of applying the optimized image operations by efficiently loading pixel data into the CPU, FPGA, or ASIC and using CPU instructions or hardware to perform operations from the optimized pipeline. While I don't completely understand how Darkroom works, I know that optimizing how data is loaded and how the image processing pipelines are executed can significantly affect throughput.

## DSL-ness
The Darkroom language really does specialize in image processing pipelines. Darkroom makes it really easy to load and save images and to build pipelines by creating functions that generate output through operations on pixels. While you could theoretically use Darkroom for tasks other than image processing by treating pixels as numbers, it is very clear that this would not be an intended (or very good) use of the language. Darkroom also helps simply image processing operations by encouraging the programmer to work with pixels. Instead of having to define operations on an entire image, you just have to specify how to generate an arbitrary pixel of the output image if given an input image (or images). So, I think it is very clear that Darkroom is a DSL because its operations, functions, and data types revolve around and are specialized for image processing. The syntax also helps convey the task at hand because code isn't cluttered with for loops to iterate over pixels and conditionals to handle edge cases properly.

## Internal or external?
Darkroom would definately be an internal DSL because it is implemented as a library for the Terra language. However, this raises the question of whether Darkroom is even a DSL to begin with. While this debate could probably go into a lot more depth, I'd like to argue that Darkroom should be considered a DSL because the library goes above and beyond what you would normally expect of a library. Even though I'm not an expert on image processing (though I did take Computational Photography), the example code on the Darkroom website was pretty clear and fairly straightforward. It also took a different approach to image processing than what other languages offer that greatly simplifies the work of writing image processing programs. Darkroom handles a lot of the details of image processing as well, further helping programmers focus on what is actually being done instead of how to actually do it. Finally, as far as I know, Terra does not support compiling programs for FPGAs and ASICs. This means that Darkroom has to be a lot more than just a wrapper for some handy functions in Terra and had to involve a lot of work that would normally be associated with creating a programming language (or at least a compiler for one). While Darkroom is "just a library", it almost feels like they integrated it into Terra to make it easier for programmers to use Darkroom code in Terra programs. 

## Host language
According to the Darkroom paper, the compiler was implemented in Terra, which itself is built using LLVM.


## Benefits
Darkroom provides several major benefits to programmers. First of all, it simplifies image processing by allowing programmers to code in a clearer paradigm for image processing. Darkroom handles tedious details that programmers shouldn't need to deal with and can target architectures not supported by most programming languages (including many general purpose ones). Finally, Darkroom relieves programmers from a lot of the work of optimizing their image processing pipelines to achieve great performance. It even beat C++ and Halide (another image processing DSL famous for its great performance).


## Drawbacks
The biggest drawback of Darkroom is that it's integrated into Terra. Since many people haven't heard of Terra before and even fewer know how to code in it, this may significantly increase the barrier to entry to use Darkroom. Even if Darkroom functions can be called from other general purpose programming languages, it still requires Terra to compile, which can increase the size and complexity of projects utilizing Darkroom code.
