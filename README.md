# Merge VCFs workflow
Merge individual sample VCFs to create a unified multi-sample VCF, optionally allowing for modification of sample names.

## Input considerations
* List of VCF file paths. If the VCFs are not sorted, use `SORT_VCFS: true`.
* List of new sample names for each input VCF in the order they appear in the VCFs list. (OPTIONAL)
* Group name after merging used in the output filenames. Default - "samples" (OPTIONAL)
* Should the input VCFs be sorted? Default is "false" (OPTIONAL)

## Test locally
```
miniwdl run --as-me -i test.inputs.default.json workflow.wdl
miniwdl run --as-me -i test.inputs.options.json workflow.wdl
```
