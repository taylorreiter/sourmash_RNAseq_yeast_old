The SRA toolkit was downloaded and installed, and caching was disabled. Then, files that I had not downloaded for previous analysis were added.
```
for accession in ERR458585 ERR458586 ERR458835 ERR458587 ERR459011 ERR458588 ERR459012 ERR458589 ERR459013 ERR458590 ERR459014 ERR458829 ERR459015 ERR458830 ERR459016 ERR458831 ERR459017 ERR458832	
  do
    fastq-dump --defline-seq '@$sn[_$rn]/$ri' -A $accession --gzip
done
```
