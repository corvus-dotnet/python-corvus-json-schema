# python-corvus-json-schema

A [Bowtie](https://github.com/bowtie-json-schema/bowtie) test harness for
[corvus-json-schema](https://pypi.org/project/corvus-json-schema/), the pure-Python evaluator of
[Corvus.JsonSchema](https://github.com/corvus-dotnet/Corvus.JsonSchema).

Its image is published to `ghcr.io/bowtie-json-schema/python-corvus-json-schema` and run via
`bowtie run -i python-corvus-json-schema`.

The harness compiles each case's schema with the case's `registry` as the document resolver and validates each
instance. For `annotations` output it evaluates through a verbose results collector and reports each annotation with
its instance location and `#…` keyword location.

The image installs the latest release from PyPI; the `IMPLEMENTATION_VERSION` build argument pins another.
