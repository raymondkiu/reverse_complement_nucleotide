#!/bin/bash
if [ $# -lt 1 ] ; then
    echo ""
    echo "usage: reverse_complement_nucleotide.sh *.fna ..|| *.fa pr *.fna or *.fasta"
    echo "complement nucleotide fasta files"
    echo ""
    exit 0
fi

filear=${@};
for i in ${filear[@]}

do

cat $i | while read L; do echo $L; read L; echo "$L" | tr "ATGC" "TACG"|tr "atgc" "tacg" ; done > $i-complement.fasta

done
