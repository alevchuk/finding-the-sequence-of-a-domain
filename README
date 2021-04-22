# finding-the-sequence-of-a-domain

This incredibly useful set of scripts were first described here over ten years ago:

https://www.biostars.org/p/10185/

HMMER3 and blast+ went through substantial updates, so after some considerable tinkering, I have managed to update a working set of scripts.
The extract sequence script was also updated as suggested by @alevchuk here: https://www.biostars.org/p/10220/#10221

## Usage

### git clone the repository & copy in your desired fasta file

```
git clone https://github.com/maltesemike/finding-the-sequence-of-a-domain.git
chmod +x 00*
cp my.fasta ./
```

### download the Pfam database & prepare it - this step required HMMER 3

```
./001-download-data
./002-prepare-hmm
```

### grep the hmm file to find the precise Pfam domain id ex. PF00145 is PF00145.19
```
grep PF00145 Pfam-A.hmm
```

### scan your fasta for your Pfam domain, extract co-ordinates and then the sequences. lovely!
```
./003-scan my.fasta PF00145.19
./004-extract-coords my.fasta.PF00145.19.scan.tab
./005-extract-seq my.fasta
```
