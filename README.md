# Assembly: Segmentation Fault due to Out-of-Bounds Memory Access
This repository demonstrates a potential segmentation fault in assembly code due to accessing memory outside allocated bounds. The bug arises from a lack of bounds checking on array indices before dereferencing them. The solution involves adding explicit checks to ensure that the array index is within the valid range before accessing array elements.

## Bug Description:
The provided assembly code attempts to access elements of an array using an index stored in `ecx`. A segmentation fault occurs if `ecx` contains an index that is out of bounds for the array. This often happens due to improper input handling, incorrect calculations or programming errors.

## Bug Solution:
The solution adds bounds checking to prevent the segmentation fault. Before accessing the array, the code verifies that the index `ecx` is valid. If the index is out of bounds, an appropriate error handling routine is invoked, preventing memory access violation. 