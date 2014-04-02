# IPCC Parse
Parse and convert data for IPCC tool from CSV to JSON

## Languages

* XSLT
* Ant
* Shell

## Included Software

* Saxon XSLT Processor

## Requirements

* Java
* Ant
* ipcc-acquire project at the same level
* 'giec' MySQL database (to generate TSV files in ipcc-acquire)
* ipcc.projetmedea.fr project at the same level

## Configuration

The relative path to the projects ipcc-acquire and ipcc.projetmedea.fr
are configured in variables at the start of the script parse.sh.

## Run

    # run test transformation (possibly customized in ant/user.properties)
    $ ant -f ant/parse.xml

    # convert output data from ipcc-acquire and export to ipcc.projetmedea.fr
    $ parse.sh
