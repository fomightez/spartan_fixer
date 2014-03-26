SPARTAN_FIXER
=============

SPARTAN08_Fixer is a program that fixes single chain Spartan'08 output
files in so-called PDB format, converting them to be true PDB format.
The fixed files can then easily be used in Jmol.

## Features :

 - Available in webserver form so no installation needed
 - command line version allows single files or entire folders of PDB files to be converted automagically.
 - conforms to PDB format as described [here][2] and [here][3]

##Webserver
[fomightez.pythonanywhere.com/spartan_fixer/][webserver]


## Usage :

###MANUAL/HELP OPTION

$ `python SPARTAN08_Fixer.py --help`



    usage: SPARTAN08_Fixer.py [-h] [--ChainDesig X] [--StartNo Y] [-a] InputData

    SPARTAN08_Fixer is a program that fixes single chain Spartan'08 output
    files in so-called PDB format, converting them to be true PDB format.
    The fixed files can then easily be used in Jmol.

    Written by Wayne Decatur --> Fomightez @ Github or Twitter.

    PDB format specification info:
    http://www.wwpdb.org/docs.html and http://deposit.rcsb.org/adit/docs/pdb_atom_format.html



    Actual example what to enter on command line to run program:
    python SPARTAN_FIXER input_file.pdb



    positional arguments:
      InputData       name of Spartan data file that will be fixed. REQUIRED.
                      Files entered this way do not have any requirement for specific extension as long
                      they are SPARTAN so-called PDB formatted-data.

                      The required input data can also be a group of files ending in '.pdb' (case does not matter)
                      contained within a folder. In that case put the folder as the input data.

    optional arguments:
      -h, --help      show this help message and exit
      --ChainDesig X  Enter in place of 'X' an alphanumeric character
                      to use as chain designation, or enter when prompted
      --StartNo Y     Enter in place of 'Y' a number in the range 1 to 9999
                      to be the first residue sequence number
                      for the output, or enter when prompted
      -a, --auto      Run without further prompts for user action, using chain
                      designation and starting residue on command line or
                      the defaults of 'A' and '1', respectively, for
                      those values if none provided.

### typical examples


## Development
Developed by Wayne Decatur in collaboration with Nick Greeves and Rui Li.

[home]: https://github.com/fomightez/spartan_fixer
[webserver]: http://fomightez.pythonanywhere.com/spartan_fixer/
[2]: http://deposit.rcsb.org/adit/docs/pdb_atom_format.html
[3]: http://www.wwpdb.org/documentation/format33/sect9.html#ATOM
