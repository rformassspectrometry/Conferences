# Talk about `Spectra` and backend functionality

Laurent Gatto, Johannes Rainer, Sebastian Gibb<sup>1</sup>

## Title

Flexible infrastructure for mass spectrometry data

## Abstract

Mass spectrometry (MS) data consists mainly of either mass-to-charge (m/z) and
intensity data pairs or retention time - intensity pairs enriched with
additional metadata information. MS instruments store such data in
vendor-specific formats which have to be converted to the open file formats mzML
or mzXML for data transfer and import. In addition, MS data from spectral
libraries or online annotation resources are usually stored and provided in a
variety of different file formats ranging from the *standard* mgf file format to
custom text-based file formats.

Learning from experiences gained in the `MSnbase` and `xcms` Bioconductor
packages we implemeted the new `Spectra` package that provides a common,
flexible and a high-performance infrastructure to represent and handle MS data
in R. The introduction of dedicated *backend* classes makes the main `Spectra`
object independent of the origin and storage of the data. Depending on the
backend used, MS data can be kept in memory for fast processing, or retrieved
from disk on demand for a low memory footprint hence enabling the analysis of
large MS data sets. Backends interfacing directly SQL based spectral libraries
can in future facilitate the comparison of spectral data from experiments with
reference spectra for annotation purposes.

<sup>1</sup>The order of authors was defined by the `sample` function with a
random seed of `42`.
