# nand2tetris-snippets

![licence](https://img.shields.io/bower/l/Mi) ![maintenance](https://img.shields.io/maintenance/yes/2020) ![release](https://img.shields.io/github/v/release/lukeJEdwards/nand2tetris-snippets)

## Features

### Syntx high-lighting

![Syntax-High-Lighting](https://github.com/lukeJEdwards/nand2tetris-snippets/blob/master/images/Syntax-high-lighting.PNG?raw=true)

### Snippets

#### hdl Elementry-logic

| Snippet | Body                                   |
| ------- | -------------------------------------- |
| Nand    | `Nand(a=a, b=b, out=out);`             |
| Not     | `Not(in=a, out=out);`                  |
| And     | `And(a=a, b=b, out=out);`              |
| Or      | `Or(a=a, b=b, out=out);`               |
| Xor     | `Xor(a=a, b=b, out=out);`              |
| Mux     | `Mux(a=a, b=b, sel=Selctor, out=out);` |
| DMux    | `Dmux(in=in, sel=selctor, a=a, b=b);`  |

#### hdl Elementry-logic 16bit

| Snippet   | Body                                                                   |
| --------- | ---------------------------------------------------------------------- |
| Not16     | `Not16(in=a, out=out);`                                                |
| And16     | `And16(a=a, b=b, out=out);`                                            |
| Or16      | `Or16(a=a, b=b, out=out);`                                             |
| Mux       | `Mux16(a=a, b=b, sel=Selctor, out=out);`                               |
| Or8Way    | `Or8Way(in=in, out=out);`                                              |
| Mux4Way16 | `Mux4Way16(a=a, b=b, c=c, d=d, e=e, f=f, g=g, h=h, sel=sel, out=out);` |
| DMux4Way  | `DMux4Way(in=in, sel=sel, a=a, b=b, c=c, d=d);`                        |
| DMux8Way  | `DMux8Way(a=a, b=b, c=c, d=d, e=e, f=f, g=g, h=h, sel=sel, out=out);`  |

#### hdl Sequential-chips

| Snippet  | Body                                                         |
| -------- | ------------------------------------------------------------ |
| DFF      | `DFF(in=in, out=out);`                                       |
| Bit      | `Bit(in=in, load=load, out=out);`                            |
| Register | `Register(in=in, load=load, out=out);`                       |
| RAM8     | `RAM8(in=in, load=load, address=addr, out=out);`             |
| RAM64    | `RAM64(in=in, load=load, address=addr, out=out);`            |
| RAM512   | `RAM512(in=in, load=load, address=addr, out=out);`           |
| RAM4k    | `RAM4k(in=i, load=load, address=addr, out=out);`             |
| RAM16k   | `RAM16k(in=in, load=load, address=addr, out=out);`           |
| PC       | `PC(in=in, load=load, inc=increment, reset=reset, out=out);` |

#### hdl Combinational-chips

| Snippet   | Body                                                                                                                               |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| HalfAdder | `HalfAdder(a=a, b=b, out=out, carry=carry);`                                                                                       |
| FullAdder | `FullAdder(a=a, b=b, cin=cin, sum=sum, carry=carry);`                                                                              |
| Add16     | `Add16(a=a, b=b, out=out);`                                                                                                        |
| Inc16     | `Inc16(in=in, out=out);`                                                                                                           |
| ALU       | `ALU(x=inputX, y=inputY, zx=zeroX, nx=negateX, ny=negateY, f=AddOrAddition, no=negateOut, out=out, zr=outIsZero, ng=OutNegitive);` |
| ROM32     | `ROM32K(address=addr, out=out);`                                                                                                   |

#### hdl Computer-Architecture

| Snippet  | Body                                                                                                                     |
| -------- | ------------------------------------------------------------------------------------------------------------------------ |
| Memory   | `Memory(in=in, load=load, address=addr, outout);`                                                                        |
| CPU      | `CPU(inM=inM, instruction=ins, reset=reset, outM=out, writeM=outwriteIntoM, addressM=outAddrM, pc=outPc);`               |
| Computer | `Computer(inM=inM, instruction=instruction, reset=reset, outM=outM, writeM=outwriteIntoM, addressM=outAddrM, pc=outPc);` |

#### tst Snippets

| Snippet                       | Body                                                                                       |
| ----------------------------- | ------------------------------------------------------------------------------------------ |
| base                          | `load ${1:ChipName}.hdl,` `output-file ${1:ChipName}.out,`                                 |
| base                          | `load ${1:ChipName}.hdl,` `output-file ${1:ChipName}.out,` `compare-to ${1:ChipnNme}.cmp,` |
| output-list-2var              | `output-list a, b, out;`                                                                   |
| output-list-3var              | `output-list a, b, c, out;`                                                                |
| var00 (has all combinations)  | `set a 0,` `set b 0,` `eval,` `output;`                                                    |
| var000 (has all combinations) | `set a 0,` `set b 0,` `set c 0,` `eval,` `output;`                                         |

### cmp Snippets

| Snippet  | Body             |
| -------- | ---------------- |
| Row-2    | ` 0 0`           |
| Row-3    | ` 0 0 0`         |
| Row-4    | ` 0 0 0 0`       |
| Row-5    | ` 0 0 0 0 0`     |
| Row-6    | ` 0 0 0 0 0 0`   |
| Head-2   | ` a b out`       |
| Head-3   | ` a b c out`     |
| Head-4   | ` a b c d out`   |
| Head-2-2 | ` a b out out`   |
| Head-2-2 | ` a b c out out` |

`Table-2`

```
| a | b |out|
| 0 | 0 | 0 |
| 0 | 0 | 0 |
| 0 | 0 | 0 |
| 0 | 0 | 0 |
```

`Table-3`

```
| a | b | c |out|
| 0 | 0 | 0 | 0 |
| 0 | 0 | 0 | 0 |
| 0 | 0 | 0 | 0 |
| 0 | 0 | 0 | 0 |
```

`Table-2-2`

```
| a | b |out|out|
| 0 | 0 | 0 | 0 |
| 0 | 0 | 0 | 0 |
| 0 | 0 | 0 | 0 |
| 0 | 0 | 0 | 0 |
```

`Table-3-2`

```
| a | b | c |out|out|
| 0 |0 | 0 | 0 | 0 |
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 0 | 0 | 0 |
| 0 | 0 | 0 | 0 | 0 |
```

### language support

- add lanuage support for hdl, tst, cmp and out.

### 0.0.4

- Updated README

### 0.0.3

- added icon

### 0.0.2

- fixed snippets for hdl
- Updated README

### 0.0.1

Initial release of nand2tetris snippets.

- adds the initial snippest for all supported files.
- add syntax highlighting for all supported files.
- adds language support for hdl, cmp, out and tst

### Contributing

This is an opne source project, open to any one. Contributions are welcome [github](https://github.com/lukeJEdwards/nand2tetris-snippets)

If you are contributing a snippet, please be sure to add the documentation for it in the tables in the README, the pull request cannot be accepted without this addition. Thanks!
