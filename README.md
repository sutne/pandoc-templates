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

Because i hate having duplicate code/styling, i have placed as much as possible in the `master.sty` file, all the other templates "inherit" the styles defined here to keep things consistant, if the template need to, these styles/options can just be overwritten.

### All optional yaml arguments:

Arguments without a default value will not appear in the document unless specified. To give a list as argument the following syntax is used:

```yaml
key:
- Value 1
- Value 2
- Value 3
```

#### Assignment

| key             | type(s)               | default value |
|:----------------|:----------------------|:-------------:|
| `toc-depth`     | Number                |       2       |
| `sec-num-depth` | Number                |       4       |
| `date`          | String                |   `\today`    |
| `author`        | String / List[String] |  Sivert Utne  |
| `subjectcode`   | String / Number       |               |
| `subjectname`   | String                |               |
| `assignment`    | Number                |               |
| `title`         | String                |               |

#### Report

| key             | type(s)               | default value |
|:----------------|:----------------------|:-------------:|
| `toc-depth`     | Number                |       3       |
| `sec-num-depth` | Number                |       4       |
| `date`          | String                |   `\today`    |
| `author`        | String / List[String] |  Sivert Utne  |
| `subjectcode`   | String / Number       |               |
| `subjectname`   | String                |               |
| `supertitle`    | String                |    Report     |
| `title`         | String                |               |

## pandoc-crossref
This makes it super easy to refer to figure, tables etc. from anywhere else in the document.

See the [demo/assignment.md](demo/assignment.md) for examples on how to create and refer to figures, tables etc.

> When using raw markdown floats/figures/tables etc. its important that the `\label{tbl:label}` is placed at the **end** of the float (again see [demo/assignment.md](demo/assignment.md)).
