## Coding Style Guidelines for WasmEdg

1. **C++ Version:** Specify the C++ version to be used. WasmEdge uses C++17, so all code should be compatible with this version.
2. **LLVM Coding Standards:** Since WasmEdge is part of the LLVM project, it should follow the [LLVM Coding Standards](https://llvm.org/docs/CodingStandards.html).
3. **Use of LLVM Libraries:** WasmEdge uses the LLVM libraries. Therefore, any code that interacts with these libraries should use the appropriate LLVM data structures and algorithms.
4. **Avoid Raw Pointers:** WasmEdge prefers smart pointers over raw pointers to handle memory. So, use `std::unique_ptr`, `std::shared_ptr`, etc., whenever possible.
5. **Include What You Use**: Only include headers that are directly used in a file. This helps to keep the compile times down and makes dependencies between files clearer.
