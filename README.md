### Platanus v1.2.1 description ###

Platanus is a novel de novo sequence assembler that can reconstruct genomic sequences of
highly heterozygous diploids from massively parallel shotgun sequencing data.

http://platanus.bio.titech.ac.jp/

### Run platanus tools help###

docker run -it --rm cmonjeau/platanus Platanus
docker run -it --rm cmonjeau/platanus Platanus_trim
docker run -it --rm cmonjeau/platanus platanus_internal_trim

### Run platanus using Godocker (http://www.genouest.org/godocker/)

Create a new job with these parameters:

"Container image" : cmonjeau/platanus

"Command" : 

```

#!/bin/bash

# command line example (adapt with your data)
Platanus assemble –o Pxut –f $GODOCKER_HOME/DRR02167[34]_[12].fastq –t 16 –m 128 2> assemble.log

```

"Mount volumes" : home(rw)


