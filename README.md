# HLTool
Parsing and getting information from CMS HLT config dump hopefully made easy.

    Usage: hltool [options] <HLT config dump>
    
    Print HLT sequences and modules used by a given HLT path, with optionable
    expansion of their configuration parameters. The HLT config dump can be
    obtained as per instructions in https://cern.ch/go/T6Wc .
    
    Options:
      --version             show program's version number and exit
      -h, --help            show this help message and exit
      -p PATH, --path=PATH  only expand path containing the string PATH (exclusive
                            with -s) [default: ]
      -l, --list            only list paths and do not expand them [default:
                            False]
      -s SEQ, --seq=SEQ     only expand sequence SEQ (exclusive with -p) [default:
                            none]
      -m MOD, --module=MOD  only print configuration for module MOD (implies -c)
                            [default: none]
      -c, --cfg             also print module configurations [default: False]
      -i IND, --ind=IND     indentation string [default: `    ']
