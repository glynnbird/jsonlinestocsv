# jsonlinestocsv

The _jsonlinestocsv_ utility (or its alias `jsonltocsv`) converts a stream of JSON documents (one per line) from stdin to a CSV file on stdout.

It suits JSON documents that are uniform with the same number and names of attributes per document. The first document found is used as the template for column names.

## Installation

```sh
npm install -g jsonlinestocsv
```

## Usage

Simply pipe your stream of data into `jsonltocsv`:

```sh
cat cities.json | jsonltocsv

_id,name,latitude,longitude,country,population,timezone
771158,Hajnówka,52.74328,23.58122,PL,22157,Europe/Warsaw
733840,Xánthi,41.13488,24.888,GR,48221,Europe/Athens
694216,Shepetivka,50.18545,27.06365,UA,46419,Europe/Kiev
7626461,Yaren,-0.55085,166.9252,NR,1100,Pacific/Nauru
771401,Grodzisk Mazowiecki,52.10387,20.6337,PL,26684,Europe/Warsaw
763111,Opoczno,51.37569,20.27827,PL,22592,Europe/Warsaw
6945291,Old City,31.77667,35.23417,PS,36000,Asia/Hebron
734643,Pylaía,40.59918,22.98613,GR,23494,Europe/Athens
982899,Lichtenburg,-26.152,26.15968,ZA,65863,Africa/Johannesburg
```
