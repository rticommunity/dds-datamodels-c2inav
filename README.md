# dds-datamodels-c2inav

This repository contains the OMG® C2INAV 1.2 beta 1 datamodel
https://www.omg.org/spec/C2INAV/1.2/Beta1

## Repo Organization

### Versioning & Branches

This repository stores different versions of the OMG® C2INAV datamodel in
different branches. Additionally, it contains `enhanced` versions of the
original datamodel. This enhanced versions modifies the original datamodel
including the latest IDL features and other potential improvements. The
different changes are explained in their own readme file.

The branches in this repo follow this pattern:

 - main: this contains the latest enhanced version
 - version/x.y\[-(version_specifier)\]\[-enhanced\]

For example, `version/2.0-beta-enhanced`

The `version_specifier` is added if a non-final version is being used. This
information appears in the datamodel website.

The `-enhanced` indicates that it contains the enhanced version of the specified
datamodel version.

### Folders

This repository contains one folder called `datamodel` that contains the
representation of this datamodel. Internally, that folder contains the different
files that implement the datamodel. It must contain an `idl` folder that
includes the IDL files of the datamodel. Additionally, other folders with the
name of the technology used for the representation of the datamodel may be
present. For example: `xml`, `json`...

Additionally, this repository contains a `dependencies` folder that includes
the datamodels that this repository depends on as git submodules.
