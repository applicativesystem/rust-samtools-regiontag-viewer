# rust-samtools-regiontag-viewer

- rust samtools regiontag-viewer 
- given an sam alignment file and a give range of the coordinate from the genome, will produce a base colour encoded alignment for the reads aligned in that region. 
- Especially important for showing the reads specific to diversity and phenotypes and linked mutations. 
- general note: Incase of Golang and RUST, please see the last commit message and if it says compiled binary then it is completed or else still in development version.
- This feature is not present in samtools. 

![](https://github.com/applicativesystem/rust-samtools-regiontag-viewer/blob/main/rust-samtools-region-viewer-additional.png)

```
cargo build
```

```
λ gauravsablok rust-samtools-regiontag-viewer → λ git main* → ./rust-samtools-regiontag-viewer -h
Usage: rust-samtools-regiontag-viewer <ALIGNMENT_ARG> <GENOME_START> <GENOME_END>

Arguments:
  <ALIGNMENT_ARG>  please provide the path to the alignment file
  <GENOME_START>   please provide the genome capture region start
  <GENOME_END>     please provide the genome capture region end

Options:
  -h, --help     Print help
  -V, --version  Print version

```
```
./rust-samtools-regiontag-viewer ./sample-files/Col0_C1.100k.sam 3654 3804 
./rust-samtools-regiontag-viewer ./sample-files/alignreads-metagenomics.sam 40 60
```

Gaurav Sablok
