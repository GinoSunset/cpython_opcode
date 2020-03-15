# cpython_otus_opcode
Add new opcode to cpython.

Patch for __python 2.7__

 The patch includes adding a new opcode  `LOAD_OTUS`. The opcode is a replacement for two opcodes:
 * `LOAD_FAST` with the argument 0 
 * `LOAD_CONST` with any argument.

 The `LOAD_COUNT` argument is passed to `LOAD_OTUS`. The `LOAD_FAST` replace to `NOP`.

 ## How install patch:
-------
* clone cpython 
    ```
    git clone https://github.com/python/cpython.git
    cd cpython
    git checkout 2.7
    ```
* change to new branch
    ```
    git checkout -b opcode_otus
    ```

* applay patch:
    ```
    git apply --check new_opcode.patch
    ```
