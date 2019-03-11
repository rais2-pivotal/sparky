# Pointers when converting data types from Teradata to Presto

### Specifications for table syntax
- NO FALLBACK: Specific to Teradata, not applicable in Presto. For Maintaining Replica of the TD table
- NO AFTER JOURNAL: Specific to Teradata, not applicable in Presto. For rollback operation
- CHECKSUM = DEFAULT: Specific to Teradata. not applicable in Presto.
- DEFAULT MERGEBLOCKRATIO: Specific to Teradata. not applicable in Presto.
- CASESPECIFIC: Specific to Teradata. Specifies if column/attribute is Case sensitive
- NOT CASESPECIFIC: Specific to Teradata. Specifies if column/attribute is Case insensitive
- COMPRESS ('1','9'): Specific to Teradata. To save space by using compression for fixed length columns
- DECOMPRESS ('1','9'): Opposite of Compress !!


### Types 

#### DATE
TD: BUSINESS_DATE DATE FORMAT 'YYYY-MM-DD' 
Presto: BUSINESS_DATE DATE FORMAT '%Y-%m-%d' 

#### Characters
TD: VARCHAR/CHAR
Presto: VARCHAR/CHAR

#### Numbers
TD: DECIMAL
Presto: DECIMAL



