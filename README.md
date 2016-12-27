<h1>The DNA# compiler</h1>
<hr>
Coded in OCaml, DNA# is a biology computational language. It has major common data types plus nucleotde, amino acid, DNA, RNA, and peptide types. Key functions include transcribe and translate functions, which mimic the biological process. It is compiled into LLVM IR.

It needs the OCaml llvm library, which is most easily installed through opam.

Install LLVM and its development libraries, the m4 macro preprocessor, and opam, then use opam to install llvm.

The version of the OCaml llvm library should match the version of the LLVM system installed on your system.

It also requires clang compiler for the c built-in functions inside the compiler.
( to install clang: sudo apt install clang )

To run your dna files using the following command:<br>
make    (to build the compiler first)<br/>
./runDNAs.sh -r filename.dnas<br/>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-a   Print AST of file<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-c   Compile file<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-r   Run file<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;-h   Print this help<br>

If the terminal shows "can't find command",feed "chmod +x runDNAs.sh" into the terminal first.

To run all the test files, run the following command:
./test_DNAs.sh

Clean up all the built files/dependencies -> make clean
