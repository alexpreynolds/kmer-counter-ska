# kmer-counter-ska

The `kfs` program reads in multiline FASTA records, counts canonical kmers using Malte Skarupke's [`bytell_hash_map` hash table](https://probablydance.com/2018/05/28/a-new-fast-hash-table-in-response-to-googles-new-fast-hash-table/), and measures time taken to read in and process records.

## Usage

### Compilation

```
$ make kfs
```

### Performance

Specify variables `K` (integer) and `FASTA` (path to FASTA sequences).

```
$ /usr/bin/time -l ./kfs -k ${K} -i ${FASTA}
...
```
