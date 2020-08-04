# Problem Statement
- In distributed storage, nodes can go down. Build fault tolerant system, which works event if node goes down.
- Want
    - Tolerate many node failures
    - Not too much storage overhead
    - we can reconstruct one failed node quickly.

Solution
- Error correcting code
- https://mathworld.wolfram.com/Error-CorrectingCode.html#:~:text=Entries%20%3E%20Interactive%20Demonstrations%20%3E-,Error%2DCorrecting%20Code,based%20on%20the%20remaining%20numbers.

# ErasureCoding
- Protect and gaurantee data availability
- It's part of Coding theory

## What is ErasureCoding?
The basic premise of erasure coding goes as follows:ss
`Take a file and split into k pieces and encode into n pieces. Now, any k pieces can be used to get back the file.`
- https://www.youtube.com/watch?v=Q5kVuM7zEUI
- In Erasure Coding, Parity's are Erasure codes

## Advantages and Disadvantages of Erasure Coding
- https://www.quobyte.com/blog/2016/08/15/erasure-coding-in-production/
- http://smahesh.com/blog/2012/07/01/dummies-guide-to-erasure-coding/
- http://docs.netapp.com/sgws-111/index.jsp?topic=%2Fcom.netapp.doc.sg-admin%2FGUID-32497B5F-6540-492D-A128-1FCB6DB4AF49.html


## Implement Erasure coding
- http://web.eecs.utk.edu/~jplank/plank/papers/CS-08-627.html


## Repair problem
- High network bandwidth
- High disk IO at 10 nodes.
- https://www.youtube.com/watch?v=TPZyW_CnXGQ (From 27:00)
- http://users.ece.utexas.edu/~dimakis/index.html

## RS Codes (Reed Solomon codes)
- Are just about evaluating low degree polynomials over finite fields.
- https://www.youtube.com/watch?v=FS503xdAg8U
- https://www.youtube.com/watch?v=Gh578e98qAk

## Reed Solomon Erasure coding
- https://www.youtube.com/watch?v=dpxD8gwgbOc


## Reed solomon Encoding Example
- https://www.youtube.com/watch?v=jgO09opx56o

## Binary Reed Solomon Encoding
https://en.wikipedia.org/wiki/Binary_Reed%E2%80%93Solomon_encoding

## Encode matrix
- https://www.youtube.com/watch?v=h7dwHg3EZjE

## Parity Codes
- solve the linear equation in parity codes to reconstruct missing data 
- https://www.tutorialspoint.com/error-detecting-codes-parity

## Erasure codes
- https://www.youtube.com/watch?v=CryhjBWQHvM
- https://en.wikipedia.org/wiki/Erasure_code

## Galois Field Algebra
- Foundation of erasure coding
- Parity's are Erasure codes.
- 

## MDS codes ( maximum separable distance)
- Any k nodes can get back my file.

## Polynomial Interpolation problem
- https://www.youtube.com/watch?v=Gh578e98qAk

## (n, k) codes
- Reed solomon code
- Array codes
- LDPC codes
- Turbo codes
- 

## In Go
- https://github.com/klauspost/reedsolomon#:~:text=README.md-,Reed%2DSolomon,Backblaze%2C%20with%20some%20additional%20optimizations.

## Different types of parity
- https://www.akalin.com/intro-erasure-codes