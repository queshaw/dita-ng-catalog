# DITA-NG Relax NG XML catalog

This is an example catalog that can be used with dita-ng-library.

## Installation

The *dita* command included in DITA-OT versions 2.0 or greater can be used to install the plugin, e.g.:


```
x:\dita-ot\bin\dita -install dist\org.not-oasis-open.dita.v1_3-cs01-20150916.zip -v
```

## Testing the installation

Processing the DITA specification is one way to test the catalog:

```
cd x:\dita-ot
set demo_dir=x:\dita-ot\plugins\org.not-oasis-open.dita.v1_3-cs01\demo\dita-1.3-specification
set ditamap=%demo_dir%\dita-1.3-specification-learningTraining.ditamap
set ditaval=%demo_dir%\resources\DITA1.3-spec-learningTraining.ditaval
bin\dita -v -f xhtml -i %ditamap% -f %ditaval -o out
out\index.html
```

There is also a smaller DITA document to use as an example in:

```
demo\flowers
```
