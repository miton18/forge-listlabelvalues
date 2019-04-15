# ListLabelValues

> labels

Return a list of all unique label values of a GTS list

## Getting started / Usage

To get started with ListLabelValues, the easiest way is to go on Quantum and follow the following instructions.

```warpscript
'ListLabelValues' FIMPORT

// Let's get some timeseries
[
  NEWGTS { 'host' 'a' } RELABEL
  NEWGTS { 'host' 'b' } RELABEL
  NEWGTS { 'host' 'b' } RELABEL
  NEWGTS {            } RELABEL
]

// put the interesting label
'host'

// Call the macro !
@ListLabelValues
```

There is a list of Time series with twice time the `b` host, and one without `host` value.
We will get the list of unique hosts, so: `a` & `b`

## Issues

Just open a new issue on [macro Github repository](https://github.com/miton18/forge-ListLabelValues)

## Licensing

The code in this project is licensed under MIT license.
