# Bam/bai file extraction from NCBI

Download Genome Workbench at http://archive-dtd.ncbi.nlm.nih.gov/projects/gbench/download.html

**BAM DATA FROM SRA RUN ACCESSION** 
1. Access https://www.ncbi.nlm.nih.gov/
2. From the databases dropdown menu select 'SRA'
3. Insert the query ("SARS-CoV-2"[Organism]) AND “aligned data"[Properties] **N.B. Run accessions from the SRA database can be visualized in Genome Workbench if they are aligned to a GenBank or RefSeq sequence.'**
4. Copy the SRA run accession (e.g. ERX5938278)
5. On Genome Workbench select *File* > *Open* > *BAM/CSRA files* 
6. Paste copied SRA run accession
7. Click *Next* and see the GenBank accession of the BAM file detected by Genome Workbench 
8. Click *Next* > *Finish*
9. A new project has been created

# Bam/bai file extraction from ENA
1. Access https://www.ebi.ac.uk/ena/browser/home
2. Download https://github.com/enasequence/enaBrowserTools **needs python installed**
3.
**For data-holding accessions such as Sequence records, Assembly records, Run or Analysis records or WGS sets**
>Enter: >enaDataGet -f fastq -d <destination/directory> *e.g. run accession from ENA*

**To download all data files of a certain type of Record that are associated with a Study, Sample or given Taxon**
>Enter: >enaGroupGet -f submitted -d <destination/directory> *e.g. sample accession*

4. Convert file from fastq to bam using https://sequencing.com/fastq2bam-conversion
