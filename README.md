# Pandoc Templates

A collection of custom pandoc templates i use on the reg. They are highly specialized so don't expect to just apply them anywhere without changing them.

## Using the templates

To use a template simply specify this in the *pandoc* command by adding:
```sh
--template path/to/the-template.tex
```
which i would recommend doing automatically by placing this in a `Makefile` or script.

> See for instance my [python conversion script](https://github.com/sutne/scripts/blob/main/bin/convert) where i can specify the template in the markdown YAML metadata (as it is done in the demo-files).

An alternative would be placing the template in a *pandoc data dir*.

## pandoc-crossref
This makes it super easy to refer to figure, tables etc. from anywhere else in the document.

See the [demo/assignment.md](demo/assignment.md) for examples on how to create and refer to figures, tables etc.

> When using raw markdown floats/figures/tables etc. its important that the `\label{tbl:label}` is placed at the **end** of the float (again see [demo/assignment.md](demo/assignment.md)).
