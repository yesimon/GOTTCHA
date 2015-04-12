Column                             | Description
---------------------------------- | -----------------------------------------------------------
RANKNAME                           | (REPLICON)  = replicon name (source + plasmid/chr)<br>(STRAIN)    = strain name<br>(SPECIES)   = species name<br>(GENUS)     = genus name<br>...
NUM_SUBRANKS                       | = no. of distinct subranks for the current rank<br>(E.g.  the no. of SPECIES under the current GENUS)
GPROJ_ENTRIES                      | = no. of genome projects (i.e. STRAINS) under this RANK NAME
LINEAR_LENGTH                      | = N/O_LENGTH<br>= non-overlapping length <br>= no. of non-overlapping bases covering the unique DB
UNIQUE_DB_LENGTH                   | = no. of unique bases for this organism
FULL_REFDB_LENGTH                  | = no. of bases in full reference
LINEAR_COV                         | = LINEAR_LENGTH / UNIQUE_DB_LENGTH
HIT_COUNT                          | = no. of hits recruited to genome
HIT_COUNT_PLASMID                  | = no. of hits recruited to plasmid
READ_COUNT                         | = no. of reads recruited to genome
FULL_HIT_COUNT                     | = no. of full-length read hits recruited to genome
TOTAL_BP_MAPPED                    | = sum total of all hit lengths recruited to genome<br>= hit1.length + hit2.length + ... hitX.length<br>[formerly FOLD_COV_UNIQUE_SAMPLE]
LINEAR_DOC                         | = linear depth-of-coverage<br>= fold coverage of sample's LINEAR_LENGTH <br>= TOTAL_BP_MAPPED / LINEAR_LENGTH<br>[formerly FOLD_COV_UNIQUE_REFDB]
UREF_DOC                           | = unique reference's depth-of-coverage<br>= fold coverage of reference's UNIQUE_DB_LENGTH<br>= TOTAL_BP_MAPPED / UNIQUE_DB_LENGTH
UREF_CMAX                          | = MAX COVERAGE OF REFDB POSSIBLE, GIVEN SAMPLE INPUT BASES<br>= Cmax = L0/l0 <br>= TOTAL_INPUT_BASES / UNIQUE_DB_LENGTH
FRAC_HITS_POSSIBLE                 | = HIT_COUNT / TOTAL_INPUT_READS
FRAC_BASES_POSSIBLE                | = TOTAL_BP_MAPPED / TOTAL_INPUT_BASES
MEAN_HIT_LENGTH                    | = TOTAL_BP_MAPPED / HIT_COUNT
MEAN_LINEAR_HIT_LENGTH             | = LINEAR_LENGTH / HIT_COUNT
best_SUBRANK                       | = name of the best subrank (determined by the highest LINEAR_COV)
best_NUM_SUBRANKS                  | = no. of subranks supporting current "SUBRANK"<br>{SS} = no. of GI entries supporting this strain<br>{S}  = no. of strains supporting this species<br>{G}  = no. of species supporting this genus<br>{F}  = no. of genera supporting this family<br>{O}  = no. of families supporting this order <br>{C}  = no. of orders supporting this class<br>{P}  = no. of classes supporting this phylum
best_GPROJ_ENTRIES                 | = no. of genome projects (i.e. STRAINS) under this best_SUBRANK<br>{SS} = no. of genome projects supporting this strain = 1<br>{S}  = no. of genome projects supporting this species<br>{G}  = no. of genome projects supporting this genus<br>{F}  = no. of genome projects supporting this family<br>{O}  = no. of genome projects supporting this order<br>{C}  = no. of genome projects supporting this class<br>{P}  = no. of genome projects supporting this phylum
best_LINEAR_LENGTH                 |
best_UNIQUE_DB_LENGTH              |
best_FULL_REFDB_LENGTH             |
best_LINEAR_COV                    |
best_HIT_COUNT                     |
best_FULL_HIT_COUNT                |
best_TOTAL_BP_MAPPED               |
best_LINEAR_DOC (a.k.a. Abundance) |
best_UREF_DOC                      |
best_UREF_CMAX                     |
best_FRAC_HITS_POSSIBLE            |
best_FRAC_BASES_POSSIBLE           |
best_MEAN_HIT_LENGTH               |
best_MEAN_LINEAR_HIT_LENGTH        |
CONTIG_COUNT                       |  = No. of contiguous fragments<br> (after mapping & generating non-overlapping fragments)
CONTIG_MEAN_LEN                    |  = Mean length of contigs (bp)
CONTIG_STDEV_LEN                   |  = Standard deviation of contig lengths (bp)
CONTIG_MINLEN                      |  = Length of smallest contig
CONTIG_MAXLEN                      |  = Length of largest contig
CONTIG_HISTOGRAM(LEN:FREQ)         |  = Contig Length Histogram<br> (in the format contigLength:frequency)
