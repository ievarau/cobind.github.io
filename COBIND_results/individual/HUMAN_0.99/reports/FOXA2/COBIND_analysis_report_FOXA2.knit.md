---
date: "Date: 2022-06-08"
output:
  html_document:
      pandoc_args: ["+RTS", "-K10000m","-RTS"]
      toc: true
      toc_depth: 3
      toc_float: true
      theme: cerulean
geometry: margin = 2cm

---




---
title: FOXA2
subtitle: "COBIND analysis report"
---

<p>&nbsp;</p>

<div align = "justify">
These are the results produced by the COBIND pipeline, which looks for sequence patterns in the neighbourhoods of the reference regions.
</div>

<p>&nbsp;</p>

# Spacings summary

## Summary in a plot

<div align = "justify">
Spacing summary plot describes the relationship between the anchor (in the center) and discovered co-binder motif (on the right). The squares show the spacing between the anchor and co-binder motifs that are displayed. The color of the square indicated the number of datasets this configuration is found in, while the the number inside indicates the proportion of input sequences this configuration was found in.
</div>

<p>&nbsp;</p>



<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/spacing-summary-plot-1.png" alt="**Figure 1. Spacings summary plot **" width="8208" />
<p class="caption">**Figure 1. Spacings summary plot **</p>
</div>

<p>&nbsp;</p>

## Summary in a table

<div align = "justify">
The spacing summary table consists of all details from co-binder motif discovery. This includes the datasets where the co-binders were found, the NMF details, number of regions in the input file and the fraction of those regions where the co-binder was found. Last columns summarizes the fraction of regions with the co-binder with specific spacer and location.
</div>

<p>&nbsp;</p>
<p>&nbsp;</p>

<!--html_preserve--><a href="data:text/csv;base64,U3ViY2x1c3RlcjtEYXRhc2V0O0ZsYW5rO05iX2NvbXBvbmVudHM7Q29tcG9uZW50O1NwYWNlcl9sZW5ndGg7TG9jYXRpb247TmJfcmVnaW9uc19pbl9pbnB1dF9iZWQ7TmJfcmVnaW9uc193aXRoX2NvYmluZGVyO0ZyYWN0aW9uX29mX3JlZ2lvbnNfd2l0aF9jb2JpbmRlcjtOYl9kYXRhc2V0cztDb2JpbmRlcl9wcm9wb3J0aW9uClN1YmNsdXN0ZXJfMDtIU19EMjg1OF9DMjQ4X0oyMl9UNTdfRk9YQTI7bGVmdDs0X2NvbXBvbmVudHM7MTsgMztsZWZ0OyA4Mjk3OTsgNjQ4OzAsMDA4OzM7MCwwMjAKU3ViY2x1c3Rlcl8wO0hTX0QyODYyX0MzNF9KMjJfVDU3X0ZPWEEyO2xlZnQ7NV9jb21wb25lbnRzOzM7IDM7bGVmdDsxMTc1NTM7MjExNDswLDAxODszOzAsMDIwClN1YmNsdXN0ZXJfMDtIU19EMjg4Nl9DMzRfSjIyX1Q1N19GT1hBMjtsZWZ0OzVfY29tcG9uZW50czs0OyAzO2xlZnQ7IDc5NDAwOzEwNDA7MCwwMTM7MzswLDAyMApTdWJjbHVzdGVyXzA7SFNfRDI4NTdfQzI0OF9KMjJfVDU3X0ZPWEEyO2xlZnQ7NV9jb21wb25lbnRzOzM7IDY7bGVmdDsxMTIyMjE7MjExNDswLDAxOTsyOzAsMDEzClN1YmNsdXN0ZXJfMDtIU19EMjg4OF9DMzRfSjIyX1Q1N19GT1hBMjtsZWZ0OzRfY29tcG9uZW50czsxOyA2O2xlZnQ7IDE5NjQxOyAxNzE7MCwwMDk7MjswLDAxMwpTdWJjbHVzdGVyXzA7SFNfRDI4ODhfQzM0X0oyMl9UNTdfRk9YQTI7bGVmdDs1X2NvbXBvbmVudHM7MzsgNjtsZWZ0OyAxOTY0MTsgMzY2OzAsMDE5OzI7MCwwMTMKU3ViY2x1c3Rlcl8wO0hTX0QyODg3X0MzNF9KMjJfVDU3X0ZPWEEyO2xlZnQ7Nl9jb21wb25lbnRzOzM7MTI7bGVmdDsgNzQ0ODc7IDUyNjswLDAwNzsxOzAsMDA5ClN1YmNsdXN0ZXJfMDtIU19EMjg1N19DMjQ4X0oyMl9UNTdfRk9YQTI7bGVmdDs1X2NvbXBvbmVudHM7MjsxODtsZWZ0OzExMjIyMTsxMTg3OzAsMDExOzQ7MCwwMTIKU3ViY2x1c3Rlcl8wO0hTX0QyODYwX0MzNF9KMjJfVDU3X0ZPWEEyO2xlZnQ7NF9jb21wb25lbnRzOzI7MTg7bGVmdDsgNzMxMDY7IDU5OTswLDAwODs0OzAsMDEyClN1YmNsdXN0ZXJfMDtIU19EMjg2MV9DMzRfSjIyX1Q1N19GT1hBMjtsZWZ0OzZfY29tcG9uZW50czsyOzE4O2xlZnQ7IDYxNDg0OyA1OTU7MCwwMTA7NDswLDAxMgpTdWJjbHVzdGVyXzA7SFNfRDI4ODdfQzM0X0oyMl9UNTdfRk9YQTI7bGVmdDs0X2NvbXBvbmVudHM7MjsxODtsZWZ0OyA3NDQ4NzsgNjMxOzAsMDA4OzQ7MCwwMTIKU3ViY2x1c3Rlcl8wO0hTX0QyODg3X0MzNF9KMjJfVDU3X0ZPWEEyO2xlZnQ7NV9jb21wb25lbnRzOzI7MTg7bGVmdDsgNzQ0ODc7MTAxMjswLDAxNDs0OzAsMDEyClN1YmNsdXN0ZXJfMDtIU19EMjg2MF9DMzRfSjIyX1Q1N19GT1hBMjtyaWdodDs0X2NvbXBvbmVudHM7MjsgMjtyaWdodDsgNzMxMDY7IDY2OTswLDAwOTsyOzAsMDE2ClN1YmNsdXN0ZXJfMDtIU19EMjg2MF9DMzRfSjIyX1Q1N19GT1hBMjtyaWdodDs2X2NvbXBvbmVudHM7NDsgMjtyaWdodDsgNzMxMDY7IDg2MTswLDAxMjsyOzAsMDE2ClN1YmNsdXN0ZXJfMDtIU19EMjg2Ml9DMzRfSjIyX1Q1N19GT1hBMjtyaWdodDs2X2NvbXBvbmVudHM7NDsgMjtyaWdodDsxMTc1NTM7IDgzMjswLDAwNzsyOzAsMDE2ClN1YmNsdXN0ZXJfMDtIU19EMjg4OF9DMzRfSjIyX1Q1N19GT1hBMjtyaWdodDs0X2NvbXBvbmVudHM7MjsgNDtyaWdodDsgMTk2NDE7IDE3NzswLDAwOTsxOzAsMDA3ClN1YmNsdXN0ZXJfMDtIU19EMjg4N19DMzRfSjIyX1Q1N19GT1hBMjtyaWdodDs1X2NvbXBvbmVudHM7NDsxMDtyaWdodDsgNzQ0ODc7IDczNDswLDAxMDsxOzAsMDExClN1YmNsdXN0ZXJfMDtIU19EMjg1N19DMjQ4X0oyMl9UNTdfRk9YQTI7cmlnaHQ7NV9jb21wb25lbnRzOzQ7MTQ7cmlnaHQ7MTEyMjIxOzEyNzM7MCwwMTE7MjswLDAxMApTdWJjbHVzdGVyXzA7SFNfRDI4NjRfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7NV9jb21wb25lbnRzOzQ7MTQ7cmlnaHQ7MTA0MTk5OzE5MDg7MCwwMTg7MjswLDAxMApTdWJjbHVzdGVyXzA7SFNfRDU5MF9DMjYxX0oyMl9UNTdfRk9YQTI7cmlnaHQ7M19jb21wb25lbnRzOzE7MTU7cmlnaHQ7IDEyMzM3OyA0MTM7MCwwMzM7MTswLDAxNgpTdWJjbHVzdGVyXzA7SFNfRDI4NjBfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7Nl9jb21wb25lbnRzOzU7MTY7cmlnaHQ7IDczMTA2OyA4MDI7MCwwMTE7MjswLDAzNApTdWJjbHVzdGVyXzA7SFNfRDI4ODdfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7Nl9jb21wb25lbnRzOzA7MTY7cmlnaHQ7IDc0NDg3OyA5NDc7MCwwMTM7MjswLDAzNApTdWJjbHVzdGVyXzA7SFNfRDI4NjJfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7Nl9jb21wb25lbnRzOzA7MTg7cmlnaHQ7MTE3NTUzOzE0MDI7MCwwMTI7NDswLDAxNQpTdWJjbHVzdGVyXzA7SFNfRDI4NjdfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7NV9jb21wb25lbnRzOzA7MTg7cmlnaHQ7IDc4MTMyOyA5Nzc7MCwwMTM7NDswLDAxNQpTdWJjbHVzdGVyXzA7SFNfRDI4NjhfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7Nl9jb21wb25lbnRzOzA7MTg7cmlnaHQ7IDc5MDE5OyA5MDE7MCwwMTE7NDswLDAxNQpTdWJjbHVzdGVyXzA7SFNfRDI4ODVfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7NV9jb21wb25lbnRzOzA7MTg7cmlnaHQ7IDc3NjY1OyA5MTk7MCwwMTI7NDswLDAxNQpTdWJjbHVzdGVyXzA7SFNfRDI4ODVfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7Nl9jb21wb25lbnRzOzA7MTg7cmlnaHQ7IDc3NjY1OyA3NzY7MCwwMTA7NDswLDAxNQpTdWJjbHVzdGVyXzA7SFNfRDI4NjJfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7Nl9jb21wb25lbnRzOzE7MTk7cmlnaHQ7MTE3NTUzOyA5MzE7MCwwMDg7MTswLDAwOApTdWJjbHVzdGVyXzE7SFNfRDI4NjBfQzM0X0oyMl9UNTdfRk9YQTI7bGVmdDs2X2NvbXBvbmVudHM7MjsgMjtsZWZ0OyA3MzEwNjsxMjUxOzAsMDE3OzE7MCwwMTEKU3ViY2x1c3Rlcl8xO0hTX0QyODYyX0MzNF9KMjJfVDU3X0ZPWEEyO2xlZnQ7Nl9jb21wb25lbnRzOzU7MTU7bGVmdDsxMTc1NTM7IDg2ODswLDAwNzs1OzAsMDA0ClN1YmNsdXN0ZXJfMTtIU19EMjg2NF9DMzRfSjIyX1Q1N19GT1hBMjtsZWZ0OzVfY29tcG9uZW50czsxOzE1O2xlZnQ7MTA0MTk5OzEyODU7MCwwMTI7NTswLDAwNApTdWJjbHVzdGVyXzE7SFNfRDI4NjdfQzM0X0oyMl9UNTdfRk9YQTI7bGVmdDs2X2NvbXBvbmVudHM7MDsxNTtsZWZ0OyA3ODEzMjsgNjQ3OzAsMDA4OzU7MCwwMDQKU3ViY2x1c3Rlcl8xO0hTX0QyODg1X0MzNF9KMjJfVDU3X0ZPWEEyO2xlZnQ7Nl9jb21wb25lbnRzOzA7MTU7bGVmdDsgNzc2NjU7IDY0MzswLDAwODs1OzAsMDA0ClN1YmNsdXN0ZXJfMTtIU19EMjg4N19DMzRfSjIyX1Q1N19GT1hBMjtsZWZ0OzZfY29tcG9uZW50czsxOzE1O2xlZnQ7IDc0NDg3OyA1NjQ7MCwwMDg7NTswLDAwNApTdWJjbHVzdGVyXzE7SFNfRDI4NjBfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7NV9jb21wb25lbnRzOzE7IDI7cmlnaHQ7IDczMTA2OyA5MTE7MCwwMTI7MTswLDAxNwpTdWJjbHVzdGVyXzE7SFNfRDI4ODdfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7Nl9jb21wb25lbnRzOzI7IDk7cmlnaHQ7IDc0NDg3OyAzMjM7MCwwMDQ7MTswLDAxMgpTdWJjbHVzdGVyXzE7SFNfRDI4ODdfQzM0X0oyMl9UNTdfRk9YQTI7cmlnaHQ7NV9jb21wb25lbnRzOzI7MTU7cmlnaHQ7IDc0NDg3OyA3NDU7MCwwMTA7MTswLDAxMApTdWJjbHVzdGVyXzI7SFNfRDM4MDRfQzQ4X0oyMl9UNTdfRk9YQTI7bGVmdDs0X2NvbXBvbmVudHM7MTsgMjtsZWZ0OyAzNTY0MzsgNTQzOzAsMDE1OzM7MCwwNTcKU3ViY2x1c3Rlcl8yO0hTX0Q4NjZfQzM2Nl9KMjJfVDU3X0ZPWEEyO2xlZnQ7M19jb21wb25lbnRzOzE7IDI7bGVmdDsxNDY1NjQ7ODAzMDswLDA1NTszOzAsMDU3ClN1YmNsdXN0ZXJfMjtIU19EODY2X0MzNjZfSjIyX1Q1N19GT1hBMjtsZWZ0OzRfY29tcG9uZW50czsxOyAyO2xlZnQ7MTQ2NTY0OzIwOTU7MCwwMTQ7MzswLDA1NwpTdWJjbHVzdGVyXzI7SFNfRDg3MV9DMTY5X0oyMl9UNTdfRk9YQTI7bGVmdDszX2NvbXBvbmVudHM7MTsgMjtsZWZ0OzEzMDg2NTs1OTQ1OzAsMDQ1OzM7MCwwNTcKU3ViY2x1c3Rlcl8yO0hTX0Q4NzFfQzE2OV9KMjJfVDU3X0ZPWEEyO2xlZnQ7NF9jb21wb25lbnRzOzE7IDI7bGVmdDsxMzA4NjU7MTQ4MDswLDAxMTszOzAsMDU3ClN1YmNsdXN0ZXJfMjtIU19EODcxX0MxNjlfSjIyX1Q1N19GT1hBMjtsZWZ0OzZfY29tcG9uZW50czsxOyAyO2xlZnQ7MTMwODY1OyA3MTg7MCwwMDU7MzswLDA1NwpTdWJjbHVzdGVyXzM7SFNfRDE0MjVfQzIxN19KMjJfVDU3X0ZPWEEyO2xlZnQ7NF9jb21wb25lbnRzOzA7IDI7bGVmdDsgMjI0NDk7MTA5MTswLDA0OTs1OzAsMDIwClN1YmNsdXN0ZXJfMztIU19EMzgwNF9DNDhfSjIyX1Q1N19GT1hBMjtsZWZ0OzNfY29tcG9uZW50czsyOyAyO2xlZnQ7IDM1NjQzOyA5NjI7MCwwMjc7NTswLDAyMApTdWJjbHVzdGVyXzM7SFNfRDM4MDRfQzQ4X0oyMl9UNTdfRk9YQTI7bGVmdDs0X2NvbXBvbmVudHM7MDsgMjtsZWZ0OyAzNTY0MzsgMzc0OzAsMDEwOzU7MCwwMjAKU3ViY2x1c3Rlcl8zO0hTX0Q4NjZfQzM2Nl9KMjJfVDU3X0ZPWEEyO2xlZnQ7NF9jb21wb25lbnRzOzA7IDI7bGVmdDsxNDY1NjQ7MTE4ODswLDAwODs1OzAsMDIwClN1YmNsdXN0ZXJfMztIU19EODcxX0MxNjlfSjIyX1Q1N19GT1hBMjtsZWZ0OzRfY29tcG9uZW50czswOyAyO2xlZnQ7MTMwODY1OzEzODc7MCwwMTE7NTswLDAyMApTdWJjbHVzdGVyXzM7SFNfRDg3MV9DMTY5X0oyMl9UNTdfRk9YQTI7bGVmdDs2X2NvbXBvbmVudHM7NDsgMjtsZWZ0OzEzMDg2NTsgODU1OzAsMDA3OzU7MCwwMjAKU3ViY2x1c3Rlcl8zO0hTX0Q4ODZfQzM2NV9KMjJfVDU3X0ZPWEEyO2xlZnQ7M19jb21wb25lbnRzOzI7IDI7bGVmdDsgIDQ4NDA7IDMyMzswLDA2Nzs1OzAsMDIwClN1YmNsdXN0ZXJfNDtIU19EMTA5X0MxOTVfSjIyX1Q1N19GT1hBMjtsZWZ0OzRfY29tcG9uZW50czswOyAyO2xlZnQ7IDg3MTUwOzEwODU7MCwwMTI7NDswLDAyNgpTdWJjbHVzdGVyXzQ7SFNfRDE0MF9DMTBfSjIyX1Q1N19GT1hBMjtsZWZ0OzZfY29tcG9uZW50czsyOyAyO2xlZnQ7IDY5NTQ1OyA1MjU7MCwwMDg7NDswLDAyNgpTdWJjbHVzdGVyXzQ7SFNfRDI4NThfQzI0OF9KMjJfVDU3X0ZPWEEyO2xlZnQ7M19jb21wb25lbnRzOzI7IDI7bGVmdDsgODI5Nzk7MzM0MzswLDA0MDs0OzAsMDI2ClN1YmNsdXN0ZXJfNDtIU19EMjg2M19DMzRfSjIyX1Q1N19GT1hBMjtsZWZ0OzRfY29tcG9uZW50czsyOyAyO2xlZnQ7IDE4NjE3OyAzMzA7MCwwMTg7NDswLDAyNgpTdWJjbHVzdGVyXzU7SFNfRDEwNDZfQzI2MV9KMjJfVDU3X0ZPWEEyO2xlZnQ7M19jb21wb25lbnRzOzE7IDI7bGVmdDsgIDI5MDc7IDEwNjswLDAzNjsyOzAsMDIyClN1YmNsdXN0ZXJfNTtIU19EMTA0Nl9DMjYxX0oyMl9UNTdfRk9YQTI7bGVmdDs2X2NvbXBvbmVudHM7NDsgMjtsZWZ0OyAgMjkwNzsgIDQ3OzAsMDE2OzI7MCwwMjIKU3ViY2x1c3Rlcl81O0hTX0Q1OTBfQzI2MV9KMjJfVDU3X0ZPWEEyO2xlZnQ7NV9jb21wb25lbnRzOzA7IDI7bGVmdDsgMTIzMzc7ICA4MjswLDAwNzsyOzAsMDIyClN1YmNsdXN0ZXJfNTtIU19ENTkwX0MyNjFfSjIyX1Q1N19GT1hBMjtsZWZ0OzZfY29tcG9uZW50czs0OyAyO2xlZnQ7IDEyMzM3OyAgOTE7MCwwMDc7MjswLDAyMgpTdWJjbHVzdGVyXzY7SFNfRDg4NV9DMjYxX0oyMl9UNTdfRk9YQTI7bGVmdDs2X2NvbXBvbmVudHM7MDsgMjtsZWZ0OyAzMTE3ODsgNzA3OzAsMDIzOzE7MCwwMjMKU3ViY2x1c3Rlcl83O0hTX0QxNDI1X0MyMTdfSjIyX1Q1N19GT1hBMjtsZWZ0OzZfY29tcG9uZW50czswOyAyO2xlZnQ7IDIyNDQ5OyA0MTI7MCwwMTg7MTswLDAxOAo=" download="FOXA2_spacings_summary.csv">
<button class="btn btn-primary" has_icon="TRUE"><i class="fa fa-save"></i> Download table as csv</button>
</a><!--/html_preserve-->

<p>&nbsp;</p>

<!-- # Co-binder regions -->

<!-- <div align = "justify"> -->
<!-- The pipeline outputs a collection of genomic regions in BED format. Bellow is the list of regions that can be downloaded. -->
<!-- </div> -->

<!-- <p>&nbsp;</p> -->

<!-- ```{r co-binder-regions, cache = TRUE, echo = FALSE, eval = TRUE, include = TRUE} -->

<!-- ## Function: -->
<!-- download_button <- function(file_name, output_name) { -->

<!--   downloadthis::download_file(path = file_name, -->
<!--                               output_name = output_name, -->
<!--                               button_label = "Download BED", -->
<!--                               button_type = "default", -->
<!--                               has_icon = TRUE, -->
<!--                               icon = "fa fa-save", -->
<!--                               self_contained = FALSE) -->
<!--   } -->

<!-- ## Regions: -->
<!-- ### Anchors: -->
<!-- all.cobinder.anchors     <- file.path(cobinder.regions.dir, "anchors/containing_all_cobinders", -->
<!--                                       paste0("overlapping_cobinders_anchors_", family_name, ".bed")) -->
<!-- with.cobinder.anchors    <- list.files(file.path(cobinder.regions.dir, "anchors/with_cobinder_motif_specific", -->
<!--                                                  family_name), full.names = TRUE) -->
<!-- no.cobinder.anchors      <- list.files(file.path(cobinder.regions.dir, "anchors/no_cobinder_motif_specific", -->
<!--                                                  family_name), full.names = TRUE) -->
<!-- ### Full regions: -->
<!-- all.cobinder.full        <- file.path(cobinder.regions.dir, "full_regions/containing_all_cobinders", -->
<!--                                       paste0("overlapping_cobinders_full_regions_", family_name, ".bed")) -->
<!-- with.cobinder.full       <- list.files(file.path(cobinder.regions.dir, "full_regions/with_cobinder_motif_specific", -->
<!--                                                  family_name), full.names = TRUE) -->
<!-- no.cobinder.full         <- list.files(file.path(cobinder.regions.dir, "full_regions/no_cobinder_motif_specific", -->
<!--                                                  family_name), full.names = TRUE) -->

<!-- ``` -->

<!-- <table class='table'> -->
<!--   <thead> -->
<!--     <tr>  -->
<!--       <th>Region type</th> <th>Description</th> <th>Download</th> -->
<!--     <tr> -->
<!--   </thead> -->
<!--   <thead> -->
<!--     <tr> -->
<!--       <th> **Anchors only** </th> <td> </td> <td> </td> -->
<!--     <tr> -->
<!--   </thead> -->
<!--   <tbody> -->
<!--     <tr>  -->
<!--       <td> Overlapping co-binders </td> <td> Anchors that can be associated with *all* co-binders. Empty if only one co-binder was discovered or there are no anchors that could be associated with all discovered co-binders. </td> -->
<!--       <td> -->
<!--       ```{r overlapping-anchors, cache = TRUE, echo = FALSE, eval = TRUE, include = TRUE} -->
<!--       download_button(all.cobinder.anchors, basename(all.cobinder.anchors)) -->
<!--       ``` -->
<!--       </td> -->
<!--     <tr>  -->
<!--     <tr>  -->
<!--       <td> With co-binder </td> <td> Anchors that are associated with co-binder (co-binder-specific). </td> -->
<!--       <td> -->
<!--       ```{r with-cobinder-anchors, cache = TRUE, echo = FALSE, eval = TRUE, include = TRUE} -->
<!--       download_button(with.cobinder.anchors, paste0("cobinder_specific_anchors_with_cobinder")) -->
<!--       ``` -->
<!--       </td>  -->
<!--     <tr> -->
<!--     <tr>  -->
<!--       <td> No co-binder </td> <td> Anchors that are *not* associated with co-binder (co-binder-specific). </td> -->
<!--       <td> -->
<!--       ```{r no-cobinder-anchors, cache = TRUE, echo = FALSE, eval = TRUE, include = TRUE} -->
<!--       download_button(no.cobinder.anchors, paste0("cobinder_specific_anchors_no_cobinder")) -->
<!--       ``` -->
<!--       </td>  -->
<!--     <tr> -->
<!--   </tbody> -->
<!--   <thead> -->
<!--     <tr>  -->
<!--       <th> **Full regions (anchors + flanks)** </th> <td> </td> <td> </td> -->
<!--     <tr> -->
<!--   </thead> -->
<!--   <tbody> -->
<!--     <tr>  -->
<!--       <td> Overlapping co-binders </td> <td> Full regions with *all* discovered co-binder. Empty if only one co-binder was discovered or there are no regions with all discovered co-binders. </td> -->
<!--       <td> -->
<!--       ```{r overlapping-full, cache = TRUE, echo = FALSE, eval = TRUE, include = TRUE} -->
<!--       download_button(all.cobinder.full, basename(all.cobinder.full)) -->
<!--       ``` -->
<!--       </td>  -->
<!--     <tr> -->
<!--     <tr> -->
<!--       <td> With co-binder </td> <td> Full regions *with* co-binder (co-binder-specific). </td> -->
<!--       <td> -->
<!--       ```{r with-cobinder-full, cache = TRUE, echo = FALSE, eval = TRUE, include = TRUE} -->
<!--       download_button(with.cobinder.full, paste0("cobinder_specific_full_regions_with_cobinder")) -->
<!--       ``` -->
<!--       </td> -->
<!--     <tr> -->
<!--     <tr>  -->
<!--       <td> No co-binder </td> <td> Full regions *without* co-binder (co-binder-specific). </td> -->
<!--       <td> -->
<!--       ```{r no-cobinder-full, cache = TRUE, echo = FALSE, eval = TRUE, include = TRUE} -->
<!--       download_button(no.cobinder.full, paste0("cobinder_specific_full_regions_no_cobinder")) -->
<!--       ``` -->
<!--       </td>  -->
<!--     <tr> -->
<!--   <tbody> -->
<!-- </table> -->


<!-- ```{r download-all-regions, cache = TRUE, echo = FALSE, eval = TRUE, include = TRUE} -->

<!-- all.regions <- c(all.cobinder.anchors, -->
<!--                  with.cobinder.anchors, -->
<!--                  no.cobinder.anchors, -->
<!--                  all.cobinder.full, -->
<!--                  with.cobinder.full, -->
<!--                  no.cobinder.full) -->

<!-- downloadthis::download_file(path = as.vector(all.regions), -->
<!--                             output_name = "all_cobinder_regions", -->
<!--                             button_label = "Download all regions", -->
<!--                             button_type = "primary", -->
<!--                             has_icon = TRUE, -->
<!--                             icon = "fa fa-save", -->
<!--                             self_contained = FALSE) -->

<!-- ``` -->

<p>&nbsp;</p>

# Co-binder validation through motif similarity and PPI data

<div align = "justify">
To infer what transcription factor (TF) could be co-binding together with the anchor TF, we compare discovered co-binder motifs against the collection of know motifs (JASPAR and CIS-BP species-specific and pooled motif collections). Then, we search the protein-protein interaction data from STRING for these co-binder pairs. If such pair is found with significance, we confirm it as a validated anchor-co-binder pair (Figure 2). If the pair is not found in PPI data, we predict the TF based on motif similarity with know motifs (Figure 3).
</div>

<p>&nbsp;</p>

## Co-binder matches in the PPI data {.tabset}

### cobinder_0  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/PPI-similarity-1.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_1  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/PPI-similarity-2.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_2  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/PPI-similarity-3.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_3  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/PPI-similarity-4.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_4  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/PPI-similarity-5.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_5  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/PPI-similarity-6.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_6  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/PPI-similarity-7.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_7  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/PPI-similarity-8.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>

## {.unlisted .unnumbered .toc-ignore}

<!-- ```{r, PPI-similarity-button, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->
<!-- if (as.character(PPI.motif.similarity.files) != "NA") { -->

<!--   if (file.exists(PPI.motif.similarity.files[1])) { -->

<!--   downloadthis::download_file(path = as.vector(PPI.motif.similarity.pdf), -->
<!--                               output_name = "ppi_motif_similarity_plots_species_specific_collection", -->
<!--                               button_label = "Download species-specific collection result plots as pdf", -->
<!--                               button_type = "primary", -->
<!--                               has_icon = TRUE, -->
<!--                               icon = "fa fa-save", -->
<!--                               self_contained = FALSE) -->
<!--   } -->
<!-- } -->
<!-- ``` -->

<!-- ```{r, PPI-similarity-button-full, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->
<!-- if (as.character(PPI.motif.similarity.files)[1] != "NA") { -->

<!--   full.PPI.motif.similarity.pdf.paths <- c() -->

<!--   for (file in as.vector(full.PPI.motif.similarity.pdf)) { -->

<!--     if (file.exists(file)) { -->
<!--        full.PPI.motif.similarity.pdf.paths <- c(full.PPI.motif.similarity.pdf.paths, file) -->
<!--     } -->
<!--   } -->

<!--   if (!identical(full.PPI.motif.similarity.pdf.paths, "NULL")) { -->

<!--       downloadthis::download_file(path = as.vector(full.PPI.motif.similarity.pdf.paths), -->
<!--                               output_name = "ppi_motif_similarity_plots_full_collection", -->
<!--                               button_label = "Download full collection result plots as pdf", -->
<!--                               button_type = "primary", -->
<!--                               has_icon = TRUE, -->
<!--                               icon = "fa fa-save", -->
<!--                               self_contained = FALSE) -->
<!--   } -->
<!-- } -->
<!-- ``` -->

<p>&nbsp;</p>

### Co-binder-anchor confirmed pairs, based on PPI analysis and comparison with species-specific motif library

<div align = "justify">
All the pairs that were significant, based on both motif similarity of the co-binder and PPI data.
</div>

<p>&nbsp;</p>

<!--html_preserve--><a href="data:text/csv;base64,YW5jaG9yX3RmO2NvYmluZGVyX2lkO2NvYmluZGVyX21vdGlmX2lkO2NvYmluZGVyX25hbWU7dGZfcGFpcjtwX3ZhbHVlO2NvbWJpbmVkX3Njb3JlCkZPWEEyO2NvYmluZGVyXzc7TTA5Mzg5XzIuMDA7U09YOSxTT1gxO0ZPWEEyOjpTT1g5OzAsMDAxMDkwMDk7NTE0CkZPWEEyO2NvYmluZGVyXzc7TUEwNDgyLjI7R0FUQTQ7Rk9YQTI6OkdBVEE0OzAsMDAyODU0NTE7NTMzCkZPWEEyO2NvYmluZGVyXzQ7TUExNjQ1LjE7TktYMi0yO0ZPWEEyOjpOS1gyLTI7MCwwMDMyMjQxNjs1MzUKRk9YQTI7Y29iaW5kZXJfNDtNMDQ4NzZfMi4wMDtHQVRBNDtGT1hBMjo6R0FUQTQ7MCwwMDMzNDQwNDs1MzMKRk9YQTI7Y29iaW5kZXJfNztNQTE5OTEuMTtITkYxQTtGT1hBMjo6SE5GMUE7MCwwMDM3OTg0Mzs1NzkKRk9YQTI7Y29iaW5kZXJfMztNQTE5OTEuMTtITkYxQTtGT1hBMjo6SE5GMUE7MCwwMDQzNzg0ODs1NzkKRk9YQTI7Y29iaW5kZXJfMDtNMDk0MjdfMi4wMDtUO0ZPWEEyOjpUOzAsMDA0Njg4MDI7NjA2CkZPWEEyO2NvYmluZGVyXzQ7TUEwNDgyLjI7R0FUQTQ7Rk9YQTI6OkdBVEE0OzAsMDA3MTEyNTE7NTMzCkZPWEEyO2NvYmluZGVyXzM7TUEwNDgyLjI7R0FUQTQ7Rk9YQTI6OkdBVEE0OzAsMDA3NTg5Mjg7NTMzCkZPWEEyO2NvYmluZGVyXzE7TTA5NDI3XzIuMDA7VDtGT1hBMjo6VDswLDAwNzgwNDgzOzYwNgpGT1hBMjtjb2JpbmRlcl80O00wOTM4OV8yLjAwO1NPWDksU09YMTtGT1hBMjo6U09YOTswLDAxMDY0OTgwOzUxNApGT1hBMjtjb2JpbmRlcl80O01BMTk5MS4xO0hORjFBO0ZPWEEyOjpITkYxQTswLDAxMzM1NTIwOzU3OQpGT1hBMjtjb2JpbmRlcl82O00wOTQyN18yLjAwO1Q7Rk9YQTI6OlQ7MCwwMTM0NjIzMDs2MDYKRk9YQTI7Y29iaW5kZXJfNztNMDQ4NzZfMi4wMDtHQVRBNDtGT1hBMjo6R0FUQTQ7MCwwMTg0OTQ1MDs1MzMKRk9YQTI7Y29iaW5kZXJfNjtNQTA0ODIuMjtHQVRBNDtGT1hBMjo6R0FUQTQ7MCwwMTk4MTEwMDs1MzMKRk9YQTI7Y29iaW5kZXJfNTtNQTE2NDUuMTtOS1gyLTI7Rk9YQTI6Ok5LWDItMjswLDAyMzA1NTIwOzUzNQpGT1hBMjtjb2JpbmRlcl82O01BMTk5MS4xO0hORjFBO0ZPWEEyOjpITkYxQTswLDAyNTE0OTcwOzU3OQpGT1hBMjtjb2JpbmRlcl80O00wOTExN18yLjAwO0dBVEE0O0ZPWEEyOjpHQVRBNDswLDAyODg0NzIwOzUzMwpGT1hBMjtjb2JpbmRlcl82O00wOTM4OV8yLjAwO1NPWDksU09YMTtGT1hBMjo6U09YOTswLDAzMDQ1OTMwOzUxNApGT1hBMjtjb2JpbmRlcl8xO01BMTY0NS4xO05LWDItMjtGT1hBMjo6TktYMi0yOzAsMDMyMjczMzA7NTM1CkZPWEEyO2NvYmluZGVyXzQ7TTAzMDY2XzIuMDA7R0FUQTQ7Rk9YQTI6OkdBVEE0OzAsMDMyNTcyODA7NTMzCkZPWEEyO2NvYmluZGVyXzM7TTA5Mzg5XzIuMDA7U09YOSxTT1gxO0ZPWEEyOjpTT1g5OzAsMDMyNzc3MTA7NTE0CkZPWEEyO2NvYmluZGVyXzU7TUEwMTE0LjQ7SE5GNEE7Rk9YQTI6OkhORjRBOzAsMDMyODUwNDA7NTc5CkZPWEEyO2NvYmluZGVyXzc7TUExNjQ1LjE7TktYMi0yO0ZPWEEyOjpOS1gyLTI7MCwwMzQ4Mzc1MDs1MzUKRk9YQTI7Y29iaW5kZXJfMTtNQTE5OTEuMTtITkYxQTtGT1hBMjo6SE5GMUE7MCwwMzg5OTg3MDs1NzkKRk9YQTI7Y29iaW5kZXJfMjtNMDMxNjZfMi4wMDtETFgxLE5LWDEtMjtGT1hBMjo6RExYMTswLDA0MjY3NjYwOzUwNApGT1hBMjtjb2JpbmRlcl83O00wMzA2Nl8yLjAwO0dBVEE0O0ZPWEEyOjpHQVRBNDswLDA0ODMxNTYwOzUzMwo=" download="FOXA2_confirmed_pairs.csv">
<button class="btn btn-primary" has_icon="TRUE"><i class="fa fa-save"></i> Download table as csv</button>
</a><!--/html_preserve-->

<p>&nbsp;</p>

<!-- ### Co-binder-anchor confirmed pairs, based on PPI analysis and comparison with pooled motif library -->

<!-- <div align = "justify"> -->
<!-- All the pairs that were significant, based on both motif similarity of the co-binder and PPI data. -->
<!-- </div> -->

<!-- <p>&nbsp;</p> -->

<!-- ```{r confirmed-pairs-full, cache = TRUE, echo = FALSE, eval = TRUE, fig.cap = "**Table 2B. Significant co-binding pairs, based on motif similarity (using pooled motif library from multiple species) and PPI data**", fig.align = "center"} -->

<!-- if (file.exists(confirmed.pairs.full.tab.file)) { -->

<!--   ## Table: -->
<!--   confirmed.pairs.tab <- fread(confirmed.pairs.full.tab.file, header = TRUE, sep = "\t") -->

<!--   confirmed.pairs.tab <- confirmed.pairs.tab %>% -->
<!--     select(anchor_tf, cobinder_id, cobinder_motif_id, -->
<!--            cobinder_name, tf_pair, -->
<!--            p_value, combined_score) -->


<!-- } else { -->

<!--   confirmed.pairs.tab <- data.frame(anchor_tf = character(), -->
<!--                                     cobinder_id = character(), -->
<!--                                     cobinder_motif_id = character(), -->
<!--                                     cobinder_name = character(),  -->
<!--                                     tf_pair = character(), -->
<!--                                     p_value = double(),  -->
<!--                                     combined_score = integer()) -->
<!-- } -->

<!--   DT::datatable(confirmed.pairs.tab, -->
<!--                 style = "default", -->
<!--                 rownames = FALSE, -->
<!--                 options = list(scrollX = TRUE)) -->

<!-- if (file.exists(confirmed.pairs.full.tab.file)) { -->

<!--   ## Download button: -->
<!--   confirmed.pairs.tab %>% -->
<!--     downloadthis::download_this(output_name      = paste0(family_name, "_confirmed_pairs_full"), -->
<!--                                 output_extension = ".csv", -->
<!--                                 button_label     = "Download table as csv", -->
<!--                                 button_type      = "primary", -->
<!--                                 has_icon         = TRUE, -->
<!--                                 icon             = "fa fa-save") -->
<!-- } -->

<!-- ``` -->

<!-- <p>&nbsp;</p> -->

## Co-binder motif similarity when no matches in the PPI data found {.tabset}

### cobinder_0  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/no-match-similarity-1.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_1  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/no-match-similarity-2.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_2  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/no-match-similarity-3.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_3  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/no-match-similarity-4.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_4  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/no-match-similarity-5.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_5  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/no-match-similarity-6.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_6  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/no-match-similarity-7.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_7  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/no-match-similarity-8.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>

## {.unlisted .unnumbered .toc-ignore}

<!-- ```{r, no-match-similarity-button, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->

<!-- if (file.exists(no.match.motif.similarity.pdf[1])) { -->

<!-- downloadthis::download_file(path = as.vector(no.match.motif.similarity.pdf), -->
<!--                             output_name = "no_match_motif_similarity_plots_species_specific_collection", -->
<!--                             button_label = "Download species-specific collection result plots as pdf", -->
<!--                             button_type = "primary", -->
<!--                             has_icon = TRUE, -->
<!--                             icon = "fa fa-save", -->
<!--                             self_contained = FALSE) -->
<!-- } -->
<!-- ``` -->

<!-- ```{r, no-match-similarity-button-full, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->

<!-- if (file.exists(full.no.match.motif.similarity.pdf[1])) { -->

<!-- downloadthis::download_file(path = as.vector(full.no.match.motif.similarity.pdf), -->
<!--                             output_name = "no_match_motif_similarity_plots_full_collection", -->
<!--                             button_label = "Download full collection result plots as pdf", -->
<!--                             button_type = "primary", -->
<!--                             has_icon = TRUE, -->
<!--                             icon = "fa fa-save", -->
<!--                             self_contained = FALSE) -->
<!-- } -->
<!-- ``` -->

<p>&nbsp;</p>

### Co-binder-anchor pair predictions, based on motif similarity

<div align = "justify">
If a match with certain know motif collection was not found, such co-binder TF prediction are displayed in plots above and provided in the table bellow.
</div>

<p>&nbsp;</p>

<!--html_preserve--><a href="data:text/csv;base64,YW5jaG9yX3RmO2NvYmluZGVyX2lkO2NvYmluZGVyX21vdGlmX2lkO2NvYmluZGVyX25hbWU7cF92YWx1ZQpGT1hBMjtjb2JpbmRlcl8xO00wODI0N18yLjAwO1pORjM4Mjs4LDA1NTExZS0wNwpGT1hBMjtjb2JpbmRlcl8xO00wNzY5Ml8yLjAwO1pORjU2NzsxLDAzOTYzZS0wNgpGT1hBMjtjb2JpbmRlcl8xO00wNzU5MF8yLjAwO1pORjI4Nzs0LDc0MDkwZS0wNgpGT1hBMjtjb2JpbmRlcl8xO00wNzU5MF8yLjAwO1pORjI4Nzs0LDc0MDkwZS0wNgpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1Ml8yLjAwO1pORjM4NDs5LDA1MDAyZS0wNgpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1Ml8yLjAwO1pORjM4NDs5LDA1MDAyZS0wNgpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1Ml8yLjAwO1pORjM4NDs5LDA1MDAyZS0wNgpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1Ml8yLjAwO1pORjM4NDs5LDA1MDAyZS0wNgpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1Ml8yLjAwO1pORjM4NDs5LDA1MDAyZS0wNgpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1Ml8yLjAwO1pORjM4NDs5LDA1MDAyZS0wNgpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1Ml8yLjAwO1pORjM4NDs5LDA1MDAyZS0wNgpGT1hBMjtjb2JpbmRlcl8xO00wNDQ1MV8yLjAwO1pORjM4NDsxLDAzOTkyZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wNDQ1MV8yLjAwO1pORjM4NDsxLDAzOTkyZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wNDQ1MV8yLjAwO1pORjM4NDsxLDAzOTkyZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wNDQ1MV8yLjAwO1pORjM4NDsxLDAzOTkyZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wNDQ1MV8yLjAwO1pORjM4NDsxLDAzOTkyZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wNDQ1MV8yLjAwO1pORjM4NDsxLDAzOTkyZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wNDQ1MV8yLjAwO1pORjM4NDsxLDAzOTkyZS0wNQpGT1hBMjtjb2JpbmRlcl8xO01BMTk3OC4xO1pORjM1NEE7MSwwNjgyNGUtMDUKRk9YQTI7Y29iaW5kZXJfMTtNQTE5NzguMTtaTkYzNTRBOzEsMDY4MjRlLTA1CkZPWEEyO2NvYmluZGVyXzE7TUExOTc4LjE7Wk5GMzU0QTsxLDA2ODI0ZS0wNQpGT1hBMjtjb2JpbmRlcl8xO01BMTk3OC4xO1pORjM1NEE7MSwwNjgyNGUtMDUKRk9YQTI7Y29iaW5kZXJfMTtNQTE5NzguMTtaTkYzNTRBOzEsMDY4MjRlLTA1CkZPWEEyO2NvYmluZGVyXzE7TUExOTc4LjE7Wk5GMzU0QTsxLDA2ODI0ZS0wNQpGT1hBMjtjb2JpbmRlcl8wO00wODI0N18yLjAwO1pORjM4MjsxLDI4MjkyZS0wNQpGT1hBMjtjb2JpbmRlcl8wO00wODM2N18yLjAwO1pORjY2OTsxLDc0NzM0ZS0wNQpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1MV8yLjAwO1pORjM4NDsxLDkzNjk1ZS0wNQpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1MV8yLjAwO1pORjM4NDsxLDkzNjk1ZS0wNQpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1MV8yLjAwO1pORjM4NDsxLDkzNjk1ZS0wNQpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1MV8yLjAwO1pORjM4NDsxLDkzNjk1ZS0wNQpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1MV8yLjAwO1pORjM4NDsxLDkzNjk1ZS0wNQpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1MV8yLjAwO1pORjM4NDsxLDkzNjk1ZS0wNQpGT1hBMjtjb2JpbmRlcl8wO00wNDQ1MV8yLjAwO1pORjM4NDsxLDkzNjk1ZS0wNQpGT1hBMjtjb2JpbmRlcl8wO00wNzY5Ml8yLjAwO1pORjU2NzsyLDA5MDk2ZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wODM3OF8yLjAwO1pGUDI4OzIsMjM3MjRlLTA1CkZPWEEyO2NvYmluZGVyXzA7TTA4Mzc4XzIuMDA7WkZQMjg7Miw0MzQ1OGUtMDUKRk9YQTI7Y29iaW5kZXJfMDtNMDc1OTBfMi4wMDtaTkYyODc7NCwwMDIwOGUtMDUKRk9YQTI7Y29iaW5kZXJfMDtNMDc1OTBfMi4wMDtaTkYyODc7NCwwMDIwOGUtMDUKRk9YQTI7Y29iaW5kZXJfMTtNMDg5NjBfMi4wMDtaTkYzNTA7NCwyNTI5NGUtMDUKRk9YQTI7Y29iaW5kZXJfMTtNMDg5NjBfMi4wMDtaTkYzNTA7NCwyNTI5NGUtMDUKRk9YQTI7Y29iaW5kZXJfMTtNMDg5MzBfMi4wMDtaRlA4Mjs1LDE3MTkxZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wNzU4MF8yLjAwO1pORjEzMzs1LDIzNzY0ZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wNzU4MF8yLjAwO1pORjEzMzs1LDIzNzY0ZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wNzU4MF8yLjAwO1pORjEzMzs1LDIzNzY0ZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wNzU3MV8yLjAwO1pORjE4NDs1LDgyMDQ3ZS0wNQpGT1hBMjtjb2JpbmRlcl82O00wODA2NV8yLjAwO0JBQ0gyOzUsOTI1MTZlLTA1CkZPWEEyO2NvYmluZGVyXzY7TTA4MDY1XzIuMDA7QkFDSDI7NSw5MjUxNmUtMDUKRk9YQTI7Y29iaW5kZXJfNjtNQTA0OTYuMztNQUZLOzYsNTgzNDllLTA1CkZPWEEyO2NvYmluZGVyXzY7TUEwNDk2LjM7TUFGSzs2LDU4MzQ5ZS0wNQpGT1hBMjtjb2JpbmRlcl8xO00wOTIzNF8yLjAwO0lSRjM7OCw4NDUzOGUtMDUKRk9YQTI7Y29iaW5kZXJfMDtNMDc1NzFfMi4wMDtaTkYxODQ7OCw5NDIzMGUtMDUKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTVfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwwNzA4OWUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTVfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwwNzA4OWUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTVfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwwNzA4OWUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTVfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwwNzA4OWUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTVfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwwNzA4OWUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTVfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwwNzA4OWUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTVfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwwNzA4OWUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQzMTZfMi4wMDtDUkVCM0wxLENSRUIzTDI7MSwwNzA4OWUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQzMTZfMi4wMDtDUkVCM0wxLENSRUIzTDI7MSwwNzA4OWUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQzMTZfMi4wMDtDUkVCM0wxLENSRUIzTDI7MSwwNzA4OWUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDgzNjdfMi4wMDtaTkY2Njk7MSwwODI2NmUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDQ0NTJfMi4wMDtaTkYzODQ7MSwxODc0MGUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDQ0NTJfMi4wMDtaTkYzODQ7MSwxODc0MGUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDQ0NTJfMi4wMDtaTkYzODQ7MSwxODc0MGUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDQ0NTJfMi4wMDtaTkYzODQ7MSwxODc0MGUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDQ0NTJfMi4wMDtaTkYzODQ7MSwxODc0MGUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDQ0NTJfMi4wMDtaTkYzODQ7MSwxODc0MGUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDQ0NTJfMi4wMDtaTkYzODQ7MSwxODc0MGUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDE5ODdfMi4wMDtGT1hJMixGT1hJMzsxLDIxNzMyZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wMTk4N18yLjAwO0ZPWEkyLEZPWEkzOzEsMjE3MzJlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA4OTAzXzIuMDA7Wk5GMzk0OzEsMzY5NjZlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA4OTAzXzIuMDA7Wk5GMzk0OzEsMzY5NjZlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA4OTE0XzIuMDA7Wk5GMzU0QTsxLDQ5MDI1ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wODkxNF8yLjAwO1pORjM1NEE7MSw0OTAyNWUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDg5MTRfMi4wMDtaTkYzNTRBOzEsNDkwMjVlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA4OTE0XzIuMDA7Wk5GMzU0QTsxLDQ5MDI1ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wODkxNF8yLjAwO1pORjM1NEE7MSw0OTAyNWUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDg5MTRfMi4wMDtaTkYzNTRBOzEsNDkwMjVlLTA0CkZPWEEyO2NvYmluZGVyXzc7TTA4OTYwXzIuMDA7Wk5GMzUwOzEsNTg3NTllLTA0CkZPWEEyO2NvYmluZGVyXzc7TTA4OTYwXzIuMDA7Wk5GMzUwOzEsNTg3NTllLTA0CkZPWEEyO2NvYmluZGVyXzA7TTA1NTIwXzIuMDA7SFNGNSxIU0ZYMSxIU0ZYMjsxLDY1NDQ0ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wNTUyMF8yLjAwO0hTRjUsSFNGWDEsSFNGWDI7MSw2NTQ0NGUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDU1MjBfMi4wMDtIU0Y1LEhTRlgxLEhTRlgyOzEsNjU0NDRlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTA1NTIwXzIuMDA7SFNGNSxIU0ZYMSxIU0ZYMjsxLDY1NDQ0ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wOTU5Nl8yLjAwO0lSRjI7MSw4OTkzOWUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDkzNDlfMi4wMDtORkFUQzE7MSw5ODk2MmUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDkzNDlfMi4wMDtORkFUQzE7MSw5ODk2MmUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDkzNDlfMi4wMDtORkFUQzE7MSw5ODk2MmUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDkzNDlfMi4wMDtORkFUQzE7MSw5ODk2MmUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDI1MzFfMi4wMDtMSU41NDsxLDk5NTIyZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wMjUzMV8yLjAwO0xJTjU0OzEsOTk1MjJlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTAyNTMxXzIuMDA7TElONTQ7MSw5OTUyMmUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDI1MzFfMi4wMDtMSU41NDsxLDk5NTIyZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wMjUzNF8yLjAwO0xJTjU0OzEsOTk1MjJlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTAyNTM0XzIuMDA7TElONTQ7MSw5OTUyMmUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDI1MzRfMi4wMDtMSU41NDsxLDk5NTIyZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wMjUzNF8yLjAwO0xJTjU0OzEsOTk1MjJlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTAyNTMzXzIuMDA7TElONTQ7MiwxMzk3NWUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDI1MzNfMi4wMDtMSU41NDsyLDEzOTc1ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wMjUzM18yLjAwO0xJTjU0OzIsMTM5NzVlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTAyNTMzXzIuMDA7TElONTQ7MiwxMzk3NWUtMDQKRk9YQTI7Y29iaW5kZXJfNjtNMDgwNzVfMi4wMDtNQUZLOzIsMjQ5NTZlLTA0CkZPWEEyO2NvYmluZGVyXzY7TTA4MDc1XzIuMDA7TUFGSzsyLDI0OTU2ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wODcyOF8yLjAwO0NMT0NLOzIsMjgwMDJlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA4NzI4XzIuMDA7Q0xPQ0s7MiwyODAwMmUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDE5ODdfMi4wMDtGT1hJMixGT1hJMzsyLDM0NjcwZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wMTk4N18yLjAwO0ZPWEkyLEZPWEkzOzIsMzQ2NzBlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA3NzMxXzIuMDA7Wk5GNDQ7MiwzOTg3NWUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDc3MzFfMi4wMDtaTkY0NDsyLDM5ODc1ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wNzczMV8yLjAwO1pORjQ0OzIsMzk4NzVlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA3NzMxXzIuMDA7Wk5GNDQ7MiwzOTg3NWUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDc3MzFfMi4wMDtaTkY0NDsyLDM5ODc1ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wNzczMV8yLjAwO1pORjQ0OzIsMzk4NzVlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTAwNzkwXzIuMDA7Rk9YSTIsRk9YSTM7Miw3OTAyNWUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDA3OTBfMi4wMDtGT1hJMixGT1hJMzsyLDc5MDI1ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wMTMyMF8yLjAwO0xJTjU0OzIsNzkwMjVlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTAxMzIwXzIuMDA7TElONTQ7Miw3OTAyNWUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDEzMjBfMi4wMDtMSU41NDsyLDc5MDI1ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wMTMyMF8yLjAwO0xJTjU0OzIsNzkwMjVlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTA3NTgwXzIuMDA7Wk5GMTMzOzIsODk5NzFlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTA3NTgwXzIuMDA7Wk5GMTMzOzIsODk5NzFlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTA3NTgwXzIuMDA7Wk5GMTMzOzIsODk5NzFlLTA0CkZPWEEyO2NvYmluZGVyXzQ7TTA3Njg0XzIuMDA7Wk5GMTk3OzMsMDEwMjJlLTA0CkZPWEEyO2NvYmluZGVyXzQ7TTA3Njg0XzIuMDA7Wk5GMTk3OzMsMDEwMjJlLTA0CkZPWEEyO2NvYmluZGVyXzQ7TTA3Njg0XzIuMDA7Wk5GMTk3OzMsMDEwMjJlLTA0CkZPWEEyO2NvYmluZGVyXzQ7TTA3Njg0XzIuMDA7Wk5GMTk3OzMsMDEwMjJlLTA0CkZPWEEyO2NvYmluZGVyXzQ7TTA3Njg0XzIuMDA7Wk5GMTk3OzMsMDEwMjJlLTA0CkZPWEEyO2NvYmluZGVyXzQ7TTA3Njg0XzIuMDA7Wk5GMTk3OzMsMDEwMjJlLTA0CkZPWEEyO2NvYmluZGVyXzQ7TTA3Njg0XzIuMDA7Wk5GMTk3OzMsMDEwMjJlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTAwNzkwXzIuMDA7Rk9YSTIsRk9YSTM7MywxMjUyOWUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDA3OTBfMi4wMDtGT1hJMixGT1hJMzszLDEyNTI5ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wMjUzM18yLjAwO0xJTjU0OzMsMTI1MjllLTA0CkZPWEEyO2NvYmluZGVyXzE7TTAyNTMzXzIuMDA7TElONTQ7MywxMjUyOWUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MzNfMi4wMDtMSU41NDszLDEyNTI5ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wMjUzM18yLjAwO0xJTjU0OzMsMTI1MjllLTA0CkZPWEEyO2NvYmluZGVyXzA7TTAwMjc3XzIuMDA7UEJYNDszLDE0MjIxZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wMjUzNF8yLjAwO0xJTjU0OzMsMjc1NjBlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTAyNTM0XzIuMDA7TElONTQ7MywyNzU2MGUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MzRfMi4wMDtMSU41NDszLDI3NTYwZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wMjUzNF8yLjAwO0xJTjU0OzMsMjc1NjBlLTA0CkZPWEEyO2NvYmluZGVyXzc7TTAzMzI4XzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7Myw4MDk5OWUtMDQKRk9YQTI7Y29iaW5kZXJfNztNMDMzMjhfMi4wMDtIU0ZZMixIU0ZYMSxIU0ZYMjszLDgwOTk5ZS0wNApGT1hBMjtjb2JpbmRlcl83O00wMzMyOF8yLjAwO0hTRlkyLEhTRlgxLEhTRlgyOzMsODA5OTllLTA0CkZPWEEyO2NvYmluZGVyXzc7TTAzMzI4XzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7Myw4MDk5OWUtMDQKRk9YQTI7Y29iaW5kZXJfNDtNMDg5NjBfMi4wMDtaTkYzNTA7Myw4MzEwNGUtMDQKRk9YQTI7Y29iaW5kZXJfNDtNMDg5NjBfMi4wMDtaTkYzNTA7Myw4MzEwNGUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyNDBfMi4wMDtDUkVCMzs0LDA2Njk0ZS0wNApGT1hBMjtjb2JpbmRlcl81O00wNDI0MF8yLjAwO0NSRUIzOzQsMDY2OTRlLTA0CkZPWEEyO2NvYmluZGVyXzU7TTA0MjQwXzIuMDA7Q1JFQjM7NCwwNjY5NGUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyNDJfMi4wMDtDUkVCMzs0LDA2Njk0ZS0wNApGT1hBMjtjb2JpbmRlcl81O00wNDI0Ml8yLjAwO0NSRUIzOzQsMDY2OTRlLTA0CkZPWEEyO2NvYmluZGVyXzU7TTA0MjQyXzIuMDA7Q1JFQjM7NCwwNjY5NGUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTdfMi4wMDtDUkVCM0w0LENSRUIzTDI7NCwwNjY5NGUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTdfMi4wMDtDUkVCM0w0LENSRUIzTDI7NCwwNjY5NGUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTdfMi4wMDtDUkVCM0w0LENSRUIzTDI7NCwwNjY5NGUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTdfMi4wMDtDUkVCM0w0LENSRUIzTDI7NCwwNjY5NGUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTdfMi4wMDtDUkVCM0w0LENSRUIzTDI7NCwwNjY5NGUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTdfMi4wMDtDUkVCM0w0LENSRUIzTDI7NCwwNjY5NGUtMDQKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTdfMi4wMDtDUkVCM0w0LENSRUIzTDI7NCwwNjY5NGUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDgzNzJfMi4wMDtaTkYxNDA7NCwwNzM0NWUtMDQKRk9YQTI7Y29iaW5kZXJfNjtVTjAyMjIuMTtaTkY3NjU7NCwxMDM1MWUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDEzMjBfMi4wMDtMSU41NDs0LDExMzM4ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wMTMyMF8yLjAwO0xJTjU0OzQsMTEzMzhlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTAxMzIwXzIuMDA7TElONTQ7NCwxMTMzOGUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDEzMjBfMi4wMDtMSU41NDs0LDExMzM4ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wMjUzMV8yLjAwO0xJTjU0OzQsMTM5NDZlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTAyNTMxXzIuMDA7TElONTQ7NCwxMzk0NmUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MzFfMi4wMDtMSU41NDs0LDEzOTQ2ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wMjUzMV8yLjAwO0xJTjU0OzQsMTM5NDZlLTA0CkZPWEEyO2NvYmluZGVyXzc7TUEwODk3LjE7SE1YMjs0LDY1NjQ2ZS0wNApGT1hBMjtjb2JpbmRlcl83O01BMDg5Ny4xO0hNWDI7NCw2NTY0NmUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDc2MDhfMi4wMDtaTkYzODI7NCw2ODM3NWUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDg5MDNfMi4wMDtaTkYzOTQ7NCw2OTM3OGUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDg5MDNfMi4wMDtaTkYzOTQ7NCw2OTM3OGUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDk1OTZfMi4wMDtJUkYyOzQsODY5NjJlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA3NzY2XzIuMDA7Wk5GODc5OzQsOTU0OThlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTA1NTIyXzIuMDA7SFNGNSxIU0ZYMSxIU0ZYMjs1LDAxNzk1ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wNTUyMl8yLjAwO0hTRjUsSFNGWDEsSFNGWDI7NSwwMTc5NWUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDU1MjJfMi4wMDtIU0Y1LEhTRlgxLEhTRlgyOzUsMDE3OTVlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTA1NTIyXzIuMDA7SFNGNSxIU0ZYMSxIU0ZYMjs1LDAxNzk1ZS0wNApGT1hBMjtjb2JpbmRlcl82O01BMTcyNS4xO1pORjE4OTs1LDIzNTUxZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wNzcxOF8yLjAwO1pORjY4Mjs1LDMyMDY4ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wODkzNF8yLjAwO1pORjcwODs1LDUyOTgzZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wODkzNF8yLjAwO1pORjcwODs1LDUyOTgzZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wODkzNF8yLjAwO1pORjcwODs1LDUyOTgzZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wNDYxMF8yLjAwO1pORjUwMTs1LDU1ODA3ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wNDYxMF8yLjAwO1pORjUwMTs1LDU1ODA3ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wOTM0OV8yLjAwO05GQVRDMTs1LDY4OTE3ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wOTM0OV8yLjAwO05GQVRDMTs1LDY4OTE3ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wOTM0OV8yLjAwO05GQVRDMTs1LDY4OTE3ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wOTM0OV8yLjAwO05GQVRDMTs1LDY4OTE3ZS0wNApGT1hBMjtjb2JpbmRlcl81O1VOMDYyNS4xO1pORjUyNzs1LDg3Mzk0ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wODcyOF8yLjAwO0NMT0NLOzYsMDc0NzhlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTA4NzI4XzIuMDA7Q0xPQ0s7NiwwNzQ3OGUtMDQKRk9YQTI7Y29iaW5kZXJfNztNQTE1NzkuMTtaQlRCMjY7NiwyNTMxOGUtMDQKRk9YQTI7Y29iaW5kZXJfNztNQTE1NzkuMTtaQlRCMjY7NiwyNTMxOGUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDAyNzdfMi4wMDtQQlg0OzYsNDY1MTZlLTA0CkZPWEEyO2NvYmluZGVyXzA7TUExNjIzLjE7U1RBVDI7NywxMjA0OGUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNQTE2MjMuMTtTVEFUMjs3LDEyMDQ4ZS0wNApGT1hBMjtjb2JpbmRlcl8wO01BMTYyMy4xO1NUQVQyOzcsMTIwNDhlLTA0CkZPWEEyO2NvYmluZGVyXzA7TUExNjIzLjE7U1RBVDI7NywxMjA0OGUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNQTE2MjMuMTtTVEFUMjs3LDEyMDQ4ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wNzYyMF8yLjAwO1pORjU1ODs3LDM2OTUzZS0wNApGT1hBMjtjb2JpbmRlcl8zO00wODM5Nl8yLjAwO1pORjM1MDs3LDUzODQ0ZS0wNApGT1hBMjtjb2JpbmRlcl8zO00wODM5Nl8yLjAwO1pORjM1MDs3LDUzODQ0ZS0wNApGT1hBMjtjb2JpbmRlcl82O00wMDI1MV8yLjAwO1pORjY1NTs3LDYwMzM0ZS0wNApGT1hBMjtjb2JpbmRlcl82O00wMDI1MV8yLjAwO1pORjY1NTs3LDYwMzM0ZS0wNApGT1hBMjtjb2JpbmRlcl83O01BMDg5OC4xO0hNWDM7Nyw2NDIyNGUtMDQKRk9YQTI7Y29iaW5kZXJfNztNQTA4OTguMTtITVgzOzcsNjQyMjRlLTA0CkZPWEEyO2NvYmluZGVyXzc7TUEwODk4LjE7SE1YMzs3LDY0MjI0ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wNzc1M18yLjAwO1pORjgwNTs4LDA0NTYzZS0wNApGT1hBMjtjb2JpbmRlcl80O00wNzczM18yLjAwO1pORjgyMzs4LDI4NjQwZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wMDM3MV8yLjAwO05SMkUzOzgsMzExOTRlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTAwMzcxXzIuMDA7TlIyRTM7OCwzMTE5NGUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDAzNzFfMi4wMDtOUjJFMzs4LDMxMTk0ZS0wNApGT1hBMjtjb2JpbmRlcl8wO00wMDM3MV8yLjAwO05SMkUzOzgsMzExOTRlLTA0CkZPWEEyO2NvYmluZGVyXzA7TTAwMzcxXzIuMDA7TlIyRTM7OCwzMTE5NGUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNQTE5NzguMTtaTkYzNTRBOzgsNDIyMDhlLTA0CkZPWEEyO2NvYmluZGVyXzA7TUExOTc4LjE7Wk5GMzU0QTs4LDQyMjA4ZS0wNApGT1hBMjtjb2JpbmRlcl8wO01BMTk3OC4xO1pORjM1NEE7OCw0MjIwOGUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNQTE5NzguMTtaTkYzNTRBOzgsNDIyMDhlLTA0CkZPWEEyO2NvYmluZGVyXzA7TUExOTc4LjE7Wk5GMzU0QTs4LDQyMjA4ZS0wNApGT1hBMjtjb2JpbmRlcl8wO01BMTk3OC4xO1pORjM1NEE7OCw0MjIwOGUtMDQKRk9YQTI7Y29iaW5kZXJfMDtNMDE5ODNfMi4wMDtGT1hCMjs4LDc3MTEzZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wMDM3MV8yLjAwO05SMkUzOzgsODY3MjZlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTAwMzcxXzIuMDA7TlIyRTM7OCw4NjcyNmUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDAzNzFfMi4wMDtOUjJFMzs4LDg2NzI2ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wMDM3MV8yLjAwO05SMkUzOzgsODY3MjZlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTAwMzcxXzIuMDA7TlIyRTM7OCw4NjcyNmUtMDQKRk9YQTI7Y29iaW5kZXJfMztNMDgyNzlfMi4wMDtaTkYzN0E7OSwwOTUzM2UtMDQKRk9YQTI7Y29iaW5kZXJfMztNMDgyNzlfMi4wMDtaTkYzN0E7OSwwOTUzM2UtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDU1MjBfMi4wMDtIU0Y1LEhTRlgxLEhTRlgyOzksNDMxMjRlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA1NTIwXzIuMDA7SFNGNSxIU0ZYMSxIU0ZYMjs5LDQzMTI0ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wNTUyMF8yLjAwO0hTRjUsSFNGWDEsSFNGWDI7OSw0MzEyNGUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDU1MjBfMi4wMDtIU0Y1LEhTRlgxLEhTRlgyOzksNDMxMjRlLTA0CkZPWEEyO2NvYmluZGVyXzY7TTAwMjUwXzIuMDA7Wk5GNjU1OzksNTAyMjFlLTA0CkZPWEEyO2NvYmluZGVyXzY7TTAwMjUwXzIuMDA7Wk5GNjU1OzksNTAyMjFlLTA0CkZPWEEyO2NvYmluZGVyXzY7TTAwMjUyXzIuMDA7Wk5GNjU1OzksNTAyMjFlLTA0CkZPWEEyO2NvYmluZGVyXzY7TTAwMjUyXzIuMDA7Wk5GNjU1OzksNTAyMjFlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA4Nzk0XzIuMDA7QkFURjM7OSw1ODQzOWUtMDQKRk9YQTI7Y29iaW5kZXJfMTtNMDg3OTRfMi4wMDtCQVRGMzs5LDU4NDM5ZS0wNApGT1hBMjtjb2JpbmRlcl8xO00wODc5NF8yLjAwO0JBVEYzOzksNTg0MzllLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA3NzA0XzIuMDA7Wk5GNjA1OzksODU0NzRlLTA0CkZPWEEyO2NvYmluZGVyXzE7TTA3NjgxXzIuMDA7Wk5GMTc7MSwwMTcyNGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDc2ODFfMi4wMDtaTkYxNzsxLDAxNzI0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wOTIzNF8yLjAwO0lSRjM7MSwwMzM2OWUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDI1MjhfMi4wMDtMSU41NDsxLDA1OTcxZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMjUyOF8yLjAwO0xJTjU0OzEsMDU5NzFlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAyNTI4XzIuMDA7TElONTQ7MSwwNTk3MWUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDI1MjhfMi4wMDtMSU41NDsxLDA1OTcxZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzc3OF8yLjAwO1pORjIyNDsxLDA4MjcyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzc3OF8yLjAwO1pORjIyNDsxLDA4MjcyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzc3OF8yLjAwO1pORjIyNDsxLDA4MjcyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzc3OF8yLjAwO1pORjIyNDsxLDA4MjcyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzc3OF8yLjAwO1pORjIyNDsxLDA4MjcyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzc3OF8yLjAwO1pORjIyNDsxLDA4MjcyZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODkzMF8yLjAwO1pGUDgyOzEsMDg3NDJlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4OTYwXzIuMDA7Wk5GMzUwOzEsMDk5NzhlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4OTYwXzIuMDA7Wk5GMzUwOzEsMDk5NzhlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA3NzM2XzIuMDA7Wk5GODQ7MSwxMTAyOGUtMDMKRk9YQTI7Y29iaW5kZXJfNjtVTjAzMzYuMTtaTkY2NzE7MSwxNTIxOGUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTRfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTRfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTRfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTRfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTRfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTRfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQyOTRfMi4wMDtDUkVCM0w0LENSRUIzTDI7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQzMTFfMi4wMDtDUkVCM0wxLENSRUIzTDI7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQzMTFfMi4wMDtDUkVCM0wxLENSRUIzTDI7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQzMTFfMi4wMDtDUkVCM0wxLENSRUIzTDI7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNQTE0NzQuMTtDUkVCM0w0OzEsMTg5OTVlLTAzCkZPWEEyO2NvYmluZGVyXzU7TUExNDc0LjE7Q1JFQjNMNDsxLDE4OTk1ZS0wMwpGT1hBMjtjb2JpbmRlcl81O01BMTQ3NC4xO0NSRUIzTDQ7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNQTE0NzQuMTtDUkVCM0w0OzEsMTg5OTVlLTAzCkZPWEEyO2NvYmluZGVyXzU7TUExNDc0LjE7Q1JFQjNMNDsxLDE4OTk1ZS0wMwpGT1hBMjtjb2JpbmRlcl81O01BMTQ3NC4xO0NSRUIzTDQ7MSwxODk5NWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDE5ODNfMi4wMDtGT1hCMjsxLDIwMDU0ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODg5OF8yLjAwO1pORjIxNDsxLDI0MzYwZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODg5OF8yLjAwO1pORjIxNDsxLDI0MzYwZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMTY2OF8yLjAwO0FSSUQ1QTsxLDI3NDIyZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMTY2OF8yLjAwO0FSSUQ1QTsxLDI3NDIyZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMTY2OF8yLjAwO0FSSUQ1QTsxLDI3NDIyZS0wMwpGT1hBMjtjb2JpbmRlcl8wO01BMTk3Ny4xO1pORjMyNDsxLDMyNjQ0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO01BMTk3Ny4xO1pORjMyNDsxLDMyNjQ0ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMzMwMF8yLjAwO1BPVTFGMTsxLDM4MzE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMzMwMF8yLjAwO1BPVTFGMTsxLDM4MzE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMzMwMF8yLjAwO1BPVTFGMTsxLDM4MzE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMzMwMF8yLjAwO1BPVTFGMTsxLDM4MzE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMzMwMF8yLjAwO1BPVTFGMTsxLDM4MzE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODg3Ml8yLjAwO1pORjg1OzEsMzg5OTRlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4ODcyXzIuMDA7Wk5GODU7MSwzODk5NGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDEyNDZfMi4wMDtIRFg7MSw0NTM3NWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDEyNDZfMi4wMDtIRFg7MSw0NTM3NWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MjhfMi4wMDtMSU41NDsxLDQ1ODEzZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMjUyOF8yLjAwO0xJTjU0OzEsNDU4MTNlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAyNTI4XzIuMDA7TElONTQ7MSw0NTgxM2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MjhfMi4wMDtMSU41NDsxLDQ1ODEzZS0wMwpGT1hBMjtjb2JpbmRlcl83O00wMzMyNl8yLjAwO0hTRlkyLEhTRlgxLEhTRlgyOzEsNDgxNzllLTAzCkZPWEEyO2NvYmluZGVyXzc7TTAzMzI2XzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7MSw0ODE3OWUtMDMKRk9YQTI7Y29iaW5kZXJfNztNMDMzMjZfMi4wMDtIU0ZZMixIU0ZYMSxIU0ZYMjsxLDQ4MTc5ZS0wMwpGT1hBMjtjb2JpbmRlcl83O00wMzMyNl8yLjAwO0hTRlkyLEhTRlgxLEhTRlgyOzEsNDgxNzllLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAwMzYwXzIuMDA7UE9VNEYzOzEsNTA2MzVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAwMzYwXzIuMDA7UE9VNEYzOzEsNTA2MzVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAwMzYwXzIuMDA7UE9VNEYzOzEsNTA2MzVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAwMzYwXzIuMDA7UE9VNEYzOzEsNTA2MzVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAxMjQ2XzIuMDA7SERYOzEsNTA2MzVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAxMjQ2XzIuMDA7SERYOzEsNTA2MzVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAyNDMwXzIuMDA7TENPUjsxLDUyNTIwZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMjQzMF8yLjAwO0xDT1I7MSw1MjUyMGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDI1MzVfMi4wMDtMSU41NDsxLDUyNTIwZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMjUzNV8yLjAwO0xJTjU0OzEsNTI1MjBlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAyNTM1XzIuMDA7TElONTQ7MSw1MjUyMGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDI1MzVfMi4wMDtMSU41NDsxLDUyNTIwZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODM4MF8yLjAwO1pORjk4OzEsNTM0OTllLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4MzgwXzIuMDA7Wk5GOTg7MSw1MzQ5OWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDg4OTJfMi4wMDtaTkYzNDE7MSw1Njg0OWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNQTE2MjMuMTtTVEFUMjsxLDU4OTc1ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO01BMTYyMy4xO1NUQVQyOzEsNTg5NzVlLTAzCkZPWEEyO2NvYmluZGVyXzE7TUExNjIzLjE7U1RBVDI7MSw1ODk3NWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNQTE2MjMuMTtTVEFUMjsxLDU4OTc1ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO01BMTYyMy4xO1NUQVQyOzEsNTg5NzVlLTAzCkZPWEEyO2NvYmluZGVyXzE7VU4wNjIwLjE7Wk5GNDg1OzEsNjA5MjJlLTAzCkZPWEEyO2NvYmluZGVyXzc7TTA4Mzk2XzIuMDA7Wk5GMzUwOzEsNjM0NjdlLTAzCkZPWEEyO2NvYmluZGVyXzc7TTA4Mzk2XzIuMDA7Wk5GMzUwOzEsNjM0NjdlLTAzCkZPWEEyO2NvYmluZGVyXzc7VU4wNjEyLjE7Wk5GMzUwOzEsNjQ2MjVlLTAzCkZPWEEyO2NvYmluZGVyXzc7VU4wNjEyLjE7Wk5GMzUwOzEsNjQ2MjVlLTAzCkZPWEEyO2NvYmluZGVyXzM7VU4wMzEzLjE7WkZQOTE7MSw2NjY4NWUtMDMKRk9YQTI7Y29iaW5kZXJfMztVTjAzMTMuMTtaRlA5MTsxLDY2Njg1ZS0wMwpGT1hBMjtjb2JpbmRlcl8zO1VOMDMxMy4xO1pGUDkxOzEsNjY2ODVlLTAzCkZPWEEyO2NvYmluZGVyXzM7VU4wMzEzLjE7WkZQOTE7MSw2NjY4NWUtMDMKRk9YQTI7Y29iaW5kZXJfMztVTjAzMTMuMTtaRlA5MTsxLDY2Njg1ZS0wMwpGT1hBMjtjb2JpbmRlcl8zO1VOMDMxMy4xO1pGUDkxOzEsNjY2ODVlLTAzCkZPWEEyO2NvYmluZGVyXzM7VU4wMzEzLjE7WkZQOTE7MSw2NjY4NWUtMDMKRk9YQTI7Y29iaW5kZXJfNDtVTjAzMTMuMTtaRlA5MTsxLDY3NzkyZS0wMwpGT1hBMjtjb2JpbmRlcl80O1VOMDMxMy4xO1pGUDkxOzEsNjc3OTJlLTAzCkZPWEEyO2NvYmluZGVyXzQ7VU4wMzEzLjE7WkZQOTE7MSw2Nzc5MmUtMDMKRk9YQTI7Y29iaW5kZXJfNDtVTjAzMTMuMTtaRlA5MTsxLDY3NzkyZS0wMwpGT1hBMjtjb2JpbmRlcl80O1VOMDMxMy4xO1pGUDkxOzEsNjc3OTJlLTAzCkZPWEEyO2NvYmluZGVyXzQ7VU4wMzEzLjE7WkZQOTE7MSw2Nzc5MmUtMDMKRk9YQTI7Y29iaW5kZXJfNDtVTjAzMTMuMTtaRlA5MTsxLDY3NzkyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wOTAxNl8yLjAwO1NQNjsxLDY5Mzg0ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wOTAxNl8yLjAwO1NQNjsxLDY5Mzg0ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wOTAxNl8yLjAwO1NQNjsxLDY5Mzg0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMTY2Ml8yLjAwO0FSSUQzQixBUklEM0M7MSw3MDkxMmUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDE2NjJfMi4wMDtBUklEM0IsQVJJRDNDOzEsNzA5MTJlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAxNjYyXzIuMDA7QVJJRDNCLEFSSUQzQzsxLDcwOTEyZS0wMwpGT1hBMjtjb2JpbmRlcl82O00wODkxN18yLjAwO1pORjU1NDsxLDcyNzc1ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMTY2Ml8yLjAwO0FSSUQzQixBUklEM0M7MSw3Mzg4MWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDE2NjJfMi4wMDtBUklEM0IsQVJJRDNDOzEsNzM4ODFlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAxNjYyXzIuMDA7QVJJRDNCLEFSSUQzQzsxLDczODgxZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMjUyNV8yLjAwO0xJTjU0OzEsODE3NzNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAyNTI1XzIuMDA7TElONTQ7MSw4MTc3M2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDI1MjVfMi4wMDtMSU41NDsxLDgxNzczZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMjUyNV8yLjAwO0xJTjU0OzEsODE3NzNlLTAzCkZPWEEyO2NvYmluZGVyXzM7VU4wNTM1LjE7Rk9YTzE6OkVMRjE7MSw4MTgyNGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDc2ODFfMi4wMDtaTkYxNzsxLDgzNTA3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNzY4MV8yLjAwO1pORjE3OzEsODM1MDdlLTAzCkZPWEEyO2NvYmluZGVyXzY7TTA3NjkzXzIuMDA7Wk5GNTczOzEsODQyODNlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TTA4MjQ1XzIuMDA7Wk5GNDE7MSw4NDU1NmUtMDMKRk9YQTI7Y29iaW5kZXJfNDtNQTE1NzkuMTtaQlRCMjY7MSw4NDU1NmUtMDMKRk9YQTI7Y29iaW5kZXJfNDtNQTE1NzkuMTtaQlRCMjY7MSw4NDU1NmUtMDMKRk9YQTI7Y29iaW5kZXJfNjtNMDc3MjNfMi4wMDtaTkY4NjA7MSw4OTkxMWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDc3MjhfMi4wMDtaTkY4MTsxLDk4MjQ2ZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wNzcyOF8yLjAwO1pORjgxOzEsOTgyNDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA3NzI4XzIuMDA7Wk5GODE7MSw5ODI0NmUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDc2NzFfMi4wMDtaTkY5MzsxLDk4NDUxZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNzY3MV8yLjAwO1pORjkzOzEsOTg0NTFlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NjcxXzIuMDA7Wk5GOTM7MSw5ODQ1MWUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDc2NzFfMi4wMDtaTkY5MzsxLDk4NDUxZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMDM2MF8yLjAwO1BPVTRGMzsxLDk5MzY3ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMDM2MF8yLjAwO1BPVTRGMzsxLDk5MzY3ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMDM2MF8yLjAwO1BPVTRGMzsxLDk5MzY3ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMDM2MF8yLjAwO1BPVTRGMzsxLDk5MzY3ZS0wMwpGT1hBMjtjb2JpbmRlcl80O1VOMDYxMi4xO1pORjM1MDsyLDAxMzE2ZS0wMwpGT1hBMjtjb2JpbmRlcl80O1VOMDYxMi4xO1pORjM1MDsyLDAxMzE2ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMjQzMV8yLjAwO0xDT1I7MiwwNzc1MmUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDI0MzFfMi4wMDtMQ09SOzIsMDc3NTJlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAxNjY4XzIuMDA7QVJJRDVBOzIsMTE2NjVlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAxNjY4XzIuMDA7QVJJRDVBOzIsMTE2NjVlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAxNjY4XzIuMDA7QVJJRDVBOzIsMTE2NjVlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAyNDMwXzIuMDA7TENPUjsyLDExNjY1ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMjQzMF8yLjAwO0xDT1I7MiwxMTY2NWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgzNzJfMi4wMDtaTkYxNDA7MiwxMjI5NGUtMDMKRk9YQTI7Y29iaW5kZXJfNDtNQTA4OTcuMTtITVgyOzIsMTgwNzVlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TUEwODk3LjE7SE1YMjsyLDE4MDc1ZS0wMwpGT1hBMjtjb2JpbmRlcl80O01BMDg5OC4xO0hNWDM7MiwxODA3NWUtMDMKRk9YQTI7Y29iaW5kZXJfNDtNQTA4OTguMTtITVgzOzIsMTgwNzVlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TUEwODk4LjE7SE1YMzsyLDE4MDc1ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO1VOMDUxMy4xO0VUVjI6OkZPWEkxOzIsMjM2OTZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NTY1XzIuMDA7TkFOT0dQODsyLDI0MDMxZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wOTU2NV8yLjAwO05BTk9HUDg7MiwyNDAzMWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNQTE2MDcuMTtGT1hMMjsyLDI3NDkzZS0wMwpGT1hBMjtjb2JpbmRlcl8xO01BMTYwNy4xO0ZPWEwyOzIsMjc0OTNlLTAzCkZPWEEyO2NvYmluZGVyXzE7TUExNjA3LjE7Rk9YTDI7MiwyNzQ5M2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNQTE2MDcuMTtGT1hMMjsyLDI3NDkzZS0wMwpGT1hBMjtjb2JpbmRlcl8xO01BMTYwNy4xO0ZPWEwyOzIsMjc0OTNlLTAzCkZPWEEyO2NvYmluZGVyXzY7TTA0MDM5XzIuMDA7TUFGRzsyLDI3ODQxZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNzU5OF8yLjAwO1pORjc7MiwzNDM1NWUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDc1OThfMi4wMDtaTkY3OzIsMzQzNTVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NTk4XzIuMDA7Wk5GNzsyLDM0MzU1ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODMxMF8yLjAwO1pORjM0MTsyLDM0MzU1ZS0wMwpGT1hBMjtjb2JpbmRlcl82O00wNDA0MF8yLjAwO01BRkI7Miw0NjgwMWUtMDMKRk9YQTI7Y29iaW5kZXJfNjtNMDQwNDBfMi4wMDtNQUZCOzIsNDY4MDFlLTAzCkZPWEEyO2NvYmluZGVyXzY7TTA0MDQwXzIuMDA7TUFGQjsyLDQ2ODAxZS0wMwpGT1hBMjtjb2JpbmRlcl82O1VOMDYzOC4xO1pORjU4NjsyLDQ2ODAxZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wOTE3Nl8yLjAwO05BTk9HUDg7Miw0ODY1NmUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDkxNzZfMi4wMDtOQU5PR1A4OzIsNDg2NTZlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAyNTI1XzIuMDA7TElONTQ7Miw1MzExMWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MjVfMi4wMDtMSU41NDsyLDUzMTExZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMjUyNV8yLjAwO0xJTjU0OzIsNTMxMTFlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAyNTI1XzIuMDA7TElONTQ7Miw1MzExMWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MzVfMi4wMDtMSU41NDsyLDUzMTExZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMjUzNV8yLjAwO0xJTjU0OzIsNTMxMTFlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAyNTM1XzIuMDA7TElONTQ7Miw1MzExMWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MzVfMi4wMDtMSU41NDsyLDUzMTExZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wNDU0N18yLjAwO1pCVEIyNjsyLDU4MDE2ZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wNDU0N18yLjAwO1pCVEIyNjsyLDU4MDE2ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODMxOV8yLjAwO1pORjM4MjsyLDY0Nzk1ZS0wMwpGT1hBMjtjb2JpbmRlcl82O00wODgwN18yLjAwO01BRjsyLDY1NzU3ZS0wMwpGT1hBMjtjb2JpbmRlcl82O00wODgwN18yLjAwO01BRjsyLDY1NzU3ZS0wMwpGT1hBMjtjb2JpbmRlcl82O00wODgwN18yLjAwO01BRjsyLDY1NzU3ZS0wMwpGT1hBMjtjb2JpbmRlcl82O00wODgwN18yLjAwO01BRjsyLDY1NzU3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNzcxNF8yLjAwO1pORjQyOTsyLDY4NTg0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODM2MF8yLjAwO1pORjcwODsyLDY4NTg0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODM2MF8yLjAwO1pORjcwODsyLDY4NTg0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODM2MF8yLjAwO1pORjcwODsyLDY4NTg0ZS0wMwpGT1hBMjtjb2JpbmRlcl8zO00wNzc0N18yLjAwO1pORjgwODsyLDcyNjEyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODk1Ml8yLjAwO1pORjMzNTsyLDc0Mzc5ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODk1Ml8yLjAwO1pORjMzNTsyLDc0Mzc5ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODk1Ml8yLjAwO1pORjMzNTsyLDc0Mzc5ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODk1Ml8yLjAwO1pORjMzNTsyLDc0Mzc5ZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wODMxOV8yLjAwO1pORjM4MjsyLDc3NDM0ZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wODM4M18yLjAwO1pORjcxOzIsNzc0MzRlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA4OTQ4XzIuMDA7Wk5GNDE4OzIsNzg2MTRlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TTA3NzQ3XzIuMDA7Wk5GODA4OzIsODUwNzllLTAzCkZPWEEyO2NvYmluZGVyXzU7TTAyODQzXzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzIsODc5NDdlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTAyODQzXzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzIsODc5NDdlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTAyODQzXzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzIsODc5NDdlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA0MDE0XzIuMDA7Q1JFQjM7Miw4Nzk0N2UtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQwMTRfMi4wMDtDUkVCMzsyLDg3OTQ3ZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wNDAxNF8yLjAwO0NSRUIzOzIsODc5NDdlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA0MjM5XzIuMDA7Q1JFQjM7Miw4Nzk0N2UtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQyMzlfMi4wMDtDUkVCMzsyLDg3OTQ3ZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wNDIzOV8yLjAwO0NSRUIzOzIsODc5NDdlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA0MzEzXzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzIsODc5NDdlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA0MzEzXzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzIsODc5NDdlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA0MzEzXzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzIsODc5NDdlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA0NjQ2XzIuMDA7U1A5LFNQNjsyLDg3OTQ3ZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wNDY0Nl8yLjAwO1NQOSxTUDY7Miw4Nzk0N2UtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQ2NDZfMi4wMDtTUDksU1A2OzIsODc5NDdlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA0NjQ2XzIuMDA7U1A5LFNQNjsyLDg3OTQ3ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMTAwOF8yLjAwO0ZPWFIxOzIsOTIxMjFlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAxMDA4XzIuMDA7Rk9YUjE7Miw5MjEyMWUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDg4OTJfMi4wMDtaTkYzNDE7Miw5MzIyOWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDg4OTZfMi4wMDtaTkY0MTsyLDk1MjEzZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMDI1Ml8yLjAwO1pORjY1NTszLDAwNDE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMDI1Ml8yLjAwO1pORjY1NTszLDAwNDE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMjQzM18yLjAwO0xDT1I7MywwMDQxN2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDI0MzNfMi4wMDtMQ09SOzMsMDA0MTdlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAyMzk1XzIuMDA7TlIzQzI7MywwMTg5M2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDIzOTVfMi4wMDtOUjNDMjszLDAxODkzZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMjM5NV8yLjAwO05SM0MyOzMsMDE4OTNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAyMzk1XzIuMDA7TlIzQzI7MywwMTg5M2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgzMTNfMi4wMDtaTkY0MTszLDAyNjI2ZS0wMwpGT1hBMjtjb2JpbmRlcl82O00wMjg1Nl8yLjAwO01BRks7MywwMzY1OWUtMDMKRk9YQTI7Y29iaW5kZXJfNjtNMDI4NTZfMi4wMDtNQUZLOzMsMDM2NTllLTAzCkZPWEEyO2NvYmluZGVyXzY7VU4wNjM2LjE7Wk5GNTczOzMsMDM2NTllLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NzM2XzIuMDA7Wk5GODQ7MywwNzEyNGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDA3MTFfMi4wMDtDSUM7MywxMzM3N2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEwMDhfMi4wMDtGT1hSMTszLDEzMzc3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMTAwOF8yLjAwO0ZPWFIxOzMsMTMzNzdlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAyMDkzXzIuMDA7WkhYMTszLDEzMzc3ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMTg0OV8yLjAwO1pGSFgzOzMsMjEwNjllLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAxODQ5XzIuMDA7WkZIWDM7MywyMTA2OWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDE4NDlfMi4wMDtaRkhYMzszLDIxMDY5ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMTg0OV8yLjAwO1pGSFgzOzMsMjEwNjllLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAxODQ5XzIuMDA7WkZIWDM7MywyMTA2OWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDI0MzFfMi4wMDtMQ09SOzMsMjEwNjllLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAyNDMxXzIuMDA7TENPUjszLDIxMDY5ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzcwNl8yLjAwO1pORjc4MjszLDIxNjIzZS0wMwpGT1hBMjtjb2JpbmRlcl80O01BMDUxOC4xO1NUQVQ0OzMsMjI0MTZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TUExNDk4LjI7SE9YQTc7MywzNDU5M2UtMDMKRk9YQTI7Y29iaW5kZXJfNTtNQTE0OTguMjtIT1hBNzszLDM0NTkzZS0wMwpGT1hBMjtjb2JpbmRlcl81O01BMTQ5OC4yO0hPWEE3OzMsMzQ1OTNlLTAzCkZPWEEyO2NvYmluZGVyXzU7TUExNDk4LjI7SE9YQTc7MywzNDU5M2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtVTjA2MzMuMTtaTkY1Njc7MywzNTk2NGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtVTjA1MTMuMTtFVFYyOjpGT1hJMTszLDQ4NjA4ZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wNDcwNF8yLjAwO0UyRjg7Myw1MTgyM2UtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDg3MjhfMi4wMDtDTE9DSzszLDUxODIzZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wODcyOF8yLjAwO0NMT0NLOzMsNTE4MjNlLTAzCkZPWEEyO2NvYmluZGVyXzU7VU4wNjQ5LjE7Wk5GNjgxOzMsNTE4MjNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAwMjUwXzIuMDA7Wk5GNjU1OzMsNTI1NjdlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAwMjUwXzIuMDA7Wk5GNjU1OzMsNTI1NjdlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TTA4Mzk1XzIuMDA7Wk5GMjYwOzMsNTQ2MDBlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TTA4Mzk1XzIuMDA7Wk5GMjYwOzMsNTQ2MDBlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TTA4Mzk1XzIuMDA7Wk5GMjYwOzMsNTQ2MDBlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4Mzk1XzIuMDA7Wk5GMjYwOzMsNTg0ODhlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4Mzk1XzIuMDA7Wk5GMjYwOzMsNTg0ODhlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4Mzk1XzIuMDA7Wk5GMjYwOzMsNTg0ODhlLTAzCkZPWEEyO2NvYmluZGVyXzY7VU4wNjIzLjE7Wk5GNTAyOzMsNjA0ODRlLTAzCkZPWEEyO2NvYmluZGVyXzc7TUExOTc4LjE7Wk5GMzU0QTszLDYwNjIxZS0wMwpGT1hBMjtjb2JpbmRlcl83O01BMTk3OC4xO1pORjM1NEE7Myw2MDYyMWUtMDMKRk9YQTI7Y29iaW5kZXJfNztNQTE5NzguMTtaTkYzNTRBOzMsNjA2MjFlLTAzCkZPWEEyO2NvYmluZGVyXzc7TUExOTc4LjE7Wk5GMzU0QTszLDYwNjIxZS0wMwpGT1hBMjtjb2JpbmRlcl83O01BMTk3OC4xO1pORjM1NEE7Myw2MDYyMWUtMDMKRk9YQTI7Y29iaW5kZXJfNztNQTE5NzguMTtaTkYzNTRBOzMsNjA2MjFlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NzIyXzIuMDA7Wk5GNjc1OzMsNjQyODZlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NzIyXzIuMDA7Wk5GNjc1OzMsNjQyODZlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3Nzc4XzIuMDA7Wk5GMjI0OzMsNzA4MjNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3Nzc4XzIuMDA7Wk5GMjI0OzMsNzA4MjNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3Nzc4XzIuMDA7Wk5GMjI0OzMsNzA4MjNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3Nzc4XzIuMDA7Wk5GMjI0OzMsNzA4MjNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3Nzc4XzIuMDA7Wk5GMjI0OzMsNzA4MjNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3Nzc4XzIuMDA7Wk5GMjI0OzMsNzA4MjNlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA4MjY0XzIuMDA7Wk5GMjUwOzMsNzU4NjZlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA4MjY0XzIuMDA7Wk5GMjUwOzMsNzU4NjZlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4MzEzXzIuMDA7Wk5GNDE7Myw3NjQ2OWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDg4NzJfMi4wMDtaTkY4NTszLDc5NTkwZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODg3Ml8yLjAwO1pORjg1OzMsNzk1OTBlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA4OTM0XzIuMDA7Wk5GNzA4OzMsNzk1OTBlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA4OTM0XzIuMDA7Wk5GNzA4OzMsNzk1OTBlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA4OTM0XzIuMDA7Wk5GNzA4OzMsNzk1OTBlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TTA4MjcwXzIuMDA7WlNDQU4zMTszLDg2Nzc0ZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wODI3MF8yLjAwO1pTQ0FOMzE7Myw4Njc3NGUtMDMKRk9YQTI7Y29iaW5kZXJfNDtNMDgyNzBfMi4wMDtaU0NBTjMxOzMsODY3NzRlLTAzCkZPWEEyO2NvYmluZGVyXzA7VU4wMjM4LjE7Wk5GODIzOzMsOTA3OTRlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAxNjU2XzIuMDA7QVJJRDNCLEFSSUQzQzs0LDEyMzUyZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMTY1Nl8yLjAwO0FSSUQzQixBUklEM0M7NCwxMjM1MmUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDE2NTZfMi4wMDtBUklEM0IsQVJJRDNDOzQsMTIzNTJlLTAzCkZPWEEyO2NvYmluZGVyXzY7TTA0NjM5XzIuMDA7Wk5GNTgwOzQsMTUzMzVlLTAzCkZPWEEyO2NvYmluZGVyXzU7TUEwNzQzLjI7U0NSVDE7NCwxNTY1OGUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNQTA3NDMuMjtTQ1JUMTs0LDE1NjU4ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMTY1Nl8yLjAwO0FSSUQzQixBUklEM0M7NCwyMTE3MmUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDE2NTZfMi4wMDtBUklEM0IsQVJJRDNDOzQsMjExNzJlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAxNjU2XzIuMDA7QVJJRDNCLEFSSUQzQzs0LDIxMTcyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNDQxMl8yLjAwO1pORjgyMTs0LDIxOTQ2ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzcxNF8yLjAwO1pORjQyOTs0LDIzMTk2ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzc0N18yLjAwO1pORjgwODs0LDIzMTk2ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODM5Nl8yLjAwO1pORjM1MDs0LDIzMTk2ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODM5Nl8yLjAwO1pORjM1MDs0LDIzMTk2ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNzczMV8yLjAwO1pORjQ0OzQsMjkxODhlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NzMxXzIuMDA7Wk5GNDQ7NCwyOTE4OGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDc3MzFfMi4wMDtaTkY0NDs0LDI5MTg4ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNzczMV8yLjAwO1pORjQ0OzQsMjkxODhlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NzMxXzIuMDA7Wk5GNDQ7NCwyOTE4OGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDc3MzFfMi4wMDtaTkY0NDs0LDI5MTg4ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMTg0OV8yLjAwO1pGSFgzOzQsMjk4OTBlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAxODQ5XzIuMDA7WkZIWDM7NCwyOTg5MGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDE4NDlfMi4wMDtaRkhYMzs0LDI5ODkwZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMTg0OV8yLjAwO1pGSFgzOzQsMjk4OTBlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAxODQ5XzIuMDA7WkZIWDM7NCwyOTg5MGUtMDMKRk9YQTI7Y29iaW5kZXJfNztNMDg5MTRfMi4wMDtaTkYzNTRBOzQsMzI1NTBlLTAzCkZPWEEyO2NvYmluZGVyXzc7TTA4OTE0XzIuMDA7Wk5GMzU0QTs0LDMyNTUwZS0wMwpGT1hBMjtjb2JpbmRlcl83O00wODkxNF8yLjAwO1pORjM1NEE7NCwzMjU1MGUtMDMKRk9YQTI7Y29iaW5kZXJfNztNMDg5MTRfMi4wMDtaTkYzNTRBOzQsMzI1NTBlLTAzCkZPWEEyO2NvYmluZGVyXzc7TTA4OTE0XzIuMDA7Wk5GMzU0QTs0LDMyNTUwZS0wMwpGT1hBMjtjb2JpbmRlcl83O00wODkxNF8yLjAwO1pORjM1NEE7NCwzMjU1MGUtMDMKRk9YQTI7Y29iaW5kZXJfMztNQTE2NTIuMTtaS1NDQU41OzQsMzc4NDhlLTAzCkZPWEEyO2NvYmluZGVyXzM7TUExNjUyLjE7WktTQ0FONTs0LDM3ODQ4ZS0wMwpGT1hBMjtjb2JpbmRlcl8zO01BMTY1Mi4xO1pLU0NBTjU7NCwzNzg0OGUtMDMKRk9YQTI7Y29iaW5kZXJfMztNQTE2NTIuMTtaS1NDQU41OzQsMzc4NDhlLTAzCkZPWEEyO2NvYmluZGVyXzM7TUExOTM2LjE7RVJGOjpGT1hPMTs0LDM3ODQ4ZS0wMwpGT1hBMjtjb2JpbmRlcl82O00wNzY0MV8yLjAwO1pORjI2Njs0LDQ0Nzk1ZS0wMwpGT1hBMjtjb2JpbmRlcl82O1VOMDYwNi4xO1pORjI2Njs0LDQ0Nzk1ZS0wMwpGT1hBMjtjb2JpbmRlcl82O1VOMDYyMi4xO1pORjQ5Mjs0LDQ0Nzk1ZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wNDU0OF8yLjAwO1pCVEIyNjs0LDQ1NjIzZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wNDU0OF8yLjAwO1pCVEIyNjs0LDQ1NjIzZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNzYzOV8yLjAwO1pORjQxNzs0LDUzMzgxZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMjA5M18yLjAwO1pIWDE7NCw1Nzg1M2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MzBfMi4wMDtMSU41NDs0LDU3ODUzZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMjUzMF8yLjAwO0xJTjU0OzQsNTc4NTNlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAyNTMwXzIuMDA7TElONTQ7NCw1Nzg1M2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MzBfMi4wMDtMSU41NDs0LDU3ODUzZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNDYxMF8yLjAwO1pORjUwMTs0LDYxOTYyZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNDYxMF8yLjAwO1pORjUwMTs0LDYxOTYyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMjM5NV8yLjAwO05SM0MyOzQsNjgxMzJlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAyMzk1XzIuMDA7TlIzQzI7NCw2ODEzMmUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDIzOTVfMi4wMDtOUjNDMjs0LDY4MTMyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMjM5NV8yLjAwO05SM0MyOzQsNjgxMzJlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAyNTMwXzIuMDA7TElONTQ7NCw3MDM0OWUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDI1MzBfMi4wMDtMSU41NDs0LDcwMzQ5ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMjUzMF8yLjAwO0xJTjU0OzQsNzAzNDllLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAyNTMwXzIuMDA7TElONTQ7NCw3MDM0OWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgzOTVfMi4wMDtaTkYyNjA7NCw3MzA1OGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgzOTVfMi4wMDtaTkYyNjA7NCw3MzA1OGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgzOTVfMi4wMDtaTkYyNjA7NCw3MzA1OGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtVTjAyMzcuMTtaTkY4MjE7NCw3MzA1OGUtMDMKRk9YQTI7Y29iaW5kZXJfNjtNMDc3NDdfMi4wMDtaTkY4MDg7NCw3NDQ4N2UtMDMKRk9YQTI7Y29iaW5kZXJfNjtNMDgzNDFfMi4wMDtaTkY1NTQ7NCw3NDQ4N2UtMDMKRk9YQTI7Y29iaW5kZXJfNjtNQTE5ODcuMTtaTkY3MDE7NCw3NDQ4N2UtMDMKRk9YQTI7Y29iaW5kZXJfMztNMDc1OTVfMi4wMDtSQkFLOzQsNzc1NThlLTAzCkZPWEEyO2NvYmluZGVyXzM7TTA4Mzk1XzIuMDA7Wk5GMjYwOzQsNzc1NThlLTAzCkZPWEEyO2NvYmluZGVyXzM7TTA4Mzk1XzIuMDA7Wk5GMjYwOzQsNzc1NThlLTAzCkZPWEEyO2NvYmluZGVyXzM7TTA4Mzk1XzIuMDA7Wk5GMjYwOzQsNzc1NThlLTAzCkZPWEEyO2NvYmluZGVyXzM7VU4wMzM2LjE7Wk5GNjcxOzQsNzc1NThlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAwMjE5XzIuMDA7Wk5GMjAwOzQsODA2OTJlLTAzCkZPWEEyO2NvYmluZGVyXzY7TUEwMDg5LjI7TUFGRzo6TkZFMkwxOzQsODkwNDNlLTAzCkZPWEEyO2NvYmluZGVyXzY7VU4wMjMyLjE7Wk5GNzkzOzQsODkwNDNlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAwMjUyXzIuMDA7Wk5GNjU1OzQsOTQ5MTJlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAwMjUyXzIuMDA7Wk5GNjU1OzQsOTQ5MTJlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAyNDMzXzIuMDA7TENPUjs0LDk0OTEyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMjQzM18yLjAwO0xDT1I7NCw5NDkxMmUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDc3MjJfMi4wMDtaTkY2NzU7NSwwNTA5NGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDc3MjJfMi4wMDtaTkY2NzU7NSwwNTA5NGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDg5MTRfMi4wMDtaTkYzNTRBOzUsMDYyNDNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4OTE0XzIuMDA7Wk5GMzU0QTs1LDA2MjQzZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODkxNF8yLjAwO1pORjM1NEE7NSwwNjI0M2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDg5MTRfMi4wMDtaTkYzNTRBOzUsMDYyNDNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4OTE0XzIuMDA7Wk5GMzU0QTs1LDA2MjQzZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODkxNF8yLjAwO1pORjM1NEE7NSwwNjI0M2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDAxMTVfMi4wMDtBUklEM0IsQVJJRDNDOzUsMDk0MjdlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAwMTE1XzIuMDA7QVJJRDNCLEFSSUQzQzs1LDA5NDI3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMDExNV8yLjAwO0FSSUQzQixBUklEM0M7NSwwOTQyN2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDAyNTFfMi4wMDtaTkY2NTU7NSwwOTQyN2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDAyNTFfMi4wMDtaTkY2NTU7NSwwOTQyN2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMDVfMi4wMDtUSUdENjs1LDA5NDI3ZS0wMwpGT1hBMjtjb2JpbmRlcl83O00wNzc0N18yLjAwO1pORjgwODs1LDEyMTQwZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNzcxOF8yLjAwO1pORjY4Mjs1LDE0MTQ0ZS0wMwpGT1hBMjtjb2JpbmRlcl8zO1VOMDYxMi4xO1pORjM1MDs1LDE3MjUxZS0wMwpGT1hBMjtjb2JpbmRlcl8zO1VOMDYxMi4xO1pORjM1MDs1LDE3MjUxZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzU4MV8yLjAwO1pORjQ4NDs1LDIwOTM4ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzY3MV8yLjAwO1pORjkzOzUsMzk1NDVlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA3NjcxXzIuMDA7Wk5GOTM7NSwzOTU0NWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDc2NzFfMi4wMDtaTkY5Mzs1LDM5NTQ1ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzY3MV8yLjAwO1pORjkzOzUsMzk1NDVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NjIwXzIuMDA7Wk5GNTU4OzUsNDAyMzRlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4Mzc1XzIuMDA7Wk5GNTAyOzUsNDAyMzRlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NzY2XzIuMDA7Wk5GODc5OzUsNDU0OTdlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TTA4MjY1XzIuMDA7Wk5GMTM2OzUsNDc0ODhlLTAzCkZPWEEyO2NvYmluZGVyXzQ7VU4wNjAwLjE7Wk5GMTk1OzUsNDc0ODhlLTAzCkZPWEEyO2NvYmluZGVyXzQ7VU4wNjAwLjE7Wk5GMTk1OzUsNDc0ODhlLTAzCkZPWEEyO2NvYmluZGVyXzQ7VU4wNjIxLjE7Wk5GNDkxOzUsNDc0ODhlLTAzCkZPWEEyO2NvYmluZGVyXzQ7VU4wNjI5LjE7Wk5GNTQ0OzUsNDc0ODhlLTAzCkZPWEEyO2NvYmluZGVyXzQ7VU4wNjQ4LjE7Wk5GNjc0OzUsNTY3MThlLTAzCkZPWEEyO2NvYmluZGVyXzQ7VU4wNjQ4LjE7Wk5GNjc0OzUsNTY3MThlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAwMTE1XzIuMDA7QVJJRDNCLEFSSUQzQzs1LDYwNDg4ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMDExNV8yLjAwO0FSSUQzQixBUklEM0M7NSw2MDQ4OGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDAxMTVfMi4wMDtBUklEM0IsQVJJRDNDOzUsNjA0ODhlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAwNzExXzIuMDA7Q0lDOzUsNjU4NDJlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NTg2XzIuMDA7Wk5GMTQxOzUsNzQyMzVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NTg2XzIuMDA7Wk5GMTQxOzUsNzQyMzVlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA3NjA4XzIuMDA7Wk5GMzgyOzUsNzUwNjVlLTAzCkZPWEEyO2NvYmluZGVyXzY7TTA3NzY1XzIuMDA7Wk5GNDkyOzUsNzc0ODFlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAwMjUwXzIuMDA7Wk5GNjU1OzUsNzkzMDdlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAwMjUwXzIuMDA7Wk5GNjU1OzUsNzkzMDdlLTAzCkZPWEEyO2NvYmluZGVyXzM7TTA0NDc5XzIuMDA7Wk5GNjYwOzUsOTY1OTBlLTAzCkZPWEEyO2NvYmluZGVyXzM7TTA4OTYwXzIuMDA7Wk5GMzUwOzUsOTY1OTBlLTAzCkZPWEEyO2NvYmluZGVyXzM7TTA4OTYwXzIuMDA7Wk5GMzUwOzUsOTY1OTBlLTAzCkZPWEEyO2NvYmluZGVyXzM7VU4wMjExLjE7Wk5GNjYwOzUsOTY1OTBlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTAyODQ2XzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzYsMDE0NjFlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTAyODQ2XzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzYsMDE0NjFlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTAyODQ2XzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzYsMDE0NjFlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA0MDA5XzIuMDA7Q0VCUEU7NiwwMTQ2MWUtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDQwMDlfMi4wMDtDRUJQRTs2LDAxNDYxZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wNDAwOV8yLjAwO0NFQlBFOzYsMDE0NjFlLTAzCkZPWEEyO2NvYmluZGVyXzU7VU4wMzEyLjE7WkJUQjQyOzYsMDE0NjFlLTAzCkZPWEEyO2NvYmluZGVyXzU7VU4wMzEyLjE7WkJUQjQyOzYsMDE0NjFlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4MzA5XzIuMDA7Wk5GMzMxOzYsMTMzNjZlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4MzA5XzIuMDA7Wk5GMzMxOzYsMTMzNjZlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4MzA5XzIuMDA7Wk5GMzMxOzYsMTMzNjZlLTAzCkZPWEEyO2NvYmluZGVyXzc7TTA3NTk2XzIuMDA7Wk5GMTU3OzYsMTQxMjRlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA1ODUzXzIuMDA7WkZQODI7NiwxOTMzNWUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDg5NDhfMi4wMDtaTkY0MTg7NiwyMDc2N2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDkxNzZfMi4wMDtOQU5PR1A4OzYsMjA3NjdlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA5MTc2XzIuMDA7TkFOT0dQODs2LDIwNzY3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODg5OF8yLjAwO1pORjIxNDs2LDMyNzg1ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODg5OF8yLjAwO1pORjIxNDs2LDMyNzg1ZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wODg1OF8yLjAwO1pORjMyNDs2LDM4NzU3ZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wODg1OF8yLjAwO1pORjMyNDs2LDM4NzU3ZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wODg5Nl8yLjAwO1pORjQxOzYsNDM3OTJlLTAzCkZPWEEyO2NvYmluZGVyXzc7TTA4Mzc4XzIuMDA7WkZQMjg7Niw0ODAyN2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDc2MDhfMi4wMDtaTkYzODI7Niw1NzQwMWUtMDMKRk9YQTI7Y29iaW5kZXJfNztVTjA1ODQuMTtURUFENDo6RVRWNzs2LDYyNDgyZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMjA5OF8yLjAwO05BTk9HUDg7Niw2NzU0OGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDIwOThfMi4wMDtOQU5PR1A4OzYsNjc1NDhlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TTA4Mjc5XzIuMDA7Wk5GMzdBOzYsNzAwNTJlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TTA4Mjc5XzIuMDA7Wk5GMzdBOzYsNzAwNTJlLTAzCkZPWEEyO2NvYmluZGVyXzM7TUEwMDAyLjI7UlVOWDE7Niw3NDg4OGUtMDMKRk9YQTI7Y29iaW5kZXJfMztNQTAwMDIuMjtSVU5YMTs2LDc0ODg4ZS0wMwpGT1hBMjtjb2JpbmRlcl8zO01BMDAwMi4yO1JVTlgxOzYsNzQ4ODhlLTAzCkZPWEEyO2NvYmluZGVyXzM7TUEwMDAyLjI7UlVOWDE7Niw3NDg4OGUtMDMKRk9YQTI7Y29iaW5kZXJfMztNQTAwMDIuMjtSVU5YMTs2LDc0ODg4ZS0wMwpGT1hBMjtjb2JpbmRlcl8zO01BMDAwMi4yO1JVTlgxOzYsNzQ4ODhlLTAzCkZPWEEyO2NvYmluZGVyXzM7TUEwMDAyLjI7UlVOWDE7Niw3NDg4OGUtMDMKRk9YQTI7Y29iaW5kZXJfMztNQTAwMDIuMjtSVU5YMTs2LDc0ODg4ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wMDIxOV8yLjAwO1pORjIwMDs2LDc1NTc4ZS0wMwpGT1hBMjtjb2JpbmRlcl8zO00wOTIzNF8yLjAwO0lSRjM7Niw3NTg2NmUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgzODRfMi4wMDtaTkYxMjE7Niw3NzQ4M2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgzODRfMi4wMDtaTkYxMjE7Niw3NzQ4M2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgzODRfMi4wMDtaTkYxMjE7Niw3NzQ4M2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDg4NjBfMi4wMDtaTkYyNjQ7Niw3NzQ4M2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgyNzRfMi4wMDtaTkY1ODI7Niw4NDQzNGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgzMDlfMi4wMDtaTkYzMzE7Niw4NDQzNGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgzMDlfMi4wMDtaTkYzMzE7Niw4NDQzNGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDgzMDlfMi4wMDtaTkYzMzE7Niw4NDQzNGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMDdfMi4wMDtZQlgyLFlCWDM7Niw4Njg2NGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMDdfMi4wMDtZQlgyLFlCWDM7Niw4Njg2NGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMDdfMi4wMDtZQlgyLFlCWDM7Niw4Njg2NGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMDdfMi4wMDtZQlgyLFlCWDM7Niw4Njg2NGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMDdfMi4wMDtZQlgyLFlCWDM7Niw4Njg2NGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMDdfMi4wMDtZQlgyLFlCWDM7Niw4Njg2NGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMDdfMi4wMDtZQlgyLFlCWDM7Niw4Njg2NGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMDdfMi4wMDtZQlgyLFlCWDM7Niw4Njg2NGUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDIwOThfMi4wMDtOQU5PR1A4OzcsMDYyMjNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAyMDk4XzIuMDA7TkFOT0dQODs3LDA2MjIzZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzU5OF8yLjAwO1pORjc7NywwNjIyM2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDc1OThfMi4wMDtaTkY3OzcsMDYyMjNlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA3NTk4XzIuMDA7Wk5GNzs3LDA2MjIzZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzYzOV8yLjAwO1pORjQxNzs3LDA2MjIzZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODM4MF8yLjAwO1pORjk4OzcsMDYyMjNlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA4MzgwXzIuMDA7Wk5GOTg7NywwNjIyM2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNQTE5NzcuMTtaTkYzMjQ7NywwNjIyM2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNQTE5NzcuMTtaTkYzMjQ7NywwNjIyM2UtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDQzNzBfMi4wMDtNQUZHOzcsMDY1NTBlLTAzCkZPWEEyO2NvYmluZGVyXzY7VU4wMjUzLjE7TFlMMTs3LDA2ODU1ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO01BMTYwNy4xO0ZPWEwyOzcsMTMxNTVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TUExNjA3LjE7Rk9YTDI7NywxMzE1NWUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNQTE2MDcuMTtGT1hMMjs3LDEzMTU1ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO01BMTYwNy4xO0ZPWEwyOzcsMTMxNTVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TUExNjA3LjE7Rk9YTDI7NywxMzE1NWUtMDMKRk9YQTI7Y29iaW5kZXJfNztNMDc2MjBfMi4wMDtaTkY1NTg7NywxNjAwM2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDkwMTZfMi4wMDtTUDY7NywzNDQyN2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDkwMTZfMi4wMDtTUDY7NywzNDQyN2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDkwMTZfMi4wMDtTUDY7NywzNDQyN2UtMDMKRk9YQTI7Y29iaW5kZXJfNztNMDIwOThfMi4wMDtOQU5PR1A4OzcsMzk0ODhlLTAzCkZPWEEyO2NvYmluZGVyXzc7TTAyMDk4XzIuMDA7TkFOT0dQODs3LDM5NDg4ZS0wMwpGT1hBMjtjb2JpbmRlcl8zO00wODg5M18yLjAwO1ZFWkYxOzcsNTUwNzllLTAzCkZPWEEyO2NvYmluZGVyXzM7TTA4ODkzXzIuMDA7VkVaRjE7Nyw1NTA3OWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDc3MDVfMi4wMDtaTkY3OTk7Nyw1NTgwOWUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDc3MDVfMi4wMDtaTkY3OTk7Nyw1NTgwOWUtMDMKRk9YQTI7Y29iaW5kZXJfMztVTjAyMzguMTtaTkY4MjM7Nyw1ODkyOGUtMDMKRk9YQTI7Y29iaW5kZXJfNztNMDkzNDlfMi4wMDtORkFUQzE7Nyw3MjI1NGUtMDMKRk9YQTI7Y29iaW5kZXJfNztNMDkzNDlfMi4wMDtORkFUQzE7Nyw3MjI1NGUtMDMKRk9YQTI7Y29iaW5kZXJfNztNMDkzNDlfMi4wMDtORkFUQzE7Nyw3MjI1NGUtMDMKRk9YQTI7Y29iaW5kZXJfNztNMDkzNDlfMi4wMDtORkFUQzE7Nyw3MjI1NGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDg2MDlfMi4wMDtUQlBMMjs3LDgwMTI1ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODYwOV8yLjAwO1RCUEwyOzcsODAxMjVlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAxMjA1XzIuMDA7VElHRDY7Nyw5MTEwNWUtMDMKRk9YQTI7Y29iaW5kZXJfNDtNMDkwMzNfMi4wMDtFMkY3OzcsOTk4MDFlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTAyOTI5XzIuMDA7U0NSVDE7OCwwMTE0M2UtMDMKRk9YQTI7Y29iaW5kZXJfNTtNMDI5MjlfMi4wMDtTQ1JUMTs4LDAxMTQzZS0wMwpGT1hBMjtjb2JpbmRlcl81O00wODI0NV8yLjAwO1pORjQxOzgsMDExNDNlLTAzCkZPWEEyO2NvYmluZGVyXzU7TUEwMDY1LjI7UFBBUkc6OlJYUkE7OCwwMTE0M2UtMDMKRk9YQTI7Y29iaW5kZXJfNjtNMDc3NTNfMi4wMDtaTkY4MDU7OCwzNDE2MWUtMDMKRk9YQTI7Y29iaW5kZXJfNjtNMDg5NjBfMi4wMDtaTkYzNTA7OCwzNDE2MWUtMDMKRk9YQTI7Y29iaW5kZXJfNjtNMDg5NjBfMi4wMDtaTkYzNTA7OCwzNDE2MWUtMDMKRk9YQTI7Y29iaW5kZXJfMztNMDkxMDRfMi4wMDtGT1hCMjs4LDQyODk3ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODkwNF8yLjAwO1pORjM4Mjs4LDU0MDQyZS0wMwpGT1hBMjtjb2JpbmRlcl81O01BMDc0NC4yO1NDUlQyOzgsNjc2MTRlLTAzCkZPWEEyO2NvYmluZGVyXzU7TUExNTk5LjE7Wk5GNjgyOzgsNjc2MTRlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTA5NDc0XzIuMDA7TkVVUk9ENCxORVVST0Q2OzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTExMDU0XzIuMDA7TVlCOzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTExMDU0XzIuMDA7TVlCOzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTExMDU0XzIuMDA7TVlCOzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTExMDU0XzIuMDA7TVlCOzgsNzA0MDZlLTAzCkZPWEEyO2NvYmluZGVyXzc7TUExNjAxLjI7Wk5GNzVEOzgsNzk2NDNlLTAzCkZPWEEyO2NvYmluZGVyXzc7TUExNjAxLjI7Wk5GNzVEOzgsNzk2NDNlLTAzCkZPWEEyO2NvYmluZGVyXzc7TUExNjAxLjI7Wk5GNzVEOzgsNzk2NDNlLTAzCkZPWEEyO2NvYmluZGVyXzc7TUExNjAxLjI7Wk5GNzVEOzgsNzk2NDNlLTAzCkZPWEEyO2NvYmluZGVyXzc7TUExNjAxLjI7Wk5GNzVEOzgsNzk2NDNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NzY0XzIuMDA7Wk5GODgwOzgsODY2OTdlLTAzCkZPWEEyO2NvYmluZGVyXzc7VU4wMTYyLjE7Wk5GMTM0OzgsOTgxNThlLTAzCkZPWEEyO2NvYmluZGVyXzc7VU4wMzEzLjE7WkZQOTE7OSwwMTEzNmUtMDMKRk9YQTI7Y29iaW5kZXJfNztVTjAzMTMuMTtaRlA5MTs5LDAxMTM2ZS0wMwpGT1hBMjtjb2JpbmRlcl83O1VOMDMxMy4xO1pGUDkxOzksMDExMzZlLTAzCkZPWEEyO2NvYmluZGVyXzc7VU4wMzEzLjE7WkZQOTE7OSwwMTEzNmUtMDMKRk9YQTI7Y29iaW5kZXJfNztVTjAzMTMuMTtaRlA5MTs5LDAxMTM2ZS0wMwpGT1hBMjtjb2JpbmRlcl83O1VOMDMxMy4xO1pGUDkxOzksMDExMzZlLTAzCkZPWEEyO2NvYmluZGVyXzc7VU4wMzEzLjE7WkZQOTE7OSwwMTEzNmUtMDMKRk9YQTI7Y29iaW5kZXJfNjtNMDgyNDVfMi4wMDtaTkY0MTs5LDAyNTE1ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODk1Ml8yLjAwO1pORjMzNTs5LDA1NDM5ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODk1Ml8yLjAwO1pORjMzNTs5LDA1NDM5ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODk1Ml8yLjAwO1pORjMzNTs5LDA1NDM5ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODk1Ml8yLjAwO1pORjMzNTs5LDA1NDM5ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO1VOMDIzOC4xO1pORjgyMzs5LDA5MTc1ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wNzc2NF8yLjAwO1pORjg4MDs5LDE4ODgzZS0wMwpGT1hBMjtjb2JpbmRlcl8zO00wOTAzMF8yLjAwO0UyRjE7OSwyNjc5NWUtMDMKRk9YQTI7Y29iaW5kZXJfMztNMDkwMzBfMi4wMDtFMkYxOzksMjY3OTVlLTAzCkZPWEEyO2NvYmluZGVyXzM7TTA5MDMwXzIuMDA7RTJGMTs5LDI2Nzk1ZS0wMwpGT1hBMjtjb2JpbmRlcl8zO00wOTAzMF8yLjAwO0UyRjE7OSwyNjc5NWUtMDMKRk9YQTI7Y29iaW5kZXJfMztNQTA1MTguMTtTVEFUNDs5LDI2Nzk1ZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wNzU5MF8yLjAwO1pORjI4Nzs5LDMyMTQ1ZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wNzU5MF8yLjAwO1pORjI4Nzs5LDMyMTQ1ZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wODMxM18yLjAwO1pORjQxOzksMzIxNDVlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAwMjUxXzIuMDA7Wk5GNjU1OzksMzMxMDNlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTAwMjUxXzIuMDA7Wk5GNjU1OzksMzMxMDNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA3NjMzXzIuMDA7WklLMTs5LDM3NjE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODI2MF8yLjAwO1pORjQ2Nzs5LDM3NjE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODI2MF8yLjAwO1pORjQ2Nzs5LDM3NjE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODM5Nl8yLjAwO1pORjM1MDs5LDM3NjE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODM5Nl8yLjAwO1pORjM1MDs5LDM3NjE3ZS0wMwpGT1hBMjtjb2JpbmRlcl83O1VOMDIyMi4xO1pORjc2NTs5LDQxMzE2ZS0wMwpGT1hBMjtjb2JpbmRlcl8xO00wODg5M18yLjAwO1ZFWkYxOzksNDEzNzBlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA4ODkzXzIuMDA7VkVaRjE7OSw0MTM3MGUtMDMKRk9YQTI7Y29iaW5kZXJfMTtNMDc2MzNfMi4wMDtaSUsxOzksNDkyOTdlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA4MzEwXzIuMDA7Wk5GMzQxOzksNDkyOTdlLTAzCkZPWEEyO2NvYmluZGVyXzE7TTA4MzgyXzIuMDA7Wk5GNjc3OzksNDkyOTdlLTAzCkZPWEEyO2NvYmluZGVyXzA7VU4wNjIwLjE7Wk5GNDg1OzksNTAyMTBlLTAzCkZPWEEyO2NvYmluZGVyXzc7TTA4MzgwXzIuMDA7Wk5GOTg7OSw2MTcyM2UtMDMKRk9YQTI7Y29iaW5kZXJfNztNMDgzODBfMi4wMDtaTkY5ODs5LDYxNzIzZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNTQ2OV8yLjAwO1BPVTJGMzs5LDY0MDY0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNTQ2OV8yLjAwO1BPVTJGMzs5LDY0MDY0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNTQ2OV8yLjAwO1BPVTJGMzs5LDY0MDY0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNTQ2OV8yLjAwO1BPVTJGMzs5LDY0MDY0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNTQ2OV8yLjAwO1BPVTJGMzs5LDY0MDY0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNTQ2OV8yLjAwO1BPVTJGMzs5LDY0MDY0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNTQ2OV8yLjAwO1BPVTJGMzs5LDY0MDY0ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO1VOMDUzOC4xO0ZPWFMxOzksNjQwNjRlLTAzCkZPWEEyO2NvYmluZGVyXzA7VU4wNTM4LjE7Rk9YUzE7OSw2NDA2NGUtMDMKRk9YQTI7Y29iaW5kZXJfNDtNMDMzMjZfMi4wMDtIU0ZZMixIU0ZYMSxIU0ZYMjs5LDc2NjYzZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wMzMyNl8yLjAwO0hTRlkyLEhTRlgxLEhTRlgyOzksNzY2NjNlLTAzCkZPWEEyO2NvYmluZGVyXzQ7TTAzMzI2XzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7OSw3NjY2M2UtMDMKRk9YQTI7Y29iaW5kZXJfNDtNMDMzMjZfMi4wMDtIU0ZZMixIU0ZYMSxIU0ZYMjs5LDc2NjYzZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wOTM0OV8yLjAwO05GQVRDMTs5LDc2NjYzZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wOTM0OV8yLjAwO05GQVRDMTs5LDc2NjYzZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wOTM0OV8yLjAwO05GQVRDMTs5LDc2NjYzZS0wMwpGT1hBMjtjb2JpbmRlcl80O00wOTM0OV8yLjAwO05GQVRDMTs5LDc2NjYzZS0wMwpGT1hBMjtjb2JpbmRlcl80O1VOMDY2MS4xO1pORjc5OzksNzY2NjNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAxMjEwXzIuMDA7Q1hYQzUsQ1hYQzQsVEVUMzs5LDc4OTYzZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMTIxMF8yLjAwO0NYWEM1LENYWEM0LFRFVDM7OSw3ODk2M2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMTBfMi4wMDtDWFhDNSxDWFhDNCxURVQzOzksNzg5NjNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAxMjEwXzIuMDA7Q1hYQzUsQ1hYQzQsVEVUMzs5LDc4OTYzZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wMTIxMF8yLjAwO0NYWEM1LENYWEM0LFRFVDM7OSw3ODk2M2UtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMTBfMi4wMDtDWFhDNSxDWFhDNCxURVQzOzksNzg5NjNlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTAxMjEwXzIuMDA7Q1hYQzUsQ1hYQzQsVEVUMzs5LDc4OTYzZS0wMwpGT1hBMjtjb2JpbmRlcl82O1VOMDMzNy4xO1pORjY3Nzs5LDkxNDE3ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wODc5NF8yLjAwO0JBVEYzOzksOTE4ODVlLTAzCkZPWEEyO2NvYmluZGVyXzA7TTA4Nzk0XzIuMDA7QkFURjM7OSw5MTg4NWUtMDMKRk9YQTI7Y29iaW5kZXJfMDtNMDg3OTRfMi4wMDtCQVRGMzs5LDkxODg1ZS0wMwpGT1hBMjtjb2JpbmRlcl8wO00wNzY5N18yLjAwO1pORjc5OzksOTI2NjFlLTAzCkZPWEEyO2NvYmluZGVyXzU7TTAzMTM0XzIuMDA7SE9YQzExOzksOTQxMjllLTAzCkZPWEEyO2NvYmluZGVyXzY7TTA3NjcxXzIuMDA7Wk5GOTM7MSwwMDUyN2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc2NzFfMi4wMDtaTkY5MzsxLDAwNTI3ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNzY3MV8yLjAwO1pORjkzOzEsMDA1MjdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NjcxXzIuMDA7Wk5GOTM7MSwwMDUyN2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDI4MzVfMi4wMDtOUkw7MSwwMDY2M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDI4MzVfMi4wMDtOUkw7MSwwMDY2M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDI4MzVfMi4wMDtOUkw7MSwwMDY2M2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDc1OTJfMi4wMDtaRlAxNDsxLDAxMDYyZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wNzczM18yLjAwO1pORjgyMzsxLDAxMDYyZS0wMgpGT1hBMjtjb2JpbmRlcl8zO01BMTU3OS4xO1pCVEIyNjsxLDAxMDYyZS0wMgpGT1hBMjtjb2JpbmRlcl8zO01BMTU3OS4xO1pCVEIyNjsxLDAxMDYyZS0wMgpGT1hBMjtjb2JpbmRlcl8zO01BMTk3Mi4xO1pGUDE0OzEsMDEwNjJlLTAyCkZPWEEyO2NvYmluZGVyXzM7VU4wNTQxLjE7R0NNMTo6RUxLMTsxLDAxMDYyZS0wMgpGT1hBMjtjb2JpbmRlcl8zO1VOMDY2NC4xO1pORjg2MDsxLDAxMDYyZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wMzgxOV8yLjAwO1RQUlgxOzEsMDExNDNlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzEsMDIwMjZlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzEsMDIwMjZlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzEsMDIwMjZlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzEsMDIwMjZlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzEsMDIwMjZlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzEsMDIwMjZlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzEsMDIwMjZlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzEsMDIwMjZlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjEwXzIuMDA7Q1hYQzUsQ1hYQzQsVEVUMzsxLDAyMDI2ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMTIxMF8yLjAwO0NYWEM1LENYWEM0LFRFVDM7MSwwMjAyNmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDEyMTBfMi4wMDtDWFhDNSxDWFhDNCxURVQzOzEsMDIwMjZlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjEwXzIuMDA7Q1hYQzUsQ1hYQzQsVEVUMzsxLDAyMDI2ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMTIxMF8yLjAwO0NYWEM1LENYWEM0LFRFVDM7MSwwMjAyNmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDEyMTBfMi4wMDtDWFhDNSxDWFhDNCxURVQzOzEsMDIwMjZlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjEwXzIuMDA7Q1hYQzUsQ1hYQzQsVEVUMzsxLDAyMDI2ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMjg1NF8yLjAwO01BRkc7MSwwMjQ4MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc3MTRfMi4wMDtaTkY0Mjk7MSwwMjQ4MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtVTjA2NDcuMTtaTkY2NjQ7MSwwMjQ4MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtVTjA2NDcuMTtaTkY2NjQ7MSwwMjQ4MWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg4OThfMi4wMDtaTkYyMTQ7MSwwMjUyNWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg4OThfMi4wMDtaTkYyMTQ7MSwwMjUyNWUtMDIKRk9YQTI7Y29iaW5kZXJfNztVTjA2NzEuMTtEVVhCTDE7MSwwMjU3NGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDc2OTdfMi4wMDtaTkY3OTsxLDAyNzg3ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODM2MF8yLjAwO1pORjcwODsxLDA0NTc1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODM2MF8yLjAwO1pORjcwODsxLDA0NTc1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODM2MF8yLjAwO1pORjcwODsxLDA0NTc1ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNzc3OF8yLjAwO1pORjIyNDsxLDA1MTc2ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNzc3OF8yLjAwO1pORjIyNDsxLDA1MTc2ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNzc3OF8yLjAwO1pORjIyNDsxLDA1MTc2ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNzc3OF8yLjAwO1pORjIyNDsxLDA1MTc2ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNzc3OF8yLjAwO1pORjIyNDsxLDA1MTc2ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNzc3OF8yLjAwO1pORjIyNDsxLDA1MTc2ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMDM3MF8yLjAwO05SMkUzOzEsMDU4MTNlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAwMzcwXzIuMDA7TlIyRTM7MSwwNTgxM2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDAzNzBfMi4wMDtOUjJFMzsxLDA1ODEzZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMDM3MF8yLjAwO05SMkUzOzEsMDU4MTNlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAwMzcwXzIuMDA7TlIyRTM7MSwwNTgxM2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDk1MjJfMi4wMDtFMkY3OzEsMDY5ODdlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUEwNjI0LjI7TkZBVEMxOzEsMDY5ODdlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUEwNjI0LjI7TkZBVEMxOzEsMDY5ODdlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUEwNjI0LjI7TkZBVEMxOzEsMDY5ODdlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUEwNjI0LjI7TkZBVEMxOzEsMDY5ODdlLTAyCkZPWEEyO2NvYmluZGVyXzE7VU4wMzM3LjE7Wk5GNjc3OzEsMDcxNTdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA1ODU2XzIuMDA7WktTQ0FONzsxLDA4MDI0ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNTg1Nl8yLjAwO1pLU0NBTjc7MSwwODAyNGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDU4NTZfMi4wMDtaS1NDQU43OzEsMDgwMjRlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA1ODU2XzIuMDA7WktTQ0FONzsxLDA4MDI0ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNTg1Nl8yLjAwO1pLU0NBTjc7MSwwODAyNGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg5NTJfMi4wMDtaTkYzMzU7MSwwODgyOGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg5NTJfMi4wMDtaTkYzMzU7MSwwODgyOGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg5NTJfMi4wMDtaTkYzMzU7MSwwODgyOGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg5NTJfMi4wMDtaTkYzMzU7MSwwODgyOGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg5NTNfMi4wMDtaTkY2Njc7MSwxMTAwOWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDc3NTNfMi4wMDtaTkY4MDU7MSwxMTE2N2UtMDIKRk9YQTI7Y29iaW5kZXJfMDtNQTE3MzEuMTtaTkY3Njg7MSwxMTE2N2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDgzNzVfMi4wMDtaTkY1MDI7MSwxMTI3N2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE3MjYuMTtaTkYzMzE7MSwxMTMyNmUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE3MjYuMTtaTkYzMzE7MSwxMTMyNmUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE3MjYuMTtaTkYzMzE7MSwxMTMyNmUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDM2NDFfMi4wMDtDUkVCM0wyOzEsMTE3NzBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MDQyXzIuMDA7QVRGNkI7MSwxMTc3MGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQwNDJfMi4wMDtBVEY2QjsxLDExNzcwZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDA0Ml8yLjAwO0FURjZCOzEsMTE3NzBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MTg0XzIuMDA7TVNDOzEsMTE3NzBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MTg0XzIuMDA7TVNDOzEsMTE3NzBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MTg0XzIuMDA7TVNDOzEsMTE3NzBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MTg0XzIuMDA7TVNDOzEsMTE3NzBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0NjQ1XzIuMDA7U1A5LFNQNjsxLDExNzcwZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDY0NV8yLjAwO1NQOSxTUDY7MSwxMTc3MGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQ2NDVfMi4wMDtTUDksU1A2OzEsMTE3NzBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0NjQ1XzIuMDA7U1A5LFNQNjsxLDExNzcwZS0wMgpGT1hBMjtjb2JpbmRlcl81O01BMTU2NC4xO1NQOTsxLDExNzcwZS0wMgpGT1hBMjtjb2JpbmRlcl8wO01BMTk3Ni4xO1pORjMyMDsxLDEyMjY1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODI1NF8yLjAwO1pORjYyMTsxLDEyOTg3ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTY2M18yLjAwO0FSSUQ1QTsxLDEzMzcwZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTY2M18yLjAwO0FSSUQ1QTsxLDEzMzcwZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTY2M18yLjAwO0FSSUQ1QTsxLDEzMzcwZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNzk3OF8yLjAwO0lSRjQ7MSwxMzQzMGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDc5NzhfMi4wMDtJUkY0OzEsMTM0MzBlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3OTc4XzIuMDA7SVJGNDsxLDEzNDMwZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNzk3OF8yLjAwO0lSRjQ7MSwxMzQzMGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg3OTlfMi4wMDtCQVRGOzEsMTM0MzBlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4Nzk5XzIuMDA7QkFURjsxLDEzNDMwZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODc5OV8yLjAwO0JBVEY7MSwxMzQzMGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg3OTlfMi4wMDtCQVRGOzEsMTM0MzBlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3NzYyXzIuMDA7Wk5GODkxOzEsMTUwOThlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA5MTc2XzIuMDA7TkFOT0dQODsxLDE1MzIxZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wOTE3Nl8yLjAwO05BTk9HUDg7MSwxNTMyMWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg5NDlfMi4wMDtaRlAyODsxLDE1NDEwZS0wMgpGT1hBMjtjb2JpbmRlcl82O01BMDExNy4yO01BRkI7MSwxNjc3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTAxMTcuMjtNQUZCOzEsMTY3NzllLTAyCkZPWEEyO2NvYmluZGVyXzY7TUEwMTE3LjI7TUFGQjsxLDE2Nzc5ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODg5Nl8yLjAwO1pORjQxOzEsMTc0NTllLTAyCkZPWEEyO2NvYmluZGVyXzM7VU4wMjIyLjE7Wk5GNzY1OzEsMTc4MDZlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA4MzEzXzIuMDA7Wk5GNDE7MSwxODk2MmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDM0NDlfMi4wMDtORkFUQzE7MSwxOTQzN2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDM0NDlfMi4wMDtORkFUQzE7MSwxOTQzN2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDM0NDlfMi4wMDtORkFUQzE7MSwxOTQzN2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDM0NDlfMi4wMDtORkFUQzE7MSwxOTQzN2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDc2OTNfMi4wMDtaTkY1NzM7MSwxOTkzMGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNQTE5NzcuMTtaTkYzMjQ7MSwxOTkzMGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNQTE5NzcuMTtaTkYzMjQ7MSwxOTkzMGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtVTjA2MzYuMTtaTkY1NzM7MSwxOTkzMGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE2NjNfMi4wMDtBUklENUE7MSwyMDc2OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE2NjNfMi4wMDtBUklENUE7MSwyMDc2OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE2NjNfMi4wMDtBUklENUE7MSwyMDc2OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDc1ODZfMi4wMDtaTkYxNDE7MSwyMTEyMmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDc1ODZfMi4wMDtaTkYxNDE7MSwyMTEyMmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDg4NThfMi4wMDtaTkYzMjQ7MSwyMjczOWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDg4NThfMi4wMDtaTkYzMjQ7MSwyMjczOWUtMDIKRk9YQTI7Y29iaW5kZXJfMztVTjAyNjQuMTtTUDc7MSwyMzMxNWUtMDIKRk9YQTI7Y29iaW5kZXJfMztVTjAyNjQuMTtTUDc7MSwyMzMxNWUtMDIKRk9YQTI7Y29iaW5kZXJfMztVTjAyNjQuMTtTUDc7MSwyMzMxNWUtMDIKRk9YQTI7Y29iaW5kZXJfMztVTjAyNjQuMTtTUDc7MSwyMzMxNWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTA1MDEuMTtNQUY6Ok5GRTI7MSwyMzQxM2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTA3ODIuMjtQS05PWDE7MSwyMzQxM2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTA3ODIuMjtQS05PWDE7MSwyMzQxM2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE1NzkuMTtaQlRCMjY7MSwyMzQxM2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE1NzkuMTtaQlRCMjY7MSwyMzQxM2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDgzNzNfMi4wMDtaTkY3NzQ7MSwyNTA2MGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDQ2NDFfMi4wMDtaTkY1ODA7MSwyNTc2NWUtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDQ0ODBfMi4wMDtaTkY2NjA7MSwyNjE2OGUtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDc1NjVfMi4wMDtaTkY1MDY7MSwyNjE2OGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQ0ODlfMi4wMDtLTEYxMDsxLDI2NTUxZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDQ4OV8yLjAwO0tMRjEwOzEsMjY1NTFlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0NDg5XzIuMDA7S0xGMTA7MSwyNjU1MWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQ0ODlfMi4wMDtLTEYxMDsxLDI2NTUxZS0wMgpGT1hBMjtjb2JpbmRlcl8xO1VOMDY2Ny4xO1pORjk4OzEsMjY1NjhlLTAyCkZPWEEyO2NvYmluZGVyXzE7VU4wNjY3LjE7Wk5GOTg7MSwyNjU2OGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDAzNjNfMi4wMDtQT1U2RjI7MSwyNjc3N2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDAzNjNfMi4wMDtQT1U2RjI7MSwyNjc3N2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDAzNjNfMi4wMDtQT1U2RjI7MSwyNjc3N2UtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDg5MzJfMi4wMDtaTkY0Njc7MSwyNzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDg5MzJfMi4wMDtaTkY0Njc7MSwyNzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfNztVTjA2NjcuMTtaTkY5ODsxLDI3ODU4ZS0wMgpGT1hBMjtjb2JpbmRlcl83O1VOMDY2Ny4xO1pORjk4OzEsMjc4NThlLTAyCkZPWEEyO2NvYmluZGVyXzc7TUExNTgxLjE7WkJUQjY7MSwzMDE3N2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNQTE1ODEuMTtaQlRCNjsxLDMwMTc3ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wODI0N18yLjAwO1pORjM4MjsxLDMwNDU4ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzc0N18yLjAwO1pORjgwODsxLDMxNjk3ZS0wMgpGT1hBMjtjb2JpbmRlcl82O01BMTU4MS4xO1pCVEI2OzEsMzI4NjhlLTAyCkZPWEEyO2NvYmluZGVyXzY7TUExNTgxLjE7WkJUQjY7MSwzMjg2OGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDc3NTNfMi4wMDtaTkY4MDU7MSwzNDE1N2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU1MjJfMi4wMDtIU0Y1LEhTRlgxLEhTRlgyOzEsMzQyNDVlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA1NTIyXzIuMDA7SFNGNSxIU0ZYMSxIU0ZYMjsxLDM0MjQ1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNTUyMl8yLjAwO0hTRjUsSFNGWDEsSFNGWDI7MSwzNDI0NWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU1MjJfMi4wMDtIU0Y1LEhTRlgxLEhTRlgyOzEsMzQyNDVlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wNjI1LjE7Wk5GNTI3OzEsMzU0ODZlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAyNTI2XzIuMDA7TElONTQ7MSwzNjUzM2UtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDI1MjZfMi4wMDtMSU41NDsxLDM2NTMzZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMjUyNl8yLjAwO0xJTjU0OzEsMzY1MzNlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAyNTI2XzIuMDA7TElONTQ7MSwzNjUzM2UtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDMzMDdfMi4wMDtQT1UyRjM7MSwzODI0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDMzMDdfMi4wMDtQT1UyRjM7MSwzODI0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDMzMDdfMi4wMDtQT1UyRjM7MSwzODI0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDMzMDdfMi4wMDtQT1UyRjM7MSwzODI0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDMzMDdfMi4wMDtQT1UyRjM7MSwzODI0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDMzMDdfMi4wMDtQT1UyRjM7MSwzODI0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDMzMDdfMi4wMDtQT1UyRjM7MSwzODI0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg5NDNfMi4wMDtaTkY1NjM7MSwzOTA1OWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDc3NDZfMi4wMDtaTkY1ODc7MSwzOTc3OGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDg4OTZfMi4wMDtaTkY0MTsxLDM5Nzc4ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODM3NV8yLjAwO1pORjUwMjsxLDQwNTAyZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzY4M18yLjAwO1pORjc1RDsxLDQxNDc5ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzY4M18yLjAwO1pORjc1RDsxLDQxNDc5ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzY4M18yLjAwO1pORjc1RDsxLDQxNDc5ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzY4M18yLjAwO1pORjc1RDsxLDQxNDc5ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzY4M18yLjAwO1pORjc1RDsxLDQxNDc5ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNzczNl8yLjAwO1pORjg0OzEsNDM0NzRlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA3NjkyXzIuMDA7Wk5GNTY3OzEsNDQxMDNlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA3NzA2XzIuMDA7Wk5GNzgyOzEsNDQxMDNlLTAyCkZPWEEyO2NvYmluZGVyXzE7VU4wNTM4LjE7Rk9YUzE7MSw0NjE4MGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtVTjA1MzguMTtGT1hTMTsxLDQ2MTgwZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wNzU5NV8yLjAwO1JCQUs7MSw0NjgwN2UtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDc3MjlfMi4wMDtaTkY3ODBBOzEsNDY5ODhlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA3NzYyXzIuMDA7Wk5GODkxOzEsNDcwMTVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4MzQxXzIuMDA7Wk5GNTU0OzEsNDcwMTVlLTAyCkZPWEEyO2NvYmluZGVyXzA7VU4wNTk4LjE7Wk5GMTg0OzEsNDcwMTVlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA1ODQ4XzIuMDA7WkZQMTQ7MSw0NzU0NGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDI0MzVfMi4wMDtMQ09SOzEsNDc3MjdlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAyNDM1XzIuMDA7TENPUjsxLDQ3NzI3ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDYxMF8yLjAwO1pORjUwMTsxLDQ4NzQ4ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDYxMF8yLjAwO1pORjUwMTsxLDQ4NzQ4ZS0wMgpGT1hBMjtjb2JpbmRlcl81O01BMTcwOS4xO1pJTTM7MSw0ODc0OGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNQTE3MDkuMTtaSU0zOzEsNDg3NDhlLTAyCkZPWEEyO2NvYmluZGVyXzU7TUExNzI5LjE7Wk5GNjgwOzEsNDg3NDhlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4ODU4XzIuMDA7Wk5GMzI0OzEsNDg4NDVlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4ODU4XzIuMDA7Wk5GMzI0OzEsNDg4NDVlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA0ODU3XzIuMDA7Rk9YUjI7MSw0ODk1MmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU4NTZfMi4wMDtaS1NDQU43OzEsNDg5NTJlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA1ODU2XzIuMDA7WktTQ0FONzsxLDQ4OTUyZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNTg1Nl8yLjAwO1pLU0NBTjc7MSw0ODk1MmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU4NTZfMi4wMDtaS1NDQU43OzEsNDg5NTJlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA1ODU2XzIuMDA7WktTQ0FONzsxLDQ4OTUyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTIwM18yLjAwO0NFTlBCRDE7MSw0OTQ1M2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDgzOTZfMi4wMDtaTkYzNTA7MSw1MDUzNmUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDgzOTZfMi4wMDtaTkYzNTA7MSw1MDUzNmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDg5MTdfMi4wMDtaTkY1NTQ7MSw1MDY5M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE2NTUuMTtaTkYzNDE7MSw1MzQ2NWUtMDIKRk9YQTI7Y29iaW5kZXJfMztVTjAyNDUuMTtaU0NBTjIwOzEsNTM5MDVlLTAyCkZPWEEyO2NvYmluZGVyXzM7VU4wMjQ1LjE7WlNDQU4yMDsxLDUzOTA1ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO1VOMDI0NS4xO1pTQ0FOMjA7MSw1MzkwNWUtMDIKRk9YQTI7Y29iaW5kZXJfMztVTjAyNDUuMTtaU0NBTjIwOzEsNTM5MDVlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3NjcxXzIuMDA7Wk5GOTM7MSw1NTIyM2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDc2NzFfMi4wMDtaTkY5MzsxLDU1MjIzZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzY3MV8yLjAwO1pORjkzOzEsNTUyMjNlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3NjcxXzIuMDA7Wk5GOTM7MSw1NTIyM2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg5MDNfMi4wMDtaTkYzOTQ7MSw1NjEwNWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg5MDNfMi4wMDtaTkYzOTQ7MSw1NjEwNWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDI0MzVfMi4wMDtMQ09SOzEsNTg1MDdlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAyNDM1XzIuMDA7TENPUjsxLDU4NTA3ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNTUxNF8yLjAwO0hTRlkyLEhTRlgxLEhTRlgyOzEsNTg2ODdlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA1NTE0XzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7MSw1ODY4N2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDU1MTRfMi4wMDtIU0ZZMixIU0ZYMSxIU0ZYMjsxLDU4Njg3ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNTUxNF8yLjAwO0hTRlkyLEhTRlgxLEhTRlgyOzEsNTg2ODdlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA3Njg5XzIuMDA7Wk5GMzgzOzEsNTk1ODdlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA3Njg5XzIuMDA7Wk5GMzgzOzEsNTk1ODdlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA3NzA1XzIuMDA7Wk5GNzk5OzEsNTk1ODdlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA3NzA1XzIuMDA7Wk5GNzk5OzEsNTk1ODdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0NjM3XzIuMDA7Wk5GNTgwOzEsNTk1ODdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NjY2XzIuMDA7Wk5GNjYyOzEsNTk1ODdlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wMjA1LjE7Wk5GNTgwOzEsNTk1ODdlLTAyCkZPWEEyO2NvYmluZGVyXzE7VU4wNTk5LjE7Wk5GMTk7MSw1OTk2NGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDAzNjFfMi4wMDtQT1U0RjM7MSw2MDA0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDAzNjFfMi4wMDtQT1U0RjM7MSw2MDA0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDAzNjFfMi4wMDtQT1U0RjM7MSw2MDA0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDAzNjFfMi4wMDtQT1U0RjM7MSw2MDA0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE2NjVfMi4wMDtBUklEM0IsQVJJRDNDOzEsNjAwNDllLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAxNjY1XzIuMDA7QVJJRDNCLEFSSUQzQzsxLDYwMDQ5ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTY2NV8yLjAwO0FSSUQzQixBUklEM0M7MSw2MDA0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU1MzZfMi4wMDtJUkY1OzEsNjA3MDBlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA5MzA2XzIuMDA7TlI0QTM7MSw2Mzg2MGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDkzMDZfMi4wMDtOUjRBMzsxLDYzODYwZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wOTMwNl8yLjAwO05SNEEzOzEsNjM4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA5MzA2XzIuMDA7TlI0QTM7MSw2Mzg2MGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDMzMDdfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDMzMDdfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDMzMDdfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDMzMDdfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDMzMDdfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDMzMDdfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDMzMDdfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU0NjlfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU0NjlfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU0NjlfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU0NjlfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU0NjlfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU0NjlfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU0NjlfMi4wMDtQT1UyRjM7MSw2Mzg4M2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtVTjAxMjMuMTtGT1hSMjsxLDY0MDQyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzcwNl8yLjAwO1pORjc4MjsxLDY0Njg0ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNzYwMl8yLjAwO1pORjE4OzEsNjQ5NjhlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NjAyXzIuMDA7Wk5GMTg7MSw2NDk2OGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc2MDJfMi4wMDtaTkYxODsxLDY0OTY4ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNzYwMl8yLjAwO1pORjE4OzEsNjQ5NjhlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NjAyXzIuMDA7Wk5GMTg7MSw2NDk2OGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc2MDJfMi4wMDtaTkYxODsxLDY0OTY4ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODM5NV8yLjAwO1pORjI2MDsxLDY0OTY4ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODM5NV8yLjAwO1pORjI2MDsxLDY0OTY4ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODM5NV8yLjAwO1pORjI2MDsxLDY0OTY4ZS0wMgpGT1hBMjtjb2JpbmRlcl82O01BMDY1OS4zO01BRkc7MSw2NDk2OGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE3MzAuMTtaTkY3MDg7MSw2NDk2OGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE3MzAuMTtaTkY3MDg7MSw2NDk2OGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE3MzAuMTtaTkY3MDg7MSw2NDk2OGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg5MzJfMi4wMDtaTkY0Njc7MSw2NTY5MmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg5MzJfMi4wMDtaTkY0Njc7MSw2NTY5MmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtVTjA1OTguMTtaTkYxODQ7MSw2NzQzMmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDAyMThfMi4wMDtaTkYyMDA7MSw2ODAyMGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQwMjZfMi4wMDtCQVRGMzsxLDY4MjA3ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDAyNl8yLjAwO0JBVEYzOzEsNjgyMDdlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MDI2XzIuMDA7QkFURjM7MSw2ODIwN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTE3MjYuMTtaTkYzMzE7MSw2OTE2NWUtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTE3MjYuMTtaTkYzMzE7MSw2OTE2NWUtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTE3MjYuMTtaTkYzMzE7MSw2OTE2NWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtVTjA2MzkuMTtaTkY1ODc7MSw3MTYxNmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MSw3MTg1MWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MSw3MTg1MWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MSw3MTg1MWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MSw3MTg1MWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MSw3MTg1MWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MSw3MTg1MWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MSw3MTg1MWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MSw3MTg1MWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDgzMTNfMi4wMDtaTkY0MTsxLDcyMTM0ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMzMwMF8yLjAwO1BPVTFGMTsxLDcyMjEwZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMzMwMF8yLjAwO1BPVTFGMTsxLDcyMjEwZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMzMwMF8yLjAwO1BPVTFGMTsxLDcyMjEwZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMzMwMF8yLjAwO1BPVTFGMTsxLDcyMjEwZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMzMwMF8yLjAwO1BPVTFGMTsxLDcyMjEwZS0wMgpGT1hBMjtjb2JpbmRlcl80O1VOMDI0NS4xO1pTQ0FOMjA7MSw3Mjg5MGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtVTjAyNDUuMTtaU0NBTjIwOzEsNzI4OTBlLTAyCkZPWEEyO2NvYmluZGVyXzQ7VU4wMjQ1LjE7WlNDQU4yMDsxLDcyODkwZS0wMgpGT1hBMjtjb2JpbmRlcl80O1VOMDI0NS4xO1pTQ0FOMjA7MSw3Mjg5MGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MjZfMi4wMDtMSU41NDsxLDczMjIyZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMjUyNl8yLjAwO0xJTjU0OzEsNzMyMjJlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAyNTI2XzIuMDA7TElONTQ7MSw3MzIyMmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDI1MjZfMi4wMDtMSU41NDsxLDczMjIyZS0wMgpGT1hBMjtjb2JpbmRlcl80O1VOMDIyMi4xO1pORjc2NTsxLDczMjY1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMjUzOF8yLjAwO1RIQVAxMjsxLDc0MzgyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMjUzOF8yLjAwO1RIQVAxMjsxLDc0MzgyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMjUzOF8yLjAwO1RIQVAxMjsxLDc0MzgyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMjUzOF8yLjAwO1RIQVAxMjsxLDc0MzgyZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODM4M18yLjAwO1pORjcxOzEsNzUxOTllLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4Mjc0XzIuMDA7Wk5GNTgyOzEsNzYxMDJlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA4MzE0XzIuMDA7Wk5GMjE0OzEsNzY4NjVlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA4MzE0XzIuMDA7Wk5GMjE0OzEsNzY4NjVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA5MzA1XzIuMDA7TlI0QTM7MSw3NzAxMGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDkzMDVfMi4wMDtOUjRBMzsxLDc3MDEwZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wOTMwNV8yLjAwO05SNEEzOzEsNzcwMTBlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA5MzA1XzIuMDA7TlI0QTM7MSw3NzAxMGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDUzNTZfMi4wMDtQT1U2RjE7MSw4MDk3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDUzNTZfMi4wMDtQT1U2RjE7MSw4MDk3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDUzNTZfMi4wMDtQT1U2RjE7MSw4MDk3OWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDg5NDNfMi4wMDtaTkY1NjM7MSw4MjM1OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDkzNzVfMi4wMDtBSVJFOzEsODMxNjFlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA5Mzc1XzIuMDA7QUlSRTsxLDgzMTYxZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wOTM3NV8yLjAwO0FJUkU7MSw4MzE2MWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDkzNzVfMi4wMDtBSVJFOzEsODMxNjFlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA5Mzc1XzIuMDA7QUlSRTsxLDgzMTYxZS0wMgpGT1hBMjtjb2JpbmRlcl83O01BMTkzNy4xO0VSRjo6SE9YQjEzOzEsODM4MTZlLTAyCkZPWEEyO2NvYmluZGVyXzc7VU4wMjMyLjE7Wk5GNzkzOzEsODM4MTZlLTAyCkZPWEEyO2NvYmluZGVyXzc7VU4wMjUzLjE7TFlMMTsxLDgzODE2ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wNzY4NF8yLjAwO1pORjE5NzsxLDg0NDAxZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wNzY4NF8yLjAwO1pORjE5NzsxLDg0NDAxZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wNzY4NF8yLjAwO1pORjE5NzsxLDg0NDAxZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wNzY4NF8yLjAwO1pORjE5NzsxLDg0NDAxZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wNzY4NF8yLjAwO1pORjE5NzsxLDg0NDAxZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wNzY4NF8yLjAwO1pORjE5NzsxLDg0NDAxZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wNzY4NF8yLjAwO1pORjE5NzsxLDg0NDAxZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wODI0NV8yLjAwO1pORjQxOzEsODQ0MDFlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA0NDEyXzIuMDA7Wk5GODIxOzEsODUyMzZlLTAyCkZPWEEyO2NvYmluZGVyXzU7VU4wMzI1LjE7Wk5GNDU7MSw4NTU4OGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtVTjAzMjUuMTtaTkY0NTsxLDg1NTg4ZS0wMgpGT1hBMjtjb2JpbmRlcl83O01BMTk0MC4xO0VUVjI6OkRSR1g7MSw4NjI0NGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDc1NjVfMi4wMDtaTkY1MDY7MSw4NjQ2OGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDc2OTdfMi4wMDtaTkY3OTsxLDg2NDY4ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wNzc1M18yLjAwO1pORjgwNTsxLDg2NDY4ZS0wMgpGT1hBMjtjb2JpbmRlcl80O1VOMDY3MS4xO0RVWEJMMTsxLDg2NDY4ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTMxOV8yLjAwO0xJTjU0OzEsODY3NTVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAxMzE5XzIuMDA7TElONTQ7MSw4Njc1NWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDEzMTlfMi4wMDtMSU41NDsxLDg2NzU1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTMxOV8yLjAwO0xJTjU0OzEsODY3NTVlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAwODMyXzIuMDA7VEJYMTA7MSw4NzQxMmUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDA4MzJfMi4wMDtUQlgxMDsxLDg3NDEyZS0wMgpGT1hBMjtjb2JpbmRlcl8xO1VOMDY1Mi4xO1pORjcxNjsxLDg3NjU0ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMDM3MF8yLjAwO05SMkUzOzEsODgzNTJlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAwMzcwXzIuMDA7TlIyRTM7MSw4ODM1MmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDAzNzBfMi4wMDtOUjJFMzsxLDg4MzUyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMDM3MF8yLjAwO05SMkUzOzEsODgzNTJlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAwMzcwXzIuMDA7TlIyRTM7MSw4ODM1MmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNQTE2NTQuMTtaTkYxNjsxLDg4OTM1ZS0wMgpGT1hBMjtjb2JpbmRlcl83O01BMTY1NC4xO1pORjE2OzEsODg5MzVlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAyODQ0XzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzEsODkwMzNlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAyODQ0XzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzEsODkwMzNlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAyODQ0XzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzEsODkwMzNlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MDE4XzIuMDA7QVRGNjsxLDg5MDMzZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDAxOF8yLjAwO0FURjY7MSw4OTAzM2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQxODZfMi4wMDtNU0M7MSw4OTAzM2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQxODZfMi4wMDtNU0M7MSw4OTAzM2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQxODZfMi4wMDtNU0M7MSw4OTAzM2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQxODZfMi4wMDtNU0M7MSw4OTAzM2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDA3OTBfMi4wMDtGT1hJMixGT1hJMzsxLDg5MzkxZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMDc5MF8yLjAwO0ZPWEkyLEZPWEkzOzEsODkzOTFlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAxOTg3XzIuMDA7Rk9YSTIsRk9YSTM7MSw4OTM5MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDE5ODdfMi4wMDtGT1hJMixGT1hJMzsxLDg5MzkxZS0wMgpGT1hBMjtjb2JpbmRlcl8wO1VOMDYzMy4xO1pORjU2NzsxLDg5ODI1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzc2NV8yLjAwO1pORjQ5MjsxLDkxNTA0ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO01BMDE0MC4yO0dBVEExOjpUQUwxOzEsOTE1MDRlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4MzQ2XzIuMDA7Wk5GNDU0OzEsOTMyNDhlLTAyCkZPWEEyO2NvYmluZGVyXzE7TUExOTc2LjE7Wk5GMzIwOzEsOTMyNDhlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NjA4XzIuMDA7Wk5GMzgyOzEsOTU2MjllLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4MzgyXzIuMDA7Wk5GNjc3OzEsOTU2MjllLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAwMzYzXzIuMDA7UE9VNkYyOzEsOTU5MzBlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAwMzYzXzIuMDA7UE9VNkYyOzEsOTU5MzBlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAwMzYzXzIuMDA7UE9VNkYyOzEsOTU5MzBlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAxNjY2XzIuMDA7QVJJRDNCLEFSSUQzQzsxLDk2OTg4ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTY2Nl8yLjAwO0FSSUQzQixBUklEM0M7MSw5Njk4OGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE2NjZfMi4wMDtBUklEM0IsQVJJRDNDOzEsOTY5ODhlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0NTI3XzIuMDA7Wk5GMjM7MSw5NzgzOGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQ1MjdfMi4wMDtaTkYyMzsxLDk3ODM4ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDUyN18yLjAwO1pORjIzOzEsOTc4MzhlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0NTI3XzIuMDA7Wk5GMjM7MSw5NzgzOGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDg5NTNfMi4wMDtaTkY2Njc7MSw5NzgzOGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtVTjAxNjcuMTtaTkYyMzsxLDk3ODM4ZS0wMgpGT1hBMjtjb2JpbmRlcl81O1VOMDE2Ny4xO1pORjIzOzEsOTc4MzhlLTAyCkZPWEEyO2NvYmluZGVyXzU7VU4wMTY3LjE7Wk5GMjM7MSw5NzgzOGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtVTjAxNjcuMTtaTkYyMzsxLDk3ODM4ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wMTQ5N18yLjAwO01BWDsxLDk4NDE4ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wOTMxN18yLjAwO05SNEEzOzEsOTg0MThlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA5MzE3XzIuMDA7TlI0QTM7MSw5ODQxOGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDkzMTdfMi4wMDtOUjRBMzsxLDk4NDE4ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wOTMxN18yLjAwO05SNEEzOzEsOTg0MThlLTAyCkZPWEEyO2NvYmluZGVyXzM7VU4wNjAzLjE7Wk5GMjIzOzEsOTk2MTNlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjAzXzIuMDA7Q0VOUEJEMTsxLDk5ODM3ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNDQ3M18yLjAwO1pORjc4NzsyLDAwODc4ZS0wMgpGT1hBMjtjb2JpbmRlcl83O1VOMDIzMC4xO1pORjc4NzsyLDAwODc4ZS0wMgpGT1hBMjtjb2JpbmRlcl83O01BMDYxNS4xO0dNRUIxOzIsMDE2MzBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TUEwNjE1LjE7R01FQjE7MiwwMTYzMGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNQTA2MjkuMTtSSE9YMTE7MiwwMTYzMGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNQTA4ODMuMTtETUJYMTsyLDAxNjMwZS0wMgpGT1hBMjtjb2JpbmRlcl83O01BMDg4My4xO0RNQlgxOzIsMDE2MzBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TUEwODgzLjE7RE1CWDE7MiwwMTYzMGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDgzNDRfMi4wMDtaTkY0NDk7MiwwMjY0NmUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDgyNzRfMi4wMDtaTkY1ODI7MiwwMzEyNGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDc1ODBfMi4wMDtaTkYxMzM7MiwwMzMyMmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDc1ODBfMi4wMDtaTkYxMzM7MiwwMzMyMmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDc1ODBfMi4wMDtaTkYxMzM7MiwwMzMyMmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDc3MDZfMi4wMDtaTkY3ODI7MiwwMzMyMmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDAzNjFfMi4wMDtQT1U0RjM7MiwwNDI0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDAzNjFfMi4wMDtQT1U0RjM7MiwwNDI0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDAzNjFfMi4wMDtQT1U0RjM7MiwwNDI0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDAzNjFfMi4wMDtQT1U0RjM7MiwwNDI0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE2NjFfMi4wMDtBUklENUE7MiwwNDI0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE2NjFfMi4wMDtBUklENUE7MiwwNDI0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE2NjFfMi4wMDtBUklENUE7MiwwNDI0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE2NjVfMi4wMDtBUklEM0IsQVJJRDNDOzIsMDQyNDllLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxNjY1XzIuMDA7QVJJRDNCLEFSSUQzQzsyLDA0MjQ5ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMTY2NV8yLjAwO0FSSUQzQixBUklEM0M7MiwwNDI0OWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDgzOTBfMi4wMDtaU0NBTjVDOzIsMDYwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4MzkwXzIuMDA7WlNDQU41QzsyLDA2MDQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO1VOMDIzNy4xO1pORjgyMTsyLDA2MDQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNTYzN18yLjAwO05SM0MyOzIsMDcwMzdlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA1NjM3XzIuMDA7TlIzQzI7MiwwNzAzN2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU2MzdfMi4wMDtOUjNDMjsyLDA3MDM3ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNTYzN18yLjAwO05SM0MyOzIsMDcwMzdlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3NjAyXzIuMDA7Wk5GMTg7MiwwODU1MGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDc2MDJfMi4wMDtaTkYxODsyLDA4NTUwZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzYwMl8yLjAwO1pORjE4OzIsMDg1NTBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3NjAyXzIuMDA7Wk5GMTg7MiwwODU1MGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDc2MDJfMi4wMDtaTkYxODsyLDA4NTUwZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzYwMl8yLjAwO1pORjE4OzIsMDg1NTBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0NTM3XzIuMDA7S0xGMTM7MiwwOTgxNGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQ1MzdfMi4wMDtLTEYxMzsyLDA5ODE0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDUzN18yLjAwO0tMRjEzOzIsMDk4MTRlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0NTM3XzIuMDA7S0xGMTM7MiwwOTgxNGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQ1MzdfMi4wMDtLTEYxMzsyLDA5ODE0ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNDM3MF8yLjAwO01BRkc7MiwxMDU1MmUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDMzMjhfMi4wMDtIU0ZZMixIU0ZYMSxIU0ZYMjsyLDEwODU2ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wMzMyOF8yLjAwO0hTRlkyLEhTRlgxLEhTRlgyOzIsMTA4NTZlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAzMzI4XzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7MiwxMDg1NmUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDMzMjhfMi4wMDtIU0ZZMixIU0ZYMSxIU0ZYMjsyLDEwODU2ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wODI0N18yLjAwO1pORjM4MjsyLDEwODU2ZS0wMgpGT1hBMjtjb2JpbmRlcl80O1VOMDUzNS4xO0ZPWE8xOjpFTEYxOzIsMTA4NTZlLTAyCkZPWEEyO2NvYmluZGVyXzQ7VU4wNjY0LjE7Wk5GODYwOzIsMTA4NTZlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAzNDQ5XzIuMDA7TkZBVEMxOzIsMTI4MTllLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAzNDQ5XzIuMDA7TkZBVEMxOzIsMTI4MTllLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAzNDQ5XzIuMDA7TkZBVEMxOzIsMTI4MTllLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAzNDQ5XzIuMDA7TkZBVEMxOzIsMTI4MTllLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3NzM2XzIuMDA7Wk5GODQ7MiwxNDkwMWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDEwODdfMi4wMDtMSU41NDsyLDE1ODQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTA4N18yLjAwO0xJTjU0OzIsMTU4NDZlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAxMDg3XzIuMDA7TElONTQ7MiwxNTg0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDEwODdfMi4wMDtMSU41NDsyLDE1ODQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTIwNl8yLjAwO1RJR0QyLEpSS0w7MiwxNTg0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDEyMDZfMi4wMDtUSUdEMixKUktMOzIsMTU4NDZlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4MzM3XzIuMDA7Wk5GNDE1OzIsMTYxMTVlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4MzM3XzIuMDA7Wk5GNDE1OzIsMTYxMTVlLTAyCkZPWEEyO2NvYmluZGVyXzY7TUExOTc1LjE7Wk5GMjE0OzIsMTYxMTVlLTAyCkZPWEEyO2NvYmluZGVyXzY7TUExOTc1LjE7Wk5GMjE0OzIsMTYxMTVlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wNjY0LjE7Wk5GODYwOzIsMTYxMTVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAwNTI4XzIuMDA7VFBSWDE7MiwxNjk2OGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE2NjFfMi4wMDtBUklENUE7MiwxNjk2OGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE2NjFfMi4wMDtBUklENUE7MiwxNjk2OGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDE2NjFfMi4wMDtBUklENUE7MiwxNjk2OGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDEwODdfMi4wMDtMSU41NDsyLDE4MTQ4ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wMTA4N18yLjAwO0xJTjU0OzIsMTgxNDhlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAxMDg3XzIuMDA7TElONTQ7MiwxODE0OGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDEwODdfMi4wMDtMSU41NDsyLDE4MTQ4ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODg1OF8yLjAwO1pORjMyNDsyLDE5NTgzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODg1OF8yLjAwO1pORjMyNDsyLDE5NTgzZS0wMgpGT1hBMjtjb2JpbmRlcl8xO01BMDE0MC4yO0dBVEExOjpUQUwxOzIsMjA1MDllLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4OTE2XzIuMDA7Wk5GMjc0OzIsMjEyODhlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4OTE2XzIuMDA7Wk5GMjc0OzIsMjEyODhlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4OTE2XzIuMDA7Wk5GMjc0OzIsMjEyODhlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4OTE2XzIuMDA7Wk5GMjc0OzIsMjEyODhlLTAyCkZPWEEyO2NvYmluZGVyXzE7VU4wMTUyLjE7WkZQMjg7MiwyMTI4OGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDkzMzZfMi4wMDtUUDczOzIsMjE1NzFlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA5MzM2XzIuMDA7VFA3MzsyLDIxNTcxZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNzU4MF8yLjAwO1pORjEzMzsyLDIyNzcxZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNzU4MF8yLjAwO1pORjEzMzsyLDIyNzcxZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNzU4MF8yLjAwO1pORjEzMzsyLDIyNzcxZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODM3OV8yLjAwO1pORjI1NzsyLDI0ODQwZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODM3OV8yLjAwO1pORjI1NzsyLDI0ODQwZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzcwNF8yLjAwO1pORjYwNTsyLDI0ODYyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzcxMF8yLjAwO1pORjMzQjsyLDI0ODYyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzcxMF8yLjAwO1pORjMzQjsyLDI0ODYyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzcxMF8yLjAwO1pORjMzQjsyLDI0ODYyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODM4Ml8yLjAwO1pORjY3NzsyLDI0ODYyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODYwOV8yLjAwO1RCUEwyOzIsMjQ4NjJlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4NjA5XzIuMDA7VEJQTDI7MiwyNDg2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDEzMjFfMi4wMDtMSU41NDsyLDI1MTIxZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTMyMV8yLjAwO0xJTjU0OzIsMjUxMjFlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAxMzIxXzIuMDA7TElONTQ7MiwyNTEyMWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDEzMjFfMi4wMDtMSU41NDsyLDI1MTIxZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODM4M18yLjAwO1pORjcxOzIsMjU3MzllLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4ODYwXzIuMDA7Wk5GMjY0OzIsMjU3MzllLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA4OTI5XzIuMDA7Wk5GODE2OzIsMjU5NjhlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAyNDM1XzIuMDA7TENPUjsyLDI2MTAyZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wMjQzNV8yLjAwO0xDT1I7MiwyNjEwMmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDEyNDZfMi4wMDtIRFg7MiwyNjI2N2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDEyNDZfMi4wMDtIRFg7MiwyNjI2N2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU1NDBfMi4wMDtJUkY0OzIsMjgxODhlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA1NTQwXzIuMDA7SVJGNDsyLDI4MTg4ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNTU0MF8yLjAwO0lSRjQ7MiwyODE4OGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU1NDBfMi4wMDtJUkY0OzIsMjgxODhlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4OTUzXzIuMDA7Wk5GNjY3OzIsMjg4NTVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA3NjY0XzIuMDA7Wk5GNzE2OzIsMjg4OTRlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4MjU0XzIuMDA7Wk5GNjIxOzIsMjg4OTRlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3NzI5XzIuMDA7Wk5GNzgwQTsyLDI5MDAyZS0wMgpGT1hBMjtjb2JpbmRlcl80O1VOMDYyNS4xO1pORjUyNzsyLDI5Nzg0ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO01BMTczMS4xO1pORjc2ODsyLDI5OTY3ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODk0OV8yLjAwO1pGUDI4OzIsMjk5NzhlLTAyCkZPWEEyO2NvYmluZGVyXzU7TUEwNDczLjM7RUxGMTsyLDMwNTUyZS0wMgpGT1hBMjtjb2JpbmRlcl81O01BMDQ3My4zO0VMRjE7MiwzMDU1MmUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQxMzBfMi4wMDtDTE9DSzsyLDMxMTAzZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDEzMF8yLjAwO0NMT0NLOzIsMzExMDNlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MjAwXzIuMDA7QkhMSEUyMjsyLDMxMTAzZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDIwMF8yLjAwO0JITEhFMjI7MiwzMTEwM2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQyMDBfMi4wMDtCSExIRTIyOzIsMzExMDNlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MjAwXzIuMDA7QkhMSEUyMjsyLDMxMTAzZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDIwMF8yLjAwO0JITEhFMjI7MiwzMTEwM2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg4OTZfMi4wMDtaTkY0MTsyLDMxNTM4ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzcwNV8yLjAwO1pORjc5OTsyLDMyNTM5ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzcwNV8yLjAwO1pORjc5OTsyLDMyNTM5ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODkwNF8yLjAwO1pORjM4MjsyLDM0NDk0ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzYxMV8yLjAwO1pORjEyOzIsMzU3MTVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA3NjExXzIuMDA7Wk5GMTI7MiwzNTcxNWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDc2MTFfMi4wMDtaTkYxMjsyLDM1NzE1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzYxMV8yLjAwO1pORjEyOzIsMzU3MTVlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0MzY3XzIuMDA7TUFGRzsyLDM2OTEwZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wODg5OF8yLjAwO1pORjIxNDsyLDM5MTAwZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wODg5OF8yLjAwO1pORjIxNDsyLDM5MTAwZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMDUyN18yLjAwO1RQUlgxOzIsMzk1NTllLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAwNTI4XzIuMDA7VFBSWDE7MiwzOTU1OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNQTE3MzEuMTtaTkY3Njg7Miw0MTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg5MTdfMi4wMDtaTkY1NTQ7Miw0MjA0M2UtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDc3MDVfMi4wMDtaTkY3OTk7Miw0MjQ5N2UtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDc3MDVfMi4wMDtaTkY3OTk7Miw0MjQ5N2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg4MDdfMi4wMDtNQUY7Miw0MjU0NGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg4MDdfMi4wMDtNQUY7Miw0MjU0NGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg4MDdfMi4wMDtNQUY7Miw0MjU0NGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg4MDdfMi4wMDtNQUY7Miw0MjU0NGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDEwMDhfMi4wMDtGT1hSMTsyLDQ0NTQwZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wMTAwOF8yLjAwO0ZPWFIxOzIsNDQ1NDBlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4ODcyXzIuMDA7Wk5GODU7Miw0NDc2MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg4NzJfMi4wMDtaTkY4NTsyLDQ0NzYxZS0wMgpGT1hBMjtjb2JpbmRlcl82O1VOMDU4NC4xO1RFQUQ0OjpFVFY3OzIsNDQ3NjFlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA0NjM5XzIuMDA7Wk5GNTgwOzIsNDUxMDllLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA1NTM2XzIuMDA7SVJGNTsyLDQ1ODQ4ZS0wMgpGT1hBMjtjb2JpbmRlcl80O01BMDg4My4xO0RNQlgxOzIsNDg2NzVlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUEwODgzLjE7RE1CWDE7Miw0ODY3NWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNQTA4ODMuMTtETUJYMTsyLDQ4Njc1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMDUyN18yLjAwO1RQUlgxOzIsNTEwMjRlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA4MTI5XzIuMDA7R1JITDI7Miw1MTI0NmUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDgxMjlfMi4wMDtHUkhMMjsyLDUxMjQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODEyOV8yLjAwO0dSSEwyOzIsNTEyNDZlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA4MTI5XzIuMDA7R1JITDI7Miw1MTI0NmUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDgxMjlfMi4wMDtHUkhMMjsyLDUxMjQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl82O01BMDE0NS4yO1RGQ1AyTDE7Miw1MTQ5N2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTAxNDUuMjtURkNQMkwxOzIsNTE0OTdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TUEwMTQ1LjI7VEZDUDJMMTsyLDUxNDk3ZS0wMgpGT1hBMjtjb2JpbmRlcl82O1VOMDMxMy4xO1pGUDkxOzIsNTE0OTdlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wMzEzLjE7WkZQOTE7Miw1MTQ5N2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtVTjAzMTMuMTtaRlA5MTsyLDUxNDk3ZS0wMgpGT1hBMjtjb2JpbmRlcl82O1VOMDMxMy4xO1pGUDkxOzIsNTE0OTdlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wMzEzLjE7WkZQOTE7Miw1MTQ5N2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtVTjAzMTMuMTtaRlA5MTsyLDUxNDk3ZS0wMgpGT1hBMjtjb2JpbmRlcl82O1VOMDMxMy4xO1pGUDkxOzIsNTE0OTdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4ODg4XzIuMDA7Wk5GMzg0OzIsNTE2ODdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4ODg4XzIuMDA7Wk5GMzg0OzIsNTE2ODdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4ODg4XzIuMDA7Wk5GMzg0OzIsNTE2ODdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4ODg4XzIuMDA7Wk5GMzg0OzIsNTE2ODdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4ODg4XzIuMDA7Wk5GMzg0OzIsNTE2ODdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4ODg4XzIuMDA7Wk5GMzg0OzIsNTE2ODdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4ODg4XzIuMDA7Wk5GMzg0OzIsNTE2ODdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAwMzYwXzIuMDA7UE9VNEYzOzIsNTIyNDBlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAwMzYwXzIuMDA7UE9VNEYzOzIsNTIyNDBlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAwMzYwXzIuMDA7UE9VNEYzOzIsNTIyNDBlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAwMzYwXzIuMDA7UE9VNEYzOzIsNTIyNDBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA1NTEyXzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7Miw1MzAxMGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDU1MTJfMi4wMDtIU0ZZMixIU0ZYMSxIU0ZYMjsyLDUzMDEwZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNTUxMl8yLjAwO0hTRlkyLEhTRlgxLEhTRlgyOzIsNTMwMTBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA1NTEyXzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7Miw1MzAxMGUtMDIKRk9YQTI7Y29iaW5kZXJfNztVTjAxMjkuMTtIU0ZZMjsyLDUzMDEwZS0wMgpGT1hBMjtjb2JpbmRlcl83O1VOMDEyOS4xO0hTRlkyOzIsNTMwMTBlLTAyCkZPWEEyO2NvYmluZGVyXzM7TUExNTgxLjE7WkJUQjY7Miw1MzA5OGUtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTE1ODEuMTtaQlRCNjsyLDUzMDk4ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNTYzN18yLjAwO05SM0MyOzIsNTM5NDhlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA1NjM3XzIuMDA7TlIzQzI7Miw1Mzk0OGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDU2MzdfMi4wMDtOUjNDMjsyLDUzOTQ4ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNTYzN18yLjAwO05SM0MyOzIsNTM5NDhlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4OTMwXzIuMDA7WkZQODI7Miw1Njg1MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTA4ODMuMTtETUJYMTsyLDU3NjYxZS0wMgpGT1hBMjtjb2JpbmRlcl82O01BMDg4My4xO0RNQlgxOzIsNTc2NjFlLTAyCkZPWEEyO2NvYmluZGVyXzY7TUEwODgzLjE7RE1CWDE7Miw1NzY2MWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDgyNTRfMi4wMDtaTkY2MjE7Miw1OTE3MmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNQTE5OTIuMTtJS1pGMzsyLDU5MTcyZS0wMgpGT1hBMjtjb2JpbmRlcl83O01BMTk5Mi4xO0lLWkYzOzIsNTkxNzJlLTAyCkZPWEEyO2NvYmluZGVyXzc7TUExOTkyLjE7SUtaRjM7Miw1OTE3MmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNQTE5OTIuMTtJS1pGMzsyLDU5MTcyZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNzYwMV8yLjAwO1pORjc3NjsyLDYwNjQyZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODM0NF8yLjAwO1pORjQ0OTsyLDYwNjQyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODc5OV8yLjAwO0JBVEY7Miw2MDk4OGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDg3OTlfMi4wMDtCQVRGOzIsNjA5ODhlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4Nzk5XzIuMDA7QkFURjsyLDYwOTg4ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODc5OV8yLjAwO0JBVEY7Miw2MDk4OGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDA0MDVfMi4wMDtTRUJPWDsyLDYxMzAyZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wMDQwNV8yLjAwO1NFQk9YOzIsNjEzMDJlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAwNDA1XzIuMDA7U0VCT1g7Miw2MTMwMmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDgzNDFfMi4wMDtaTkY1NTQ7Miw2MjQ3M2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDMwODhfMi4wMDtWU1gxOzIsNjM2NzhlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAzMDg4XzIuMDA7VlNYMTsyLDYzNjc4ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wMzA4OF8yLjAwO1ZTWDE7Miw2MzY3OGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDMwODhfMi4wMDtWU1gxOzIsNjM2NzhlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAzMDg4XzIuMDA7VlNYMTsyLDYzNjc4ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wMzA4OF8yLjAwO1ZTWDE7Miw2MzY3OGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDMwODhfMi4wMDtWU1gxOzIsNjM2NzhlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA1Njc1XzIuMDA7RVNSUkc7Miw2MzY3OGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDU2NzVfMi4wMDtFU1JSRzsyLDYzNjc4ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNTY3NV8yLjAwO0VTUlJHOzIsNjM2NzhlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA1Njc1XzIuMDA7RVNSUkc7Miw2MzY3OGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDU2NzVfMi4wMDtFU1JSRzsyLDYzNjc4ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wOTAzMF8yLjAwO0UyRjE7Miw2NjE2MWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDkwMzBfMi4wMDtFMkYxOzIsNjYxNjFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA5MDMwXzIuMDA7RTJGMTsyLDY2MTYxZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wOTAzMF8yLjAwO0UyRjE7Miw2NjE2MWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDgzNTNfMi4wMDtaTkY4MTY7Miw2NzUzMGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDgzNDZfMi4wMDtaTkY0NTQ7Miw2ODkyOGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg5MjlfMi4wMDtaTkY4MTY7Miw3MjU2N2UtMDIKRk9YQTI7Y29iaW5kZXJfNztVTjA1OTguMTtaTkYxODQ7Miw3MjU2N2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDAyNzdfMi4wMDtQQlg0OzIsNzQ0NTBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3Njk3XzIuMDA7Wk5GNzk7Miw3NTE2NGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDgzMzZfMi4wMDtaTkYxNjsyLDc1MTY0ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wODMzNl8yLjAwO1pORjE2OzIsNzUxNjRlLTAyCkZPWEEyO2NvYmluZGVyXzc7VU4wNjgxLjE7WkZQNjgzOzIsNzUxNjRlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA3NzA0XzIuMDA7Wk5GNjA1OzIsNzUzMjJlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA3NzM2XzIuMDA7Wk5GODQ7Miw3NTMyMmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtVTjA1OTEuMTtaSUsxOzIsNzU2OTJlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3NjY0XzIuMDA7Wk5GNzE2OzIsNzYzNTRlLTAyCkZPWEEyO2NvYmluZGVyXzE7TUExNzA5LjE7WklNMzsyLDc2MzU0ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO01BMTcwOS4xO1pJTTM7Miw3NjM1NGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDgzODRfMi4wMDtaTkYxMjE7Miw3NzE4NGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDgzODRfMi4wMDtaTkYxMjE7Miw3NzE4NGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDgzODRfMi4wMDtaTkYxMjE7Miw3NzE4NGUtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTE5NTQuMTtGT1hPMTo6RUxLMTsyLDc4MDUzZS0wMgpGT1hBMjtjb2JpbmRlcl8zO1VOMDY0OC4xO1pORjY3NDsyLDc4MDUzZS0wMgpGT1hBMjtjb2JpbmRlcl8zO1VOMDY0OC4xO1pORjY3NDsyLDc4MDUzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNDM0Nl8yLjAwO01BRjsyLDc4MDgxZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNDM0Nl8yLjAwO01BRjsyLDc4MDgxZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNDM0Nl8yLjAwO01BRjsyLDc4MDgxZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNDM0Nl8yLjAwO01BRjsyLDc4MDgxZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wOTQ4OF8yLjAwO0JBQ0gxOzIsNzgwODFlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA5NDg4XzIuMDA7QkFDSDE7Miw3ODA4MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE1MjAuMTtNQUY7Miw3ODA4MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE1MjAuMTtNQUY7Miw3ODA4MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE1MjAuMTtNQUY7Miw3ODA4MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE1MjAuMTtNQUY7Miw3ODA4MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc1NjVfMi4wMDtaTkY1MDY7Miw3ODM2N2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDEzMTlfMi4wMDtMSU41NDsyLDc5NTY1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMTMxOV8yLjAwO0xJTjU0OzIsNzk1NjVlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMzE5XzIuMDA7TElONTQ7Miw3OTU2NWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDEzMTlfMi4wMDtMSU41NDsyLDc5NTY1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzY4NF8yLjAwO1pORjE5NzsyLDgxMzg2ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzY4NF8yLjAwO1pORjE5NzsyLDgxMzg2ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzY4NF8yLjAwO1pORjE5NzsyLDgxMzg2ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzY4NF8yLjAwO1pORjE5NzsyLDgxMzg2ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzY4NF8yLjAwO1pORjE5NzsyLDgxMzg2ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzY4NF8yLjAwO1pORjE5NzsyLDgxMzg2ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzY4NF8yLjAwO1pORjE5NzsyLDgxMzg2ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO01BMTEyNi4xO0ZPUzo6SlVOOzIsODMxNThlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wMjQ1LjE7WlNDQU4yMDsyLDg1Mjc1ZS0wMgpGT1hBMjtjb2JpbmRlcl82O1VOMDI0NS4xO1pTQ0FOMjA7Miw4NTI3NWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtVTjAyNDUuMTtaU0NBTjIwOzIsODUyNzVlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wMjQ1LjE7WlNDQU4yMDsyLDg1Mjc1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO1VOMDU5MS4xO1pJSzE7Miw4NjQ2NWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMTEwNTBfMi4wMDtNWUI7Miw4ODU5NGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMTEwNTBfMi4wMDtNWUI7Miw4ODU5NGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMTEwNTBfMi4wMDtNWUI7Miw4ODU5NGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMTEwNTBfMi4wMDtNWUI7Miw4ODU5NGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtVTjA2MTEuMTtaTkYzM0I7Miw4ODYyNGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtVTjA2MTEuMTtaTkYzM0I7Miw4ODYyNGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtVTjA2MTEuMTtaTkYzM0I7Miw4ODYyNGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg5NTNfMi4wMDtaTkY2Njc7Miw4OTkxN2UtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDA0MDVfMi4wMDtTRUJPWDsyLDkxNDg3ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMDQwNV8yLjAwO1NFQk9YOzIsOTE0ODdlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAwNDA1XzIuMDA7U0VCT1g7Miw5MTQ4N2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDU1NDdfMi4wMDtJUkY3OzIsOTIyNzBlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA1NTQ3XzIuMDA7SVJGNzsyLDkyMjcwZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wNTU0N18yLjAwO0lSRjc7Miw5MjI3MGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDU1NDdfMi4wMDtJUkY3OzIsOTIyNzBlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA1NTQ3XzIuMDA7SVJGNzsyLDkyMjcwZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wNTU0N18yLjAwO0lSRjc7Miw5MjI3MGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDU1NDdfMi4wMDtJUkY3OzIsOTIyNzBlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA5MjkwXzIuMDA7RVNSUkE7Miw5MjI3MGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDkyOTBfMi4wMDtFU1JSQTsyLDkyMjcwZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wOTI5MF8yLjAwO0VTUlJBOzIsOTIyNzBlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA5MjkwXzIuMDA7RVNSUkE7Miw5MjI3MGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDkyOTBfMi4wMDtFU1JSQTsyLDkyMjcwZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wMjA5OF8yLjAwO05BTk9HUDg7Miw5MjcyNmUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDIwOThfMi4wMDtOQU5PR1A4OzIsOTI3MjZlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA3NzIyXzIuMDA7Wk5GNjc1OzIsOTUyODRlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA3NzIyXzIuMDA7Wk5GNjc1OzIsOTUyODRlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MDMxXzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzIsOTYxNDZlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MDMxXzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzIsOTYxNDZlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MDMxXzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzIsOTYxNDZlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0Mzc3XzIuMDA7QVRGNkI7Miw5NjE0NmUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQzNzdfMi4wMDtBVEY2QjsyLDk2MTQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDM3N18yLjAwO0FURjZCOzIsOTYxNDZlLTAyCkZPWEEyO2NvYmluZGVyXzU7VU4wMTEyLjE7QVRGNkI7Miw5NjE0NmUtMDIKRk9YQTI7Y29iaW5kZXJfNTtVTjAxMTIuMTtBVEY2QjsyLDk2MTQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl81O1VOMDExMi4xO0FURjZCOzIsOTYxNDZlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAwMjE4XzIuMDA7Wk5GMjAwOzIsOTgzNzdlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3NzM3XzIuMDA7Wk5GNjY3OzIsOTg2MjFlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4Mjc0XzIuMDA7Wk5GNTgyOzIsOTg2MjFlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wNjU2LjE7Wk5GNzc0OzIsOTkwMzBlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMzIxXzIuMDA7TElONTQ7MywwMTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDEzMjFfMi4wMDtMSU41NDszLDAxNjM5ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMTMyMV8yLjAwO0xJTjU0OzMsMDE2MzllLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMzIxXzIuMDA7TElONTQ7MywwMTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE2NjZfMi4wMDtBUklEM0IsQVJJRDNDOzMsMDE2MzllLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxNjY2XzIuMDA7QVJJRDNCLEFSSUQzQzszLDAxNjM5ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMTY2Nl8yLjAwO0FSSUQzQixBUklEM0M7MywwMTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MywwMTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MywwMTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MywwMTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MywwMTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MywwMTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MywwMTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MywwMTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDE5MDNfMi4wMDtZQlgyLFlCWDM7MywwMTYzOWUtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDc5NTlfMi4wMDtGT1hBMixGT1hCMjszLDAyOTQ0ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wNzk1OV8yLjAwO0ZPWEEyLEZPWEIyOzMsMDI5NDRlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA3OTU5XzIuMDA7Rk9YQTIsRk9YQjI7MywwMjk0NGUtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDc5NTlfMi4wMDtGT1hBMixGT1hCMjszLDAyOTQ0ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNzczMV8yLjAwO1pORjQ0OzMsMDI5NjNlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NzMxXzIuMDA7Wk5GNDQ7MywwMjk2M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc3MzFfMi4wMDtaTkY0NDszLDAyOTYzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNzczMV8yLjAwO1pORjQ0OzMsMDI5NjNlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NzMxXzIuMDA7Wk5GNDQ7MywwMjk2M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc3MzFfMi4wMDtaTkY0NDszLDAyOTYzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNDM0N18yLjAwO01BRjszLDA0NTkzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNDM0N18yLjAwO01BRjszLDA0NTkzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNDM0N18yLjAwO01BRjszLDA0NTkzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNDM0N18yLjAwO01BRjszLDA0NTkzZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzU4MV8yLjAwO1pORjQ4NDszLDA0NjMyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO1VOMDU5OS4xO1pORjE5OzMsMDY0NzNlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA0NjE1XzIuMDA7Wk5GMTc3OzMsMDc4NDNlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA0NjE2XzIuMDA7Wk5GMTc3OzMsMDc4NDNlLTAyCkZPWEEyO2NvYmluZGVyXzc7VU4wMTY1LjE7Wk5GMTc3OzMsMDc4NDNlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4MzE0XzIuMDA7Wk5GMjE0OzMsMDgxMzBlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4MzE0XzIuMDA7Wk5GMjE0OzMsMDgxMzBlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4Mzg0XzIuMDA7Wk5GMTIxOzMsMDgxMzBlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4Mzg0XzIuMDA7Wk5GMTIxOzMsMDgxMzBlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4Mzg0XzIuMDA7Wk5GMTIxOzMsMDgxMzBlLTAyCkZPWEEyO2NvYmluZGVyXzM7TUExNjQ5LjE7WkJUQjEyOzMsMDk1NjdlLTAyCkZPWEEyO2NvYmluZGVyXzM7TUExNjQ5LjE7WkJUQjEyOzMsMDk1NjdlLTAyCkZPWEEyO2NvYmluZGVyXzM7TUExNjQ5LjE7WkJUQjEyOzMsMDk1NjdlLTAyCkZPWEEyO2NvYmluZGVyXzM7TUExNjQ5LjE7WkJUQjEyOzMsMDk1NjdlLTAyCkZPWEEyO2NvYmluZGVyXzM7TUExNjQ5LjE7WkJUQjEyOzMsMDk1NjdlLTAyCkZPWEEyO2NvYmluZGVyXzM7TUExNzA4LjE7RVRWNzszLDA5NTY3ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO01BMTcwOC4xO0VUVjc7MywwOTU2N2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTE3MDguMTtFVFY3OzMsMDk1NjdlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4MjYwXzIuMDA7Wk5GNDY3OzMsMTI0MDBlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4MjYwXzIuMDA7Wk5GNDY3OzMsMTI0MDBlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4MzQ0XzIuMDA7Wk5GNDQ5OzMsMTI0MDBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA4MzEyXzIuMDA7WklNMzszLDEzMDY1ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODMxMl8yLjAwO1pJTTM7MywxMzA2NWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtVTjAzNDAuMTtaTkY3NUE7MywxMzA2NWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDU1MTZfMi4wMDtIU0ZZMSxIU0ZYMSxIU0ZYMjszLDEzOTI5ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNTUxNl8yLjAwO0hTRlkxLEhTRlgxLEhTRlgyOzMsMTM5MjllLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA1NTE2XzIuMDA7SFNGWTEsSFNGWDEsSFNGWDI7MywxMzkyOWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDU1MTZfMi4wMDtIU0ZZMSxIU0ZYMSxIU0ZYMjszLDEzOTI5ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNTUxOF8yLjAwO0hTRlkxLEhTRlgxLEhTRlgyOzMsMTM5MjllLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA1NTE4XzIuMDA7SFNGWTEsSFNGWDEsSFNGWDI7MywxMzkyOWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDU1MThfMi4wMDtIU0ZZMSxIU0ZYMSxIU0ZYMjszLDEzOTI5ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNTUxOF8yLjAwO0hTRlkxLEhTRlgxLEhTRlgyOzMsMTM5MjllLTAyCkZPWEEyO2NvYmluZGVyXzc7VU4wMTI3LjE7SFNGWTE7MywxMzkyOWUtMDIKRk9YQTI7Y29iaW5kZXJfNztVTjAxMjcuMTtIU0ZZMTszLDEzOTI5ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wMjEyM18yLjAwO1RQUlgxOzMsMTQ3MDdlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3NjUwXzIuMDA7Wk5GMTE0OzMsMTQ5ODhlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAyODU3XzIuMDA7TUFGSzszLDE1MjQzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMjg1N18yLjAwO01BRks7MywxNTI0M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDQ2NjBfMi4wMDtNQk5MMjszLDE1MjQzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNDY2MF8yLjAwO01CTkwyOzMsMTUyNDNlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0NjYwXzIuMDA7TUJOTDI7MywxNTI0M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc1NjdfMi4wMDtaTkY2NzE7MywxNTI0M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDgzMTZfMi4wMDtaTkYxODszLDE1MjQzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODMxNl8yLjAwO1pORjE4OzMsMTUyNDNlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4MzE2XzIuMDA7Wk5GMTg7MywxNTI0M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDgzMTZfMi4wMDtaTkYxODszLDE1MjQzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODMxNl8yLjAwO1pORjE4OzMsMTUyNDNlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4MzE2XzIuMDA7Wk5GMTg7MywxNTI0M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg5MDFfMi4wMDtaTkYxODszLDE1MjQzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODkwMV8yLjAwO1pORjE4OzMsMTUyNDNlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4OTAxXzIuMDA7Wk5GMTg7MywxNTI0M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg5MDFfMi4wMDtaTkYxODszLDE1MjQzZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODkwMV8yLjAwO1pORjE4OzMsMTUyNDNlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4OTAxXzIuMDA7Wk5GMTg7MywxNTI0M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg5NTBfMi4wMDtaTkYyNTc7MywxNTI0M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg5NTBfMi4wMDtaTkYyNTc7MywxNTI0M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDk1OTZfMi4wMDtJUkYyOzMsMTUyNDNlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4ODA3XzIuMDA7TUFGOzMsMTU5NTVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4ODA3XzIuMDA7TUFGOzMsMTU5NTVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4ODA3XzIuMDA7TUFGOzMsMTU5NTVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4ODA3XzIuMDA7TUFGOzMsMTU5NTVlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3NzY1XzIuMDA7Wk5GNDkyOzMsMTYzNzZlLTAyCkZPWEEyO2NvYmluZGVyXzQ7VU4wMjMyLjE7Wk5GNzkzOzMsMTgzMTBlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4MzExXzIuMDA7Wk5GMTg5OzMsMTg3MDllLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA5Mjc1XzIuMDA7VEhSQTszLDE5MTA1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wOTI3NV8yLjAwO1RIUkE7MywxOTEwNWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDkyNzVfMi4wMDtUSFJBOzMsMTkxMDVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA5Mjc1XzIuMDA7VEhSQTszLDE5MTA1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wOTI3NV8yLjAwO1RIUkE7MywxOTEwNWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDkyNzVfMi4wMDtUSFJBOzMsMTkxMDVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA5Mjc1XzIuMDA7VEhSQTszLDE5MTA1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wOTI3NV8yLjAwO1RIUkE7MywxOTEwNWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDkyNzVfMi4wMDtUSFJBOzMsMTkxMDVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA5Mjc1XzIuMDA7VEhSQTszLDE5MTA1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wOTI3NV8yLjAwO1RIUkE7MywxOTEwNWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDkyMzRfMi4wMDtJUkYzOzMsMTkzMjJlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0NDczXzIuMDA7Wk5GNzg3OzMsMTk2NDhlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wMjMwLjE7Wk5GNzg3OzMsMTk2NDhlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA4ODk2XzIuMDA7Wk5GNDE7MywyMDQ2N2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDg5MzBfMi4wMDtaRlA4MjszLDIwNDY3ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO1VOMDU5OS4xO1pORjE5OzMsMjA0NjdlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUExNjIzLjE7U1RBVDI7MywyMzY3MWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNQTE2MjMuMTtTVEFUMjszLDIzNjcxZS0wMgpGT1hBMjtjb2JpbmRlcl80O01BMTYyMy4xO1NUQVQyOzMsMjM2NzFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUExNjIzLjE7U1RBVDI7MywyMzY3MWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNQTE2MjMuMTtTVEFUMjszLDIzNjcxZS0wMgpGT1hBMjtjb2JpbmRlcl80O1VOMDU5OC4xO1pORjE4NDszLDIzODc2ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wMDcxMV8yLjAwO0NJQzszLDI1NzI4ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO1VOMDIzMi4xO1pORjc5MzszLDI3NzcxZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDY1N18yLjAwO0tMRjE0OzMsMjg1MDRlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAyMjgxXzIuMDA7TkFJRjE7MywzMDMxNmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDIyODFfMi4wMDtOQUlGMTszLDMwMzE2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMDQyOF8yLjAwO1RQUlgxOzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAwNDQwXzIuMDA7VFBSWDE7MywzMzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDA2NzNfMi4wMDtUUFJYMTszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMjUyMF8yLjAwO0xJTjU0OzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAyNTIwXzIuMDA7TElONTQ7MywzMzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDI1MjBfMi4wMDtMSU41NDszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMjUyMF8yLjAwO0xJTjU0OzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzMDg3XzIuMDA7VlNYMTszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzA4N18yLjAwO1ZTWDE7MywzMzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMwODdfMi4wMDtWU1gxOzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzMDg3XzIuMDA7VlNYMTszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzA4N18yLjAwO1ZTWDE7MywzMzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMwODdfMi4wMDtWU1gxOzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzMDg3XzIuMDA7VlNYMTszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzI1MF8yLjAwO1RQUlgxOzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA0OTQzXzIuMDA7VlNYMTszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wNDk0M18yLjAwO1ZTWDE7MywzMzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDQ5NDNfMi4wMDtWU1gxOzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA0OTQzXzIuMDA7VlNYMTszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wNDk0M18yLjAwO1ZTWDE7MywzMzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDQ5NDNfMi4wMDtWU1gxOzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA0OTQzXzIuMDA7VlNYMTszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO01BMDYzMC4xO1NIT1g7MywzMzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNQTA2MzAuMTtTSE9YOzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TUEwNjMwLjE7U0hPWDszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO01BMDYzMC4xO1NIT1g7MywzMzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNQTA3MTcuMTtSQVgyOzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TUEwNzE3LjE7UkFYMjszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO01BMDcxNy4xO1JBWDI7MywzMzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNQTA3MTcuMTtSQVgyOzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TUEwNzI1LjE7VlNYMTszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO01BMDcyNS4xO1ZTWDE7MywzMzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNQTA3MjUuMTtWU1gxOzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TUEwNzI1LjE7VlNYMTszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl8yO01BMDcyNS4xO1ZTWDE7MywzMzUzMWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNQTA3MjUuMTtWU1gxOzMsMzM1MzFlLTAyCkZPWEEyO2NvYmluZGVyXzI7TUEwNzI1LjE7VlNYMTszLDMzNTMxZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wODEwOF8yLjAwO1RGRFAxLFRGRFAyLFRGRFAzOzMsMzQ0MTVlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA4MTA4XzIuMDA7VEZEUDEsVEZEUDIsVEZEUDM7MywzNDQxNWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDgxMDhfMi4wMDtURkRQMSxURkRQMixURkRQMzszLDM0NDE1ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wODEwOF8yLjAwO1RGRFAxLFRGRFAyLFRGRFAzOzMsMzQ0MTVlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA4MTA4XzIuMDA7VEZEUDEsVEZEUDIsVEZEUDM7MywzNDQxNWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDgxMDhfMi4wMDtURkRQMSxURkRQMixURkRQMzszLDM0NDE1ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wODEwOF8yLjAwO1RGRFAxLFRGRFAyLFRGRFAzOzMsMzQ0MTVlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA4MTA4XzIuMDA7VEZEUDEsVEZEUDIsVEZEUDM7MywzNDQxNWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNQTExMjIuMTtURkRQMTszLDM0NDE1ZS0wMgpGT1hBMjtjb2JpbmRlcl80O01BMTEyMi4xO1RGRFAxOzMsMzQ0MTVlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUExMTIyLjE7VEZEUDE7MywzNDQxNWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNQTExMjIuMTtURkRQMTszLDM0NDE1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wOTMwNV8yLjAwO05SNEEzOzMsMzU4NzJlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA5MzA1XzIuMDA7TlI0QTM7MywzNTg3MmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDkzMDVfMi4wMDtOUjRBMzszLDM1ODcyZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wOTMwNV8yLjAwO05SNEEzOzMsMzU4NzJlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4MzEzXzIuMDA7Wk5GNDE7MywzODQ4MGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDgzNzhfMi4wMDtaRlAyODszLDM4NDgwZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODc3MF8yLjAwO05FVVJPRDQsTkVVUk9ENjszLDQwNjc0ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wODMxMV8yLjAwO1pORjE4OTszLDQxMTkyZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzYzM18yLjAwO1pJSzE7Myw0MTMyNmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDgzNDRfMi4wMDtaTkY0NDk7Myw0MTMyNmUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDExNDNfMi4wMDtDUkVCM0wyOzMsNDM0MTBlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4MjY0XzIuMDA7Wk5GMjUwOzMsNDQxNzJlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4MjY0XzIuMDA7Wk5GMjUwOzMsNDQxNzJlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA1NTE0XzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7Myw0NDI3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDU1MTRfMi4wMDtIU0ZZMixIU0ZYMSxIU0ZYMjszLDQ0Mjc5ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wNTUxNF8yLjAwO0hTRlkyLEhTRlgxLEhTRlgyOzMsNDQyNzllLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA1NTE0XzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7Myw0NDI3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDkwNjRfMi4wMDtTUElCOzMsNDQyNzllLTAyCkZPWEEyO2NvYmluZGVyXzc7TUEwNTE4LjE7U1RBVDQ7Myw0ODM3NWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDgzNzNfMi4wMDtaTkY3NzQ7Myw1MTUyMWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDQzNjZfMi4wMDtNQUZHOzMsNTIxMDVlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0MzY5XzIuMDA7TUFGRzszLDUyMTA1ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODI0N18yLjAwO1pORjM4MjszLDUyMTA1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNTUzNV8yLjAwO0lSRjU7Myw1NDk1OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc2ODlfMi4wMDtaTkYzODM7Myw1NTM4NmUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc2ODlfMi4wMDtaTkYzODM7Myw1NTM4NmUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDE4NDlfMi4wMDtaRkhYMzszLDU2MTYyZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMTg0OV8yLjAwO1pGSFgzOzMsNTYxNjJlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAxODQ5XzIuMDA7WkZIWDM7Myw1NjE2MmUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDE4NDlfMi4wMDtaRkhYMzszLDU2MTYyZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMTg0OV8yLjAwO1pGSFgzOzMsNTYxNjJlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0MzQzXzIuMDA7TUFGOzMsNTYxNjJlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0MzQzXzIuMDA7TUFGOzMsNTYxNjJlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0MzQzXzIuMDA7TUFGOzMsNTYxNjJlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0MzQzXzIuMDA7TUFGOzMsNTYxNjJlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0MjgwXzIuMDA7TlJMOzMsNTY4MzNlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0MjgwXzIuMDA7TlJMOzMsNTY4MzNlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA0MjgwXzIuMDA7TlJMOzMsNTY4MzNlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4OTQwXzIuMDA7WkJUQjY7Myw1NjgzM2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg5NDBfMi4wMDtaQlRCNjszLDU2ODMzZS0wMgpGT1hBMjtjb2JpbmRlcl82O1VOMDMzMi4xO1pORjUzNDszLDU2ODMzZS0wMgpGT1hBMjtjb2JpbmRlcl82O1VOMDYzNy4xO1pORjU4NUE7Myw1NjgzM2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc3MjhfMi4wMDtaTkY4MTszLDU3Mzk5ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wNzcyOF8yLjAwO1pORjgxOzMsNTczOTllLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NzI4XzIuMDA7Wk5GODE7Myw1NzM5OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc3NzJfMi4wMDtaTkY1NTA7Myw1NzM5OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTExNDkuMTtSQVJBOjpSWFJHOzMsNTczOTllLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wNjQ2LjE7Wk5GNjYyOzMsNTczOTllLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUEwMDQzLjM7SExGOzMsNTg1OTJlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4OTU3XzIuMDA7Wk5GMTM0OzMsNjA3NTRlLTAyCkZPWEEyO2NvYmluZGVyXzU7VU4wMTUzLjE7WkZQMzszLDYwNzU1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO1VOMDMwNS4xO0FETlA7Myw2MzQ1MWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtVTjAzMDUuMTtBRE5QOzMsNjM0NTFlLTAyCkZPWEEyO2NvYmluZGVyXzA7VU4wMzA1LjE7QUROUDszLDYzNDUxZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODMxM18yLjAwO1pORjQxOzMsNjc3MzJlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4ODc0XzIuMDA7WktTQ0FOMTszLDY4Mzc5ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wODg3NF8yLjAwO1pLU0NBTjE7Myw2ODM3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg4NzRfMi4wMDtaS1NDQU4xOzMsNjgzNzllLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4ODc0XzIuMDA7WktTQ0FOMTszLDY4Mzc5ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wODg3NF8yLjAwO1pLU0NBTjE7Myw2ODM3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDkyMzVfMi4wMDtJUkY0OzMsNzAxNzhlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA5MjM1XzIuMDA7SVJGNDszLDcwMTc4ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wOTIzNV8yLjAwO0lSRjQ7Myw3MDE3OGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDkyMzVfMi4wMDtJUkY0OzMsNzAxNzhlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA5MzA2XzIuMDA7TlI0QTM7Myw3MDY0MGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDkzMDZfMi4wMDtOUjRBMzszLDcwNjQwZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wOTMwNl8yLjAwO05SNEEzOzMsNzA2NDBlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA5MzA2XzIuMDA7TlI0QTM7Myw3MDY0MGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDQzNDdfMi4wMDtNQUY7Myw3MjE0N2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDQzNDdfMi4wMDtNQUY7Myw3MjE0N2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDQzNDdfMi4wMDtNQUY7Myw3MjE0N2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDQzNDdfMi4wMDtNQUY7Myw3MjE0N2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtVTjA2MTIuMTtaTkYzNTA7Myw3MjE0N2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtVTjA2MTIuMTtaTkYzNTA7Myw3MjE0N2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDE2NTZfMi4wMDtBUklEM0IsQVJJRDNDOzMsNzMwNDhlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAxNjU2XzIuMDA7QVJJRDNCLEFSSUQzQzszLDczMDQ4ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wMTY1Nl8yLjAwO0FSSUQzQixBUklEM0M7Myw3MzA0OGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDI0MzVfMi4wMDtMQ09SOzMsNzMwNDhlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAyNDM1XzIuMDA7TENPUjszLDczMDQ4ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzU4NF8yLjAwO1pORjMxNzszLDczMDYzZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODMxOV8yLjAwO1pORjM4MjszLDczMDYzZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMTI0N18yLjAwO0RVWEE7Myw3MzMzNGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDI0MzhfMi4wMDtMQ09SOzMsNzMzMzRlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAyNDM4XzIuMDA7TENPUjszLDczMzM0ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO1VOMDYzNy4xO1pORjU4NUE7Myw3MzQxNWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDc2OTRfMi4wMDtaTkY1Mjc7Myw3NDQ5MmUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDc3MThfMi4wMDtaTkY2ODI7Myw3NDQ5MmUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDc3NjlfMi4wMDtaTkYzMjRCOzMsNzQ0OTJlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA4MzQzXzIuMDA7Wk5GNjgwOzMsNzQ0OTJlLTAyCkZPWEEyO2NvYmluZGVyXzU7VU4wNDkwLjE7RTJGMTo6SEVTNzszLDc0NDkyZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNDY2MF8yLjAwO01CTkwyOzMsNzQ1OTllLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA0NjYwXzIuMDA7TUJOTDI7Myw3NDU5OWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDQ2NjBfMi4wMDtNQk5MMjszLDc0NTk5ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMTI0Nl8yLjAwO0hEWDszLDc0ODE3ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMTI0Nl8yLjAwO0hEWDszLDc0ODE3ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODkxNl8yLjAwO1pORjI3NDszLDc4MTI3ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODkxNl8yLjAwO1pORjI3NDszLDc4MTI3ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODkxNl8yLjAwO1pORjI3NDszLDc4MTI3ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODkxNl8yLjAwO1pORjI3NDszLDc4MTI3ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wODkxNF8yLjAwO1pORjM1NEE7Myw3OTg5NmUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDg5MTRfMi4wMDtaTkYzNTRBOzMsNzk4OTZlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA4OTE0XzIuMDA7Wk5GMzU0QTszLDc5ODk2ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wODkxNF8yLjAwO1pORjM1NEE7Myw3OTg5NmUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDg5MTRfMi4wMDtaTkYzNTRBOzMsNzk4OTZlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA4OTE0XzIuMDA7Wk5GMzU0QTszLDc5ODk2ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wNzU2N18yLjAwO1pORjY3MTszLDgwMTQxZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wOTUzN18yLjAwO1NQSUI7Myw4MDE0MWUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDA0MTFfMi4wMDtUUFJYMTszLDgwMjYyZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMDQxNV8yLjAwO1RQUlgxOzMsODAyNjJlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAwNDQxXzIuMDA7VFBSWDE7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDEzMjJfMi4wMDtMSU41NDszLDgwMjYyZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMTMyMl8yLjAwO0xJTjU0OzMsODAyNjJlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAxMzIyXzIuMDA7TElONTQ7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDEzMjJfMi4wMDtMSU41NDszLDgwMjYyZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMTY2Nl8yLjAwO0FSSUQzQixBUklEM0M7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDE2NjZfMi4wMDtBUklEM0IsQVJJRDNDOzMsODAyNjJlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAxNjY2XzIuMDA7QVJJRDNCLEFSSUQzQzszLDgwMjYyZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMjEyM18yLjAwO1RQUlgxOzMsODAyNjJlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAyNDM4XzIuMDA7TENPUjszLDgwMjYyZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMjQzOF8yLjAwO0xDT1I7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMxMzVfMi4wMDtIT1hDMTI7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMxMzVfMi4wMDtIT1hDMTI7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMxMzVfMi4wMDtIT1hDMTI7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMyMDZfMi4wMDtIT1hEMTI7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMzMDZfMi4wMDtQT1UyRjM7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMzMDZfMi4wMDtQT1UyRjM7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMzMDZfMi4wMDtQT1UyRjM7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMzMDZfMi4wMDtQT1UyRjM7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMzMDZfMi4wMDtQT1UyRjM7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMzMDZfMi4wMDtQT1UyRjM7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMzMDZfMi4wMDtQT1UyRjM7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDUxODBfMi4wMDtITUJPWDE7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDUxODBfMi4wMDtITUJPWDE7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDUxODBfMi4wMDtITUJPWDE7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDUxODBfMi4wMDtITUJPWDE7Myw4MDI2MmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDg5NTNfMi4wMDtaTkY2Njc7Myw4MzgyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMTtVTjAzMDUuMTtBRE5QOzMsODQxNTVlLTAyCkZPWEEyO2NvYmluZGVyXzE7VU4wMzA1LjE7QUROUDszLDg0MTU1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO1VOMDMwNS4xO0FETlA7Myw4NDE1NWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg4NThfMi4wMDtaTkYzMjQ7Myw4NTE4M2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg4NThfMi4wMDtaTkYzMjQ7Myw4NTE4M2UtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDQzNzBfMi4wMDtNQUZHOzMsODUzNDdlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wNjEyLjE7Wk5GMzUwOzMsODUzNDdlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wNjEyLjE7Wk5GMzUwOzMsODUzNDdlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAyNTM4XzIuMDA7VEhBUDEyOzMsODYyOTdlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAyNTM4XzIuMDA7VEhBUDEyOzMsODYyOTdlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAyNTM4XzIuMDA7VEhBUDEyOzMsODYyOTdlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAyNTM4XzIuMDA7VEhBUDEyOzMsODYyOTdlLTAyCkZPWEEyO2NvYmluZGVyXzA7TUEwMDQ3LjM7Rk9YQTI7Myw4Njc3NWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNQTAwNDcuMztGT1hBMjszLDg2Nzc1ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO01BMDA0Ny4zO0ZPWEEyOzMsODY3NzVlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAzMTMyXzIuMDA7SE9YQzExOzMsODgzODVlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA1MDgwXzIuMDA7SE9YQzExOzMsODgzODVlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA1NjU1XzIuMDA7RVNSUkE7Myw4ODM4NWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDU2NTVfMi4wMDtFU1JSQTszLDg4Mzg1ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNTY1NV8yLjAwO0VTUlJBOzMsODgzODVlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA1NjU1XzIuMDA7RVNSUkE7Myw4ODM4NWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDU2NTVfMi4wMDtFU1JSQTszLDg4Mzg1ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNTY1Nl8yLjAwO0VTUlJBOzMsODgzODVlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA1NjU2XzIuMDA7RVNSUkE7Myw4ODM4NWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDU2NTZfMi4wMDtFU1JSQTszLDg4Mzg1ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNTY1Nl8yLjAwO0VTUlJBOzMsODgzODVlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA1NjU2XzIuMDA7RVNSUkE7Myw4ODM4NWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDU2NzNfMi4wMDtFU1JSRzszLDg4Mzg1ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNTY3M18yLjAwO0VTUlJHOzMsODgzODVlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA1NjczXzIuMDA7RVNSUkc7Myw4ODM4NWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDU2NzNfMi4wMDtFU1JSRzszLDg4Mzg1ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNTY3M18yLjAwO0VTUlJHOzMsODgzODVlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA1Njc2XzIuMDA7RVNSUkc7Myw4ODM4NWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDU2NzZfMi4wMDtFU1JSRzszLDg4Mzg1ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNTY3Nl8yLjAwO0VTUlJHOzMsODgzODVlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA1Njc2XzIuMDA7RVNSUkc7Myw4ODM4NWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDU2NzZfMi4wMDtFU1JSRzszLDg4Mzg1ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNzczM18yLjAwO1pORjgyMzszLDg4ODA1ZS0wMgpGT1hBMjtjb2JpbmRlcl83O1VOMDMzNi4xO1pORjY3MTszLDg4ODA1ZS0wMgpGT1hBMjtjb2JpbmRlcl83O1VOMDUzNS4xO0ZPWE8xOjpFTEYxOzMsODg4MDVlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NTg1XzIuMDA7Wk5GMzMxOzMsOTAwMjVlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NTg1XzIuMDA7Wk5GMzMxOzMsOTAwMjVlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NTg1XzIuMDA7Wk5GMzMxOzMsOTAwMjVlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NjE4XzIuMDA7Wk5GNzAxOzMsOTAwMjVlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NzI1XzIuMDA7Wk5GNjE1OzMsOTAwMjVlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wNjY1LjE7Wk5GODgwOzMsOTAwMjVlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjQ3XzIuMDA7RFVYQTszLDkwNDAzZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wODkwMV8yLjAwO1pORjE4OzMsOTEyNDFlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4OTAxXzIuMDA7Wk5GMTg7Myw5MTI0MWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg5MDFfMi4wMDtaTkYxODszLDkxMjQxZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wODkwMV8yLjAwO1pORjE4OzMsOTEyNDFlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4OTAxXzIuMDA7Wk5GMTg7Myw5MTI0MWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg5MDFfMi4wMDtaTkYxODszLDkxMjQxZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wODk1MF8yLjAwO1pORjI1NzszLDkxMjQxZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wODk1MF8yLjAwO1pORjI1NzszLDkxMjQxZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDU2M18yLjAwO1pORjQ0OTszLDkyODk5ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDYwOV8yLjAwO1pORjUwMTszLDkyODk5ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDYwOV8yLjAwO1pORjUwMTszLDkyODk5ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNzYyNF8yLjAwO1pORjc3ODszLDkyODk5ZS0wMgpGT1hBMjtjb2JpbmRlcl81O01BMTk5Mi4xO0lLWkYzOzMsOTI4OTllLTAyCkZPWEEyO2NvYmluZGVyXzU7TUExOTkyLjE7SUtaRjM7Myw5Mjg5OWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNQTE5OTIuMTtJS1pGMzszLDkyODk5ZS0wMgpGT1hBMjtjb2JpbmRlcl81O01BMTk5Mi4xO0lLWkYzOzMsOTI4OTllLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA4MzkwXzIuMDA7WlNDQU41QzszLDkzMzg3ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wODM5MF8yLjAwO1pTQ0FONUM7Myw5MzM4N2UtMDIKRk9YQTI7Y29iaW5kZXJfMDtVTjA2MzcuMTtaTkY1ODVBOzMsOTQzMjRlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAwNTE1XzIuMDA7VFBSWDE7Myw5NjEzMGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDE2NTZfMi4wMDtBUklEM0IsQVJJRDNDOzMsOTYxMzBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAxNjU2XzIuMDA7QVJJRDNCLEFSSUQzQzszLDk2MTMwZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wMTY1Nl8yLjAwO0FSSUQzQixBUklEM0M7Myw5NjEzMGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDI0MzFfMi4wMDtMQ09SOzMsOTk0NzRlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAyNDMxXzIuMDA7TENPUjszLDk5NDc0ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODM5MF8yLjAwO1pTQ0FONUM7NCwwMDU3MmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDgzOTBfMi4wMDtaU0NBTjVDOzQsMDA1NzJlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA0NjQxXzIuMDA7Wk5GNTgwOzQsMDE4NzJlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAyODU2XzIuMDA7TUFGSzs0LDAzMjM0ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMjg1Nl8yLjAwO01BRks7NCwwMzIzNGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDA0ODlfMi4wMDtUUFJYMTs0LDA0ODg4ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wMjA5M18yLjAwO1pIWDE7NCwwNDg4OGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDQ5MjBfMi4wMDtHU0MyLFRQUlgxOzQsMDQ4ODhlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA0OTIwXzIuMDA7R1NDMixUUFJYMTs0LDA0ODg4ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wODM0M18yLjAwO1pORjY4MDs0LDA3Njk5ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wMTMwNF8yLjAwO0xDT1JMOzQsMDgwMzNlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAyNTMwXzIuMDA7TElONTQ7NCwwODAzM2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDI1MzBfMi4wMDtMSU41NDs0LDA4MDMzZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wMjUzMF8yLjAwO0xJTjU0OzQsMDgwMzNlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAyNTMwXzIuMDA7TElONTQ7NCwwODAzM2UtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDUzNTBfMi4wMDtQT1U2RjE7NCwwODkwMmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDUzNTBfMi4wMDtQT1U2RjE7NCwwODkwMmUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDUzNTBfMi4wMDtQT1U2RjE7NCwwODkwMmUtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDc3MDZfMi4wMDtaTkY3ODI7NCwxMDEyOGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDgzMTFfMi4wMDtaTkYxODk7NCwxMTE0NWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMTEwNTBfMi4wMDtNWUI7NCwxMTE0NWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMTEwNTBfMi4wMDtNWUI7NCwxMTE0NWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMTEwNTBfMi4wMDtNWUI7NCwxMTE0NWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMTEwNTBfMi4wMDtNWUI7NCwxMTE0NWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNQTExMzcuMTtGT1NMMTo6SlVOQjs0LDExMzQyZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMDIxN18yLjAwO1pORjIwMDs0LDE1NzU5ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wODgxMV8yLjAwO01BRkI7NCwxNTc1OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDg4MTFfMi4wMDtNQUZCOzQsMTU3NTllLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4ODExXzIuMDA7TUFGQjs0LDE1NzU5ZS0wMgpGT1hBMjtjb2JpbmRlcl82O1VOMDYwMi4xO1pORjIyMjs0LDE1NzU5ZS0wMgpGT1hBMjtjb2JpbmRlcl82O1VOMDYzMC4xO1pORjU1NDs0LDE1NzU5ZS0wMgpGT1hBMjtjb2JpbmRlcl82O01BMDYyOS4xO1JIT1gxMTs0LDE4NDc1ZS0wMgpGT1hBMjtjb2JpbmRlcl83O01BMTczMS4xO1pORjc2ODs0LDE4NzM4ZS0wMgpGT1hBMjtjb2JpbmRlcl83O01BMTkzNi4xO0VSRjo6Rk9YTzE7NCwyMTc2NWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNQTE5NDQuMTtFVFY1OjpEUkdYOzQsMjE3NjVlLTAyCkZPWEEyO2NvYmluZGVyXzc7VU4wNjQ4LjE7Wk5GNjc0OzQsMjE3NjVlLTAyCkZPWEEyO2NvYmluZGVyXzc7VU4wNjQ4LjE7Wk5GNjc0OzQsMjE3NjVlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA5MjM0XzIuMDA7SVJGMzs0LDIxNzY5ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wOTMzNl8yLjAwO1RQNzM7NCwyMjI0N2UtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDkzMzZfMi4wMDtUUDczOzQsMjIyNDdlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4NjA5XzIuMDA7VEJQTDI7NCwyMjUyMmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDg2MDlfMi4wMDtUQlBMMjs0LDIyNTIyZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wOTMwNl8yLjAwO05SNEEzOzQsMjI1MjJlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA5MzA2XzIuMDA7TlI0QTM7NCwyMjUyMmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDkzMDZfMi4wMDtOUjRBMzs0LDIyNTIyZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wOTMwNl8yLjAwO05SNEEzOzQsMjI1MjJlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3Nzc4XzIuMDA7Wk5GMjI0OzQsMjI4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3Nzc4XzIuMDA7Wk5GMjI0OzQsMjI4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3Nzc4XzIuMDA7Wk5GMjI0OzQsMjI4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3Nzc4XzIuMDA7Wk5GMjI0OzQsMjI4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3Nzc4XzIuMDA7Wk5GMjI0OzQsMjI4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA3Nzc4XzIuMDA7Wk5GMjI0OzQsMjI4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA0NzAzXzIuMDA7RTJGODs0LDIzMTY4ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wOTAzNV8yLjAwO1RGRFAxLFRGRFAyLFRGRFAzOzQsMjMxNjhlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA5MDM1XzIuMDA7VEZEUDEsVEZEUDIsVEZEUDM7NCwyMzE2OGUtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDkwMzVfMi4wMDtURkRQMSxURkRQMixURkRQMzs0LDIzMTY4ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wOTAzNV8yLjAwO1RGRFAxLFRGRFAyLFRGRFAzOzQsMjMxNjhlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA5MDM1XzIuMDA7VEZEUDEsVEZEUDIsVEZEUDM7NCwyMzE2OGUtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDkwMzVfMi4wMDtURkRQMSxURkRQMixURkRQMzs0LDIzMTY4ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wOTAzNV8yLjAwO1RGRFAxLFRGRFAyLFRGRFAzOzQsMjMxNjhlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA5MDM1XzIuMDA7VEZEUDEsVEZEUDIsVEZEUDM7NCwyMzE2OGUtMDIKRk9YQTI7Y29iaW5kZXJfMztVTjA1ODIuMTtURUFENDo6RUxGMTs0LDIzMTY4ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMTA4N18yLjAwO0xJTjU0OzQsMjM0NTVlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMDg3XzIuMDA7TElONTQ7NCwyMzQ1NWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDEwODdfMi4wMDtMSU41NDs0LDIzNDU1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMTA4N18yLjAwO0xJTjU0OzQsMjM0NTVlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAxMjA2XzIuMDA7VElHRDIsSlJLTDs0LDIzNDU1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMTIwNl8yLjAwO1RJR0QyLEpSS0w7NCwyMzQ1NWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtVTjAzMTcuMTtaTkYxODs0LDI1NjUwZS0wMgpGT1hBMjtjb2JpbmRlcl80O1VOMDMxNy4xO1pORjE4OzQsMjU2NTBlLTAyCkZPWEEyO2NvYmluZGVyXzQ7VU4wMzE3LjE7Wk5GMTg7NCwyNTY1MGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtVTjAzMTcuMTtaTkYxODs0LDI1NjUwZS0wMgpGT1hBMjtjb2JpbmRlcl80O1VOMDMxNy4xO1pORjE4OzQsMjU2NTBlLTAyCkZPWEEyO2NvYmluZGVyXzQ7VU4wMzE3LjE7Wk5GMTg7NCwyNTY1MGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDc5NzhfMi4wMDtJUkY0OzQsMjYwMjRlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA3OTc4XzIuMDA7SVJGNDs0LDI2MDI0ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzk3OF8yLjAwO0lSRjQ7NCwyNjAyNGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDc5NzhfMi4wMDtJUkY0OzQsMjYwMjRlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA5Mzc1XzIuMDA7QUlSRTs0LDI2MDI0ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wOTM3NV8yLjAwO0FJUkU7NCwyNjAyNGUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDkzNzVfMi4wMDtBSVJFOzQsMjYwMjRlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA5Mzc1XzIuMDA7QUlSRTs0LDI2MDI0ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wOTM3NV8yLjAwO0FJUkU7NCwyNjAyNGUtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDgyMzlfMi4wMDtaTkY1NzQ7NCwyNjQ0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDA1MTVfMi4wMDtUUFJYMTs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMTk4M18yLjAwO0ZPWEIyOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAyMTk1XzIuMDA7VFBSWDE7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDI0MzNfMi4wMDtMQ09SOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAyNDMzXzIuMDA7TENPUjs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMjQzNV8yLjAwO0xDT1I7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDI0MzVfMi4wMDtMQ09SOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAyNzQ4XzIuMDA7TkZBVEMxOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAyNzQ4XzIuMDA7TkZBVEMxOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAyNzQ4XzIuMDA7TkZBVEMxOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAyNzQ4XzIuMDA7TkZBVEMxOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAyNzgwXzIuMDA7TVlGNjs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMjc4MF8yLjAwO01ZRjY7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDI3ODBfMi4wMDtNWUY2OzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAyNzgwXzIuMDA7TVlGNjs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzA3Ml8yLjAwO0dSSEwxOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzMDcyXzIuMDA7R1JITDE7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMwNzJfMi4wMDtHUkhMMTs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzA3Ml8yLjAwO0dSSEwxOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzMDc0XzIuMDA7VEZDUDI7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMwNzRfMi4wMDtURkNQMjs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzA3NF8yLjAwO1RGQ1AyOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzMDc0XzIuMDA7VEZDUDI7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMwNzRfMi4wMDtURkNQMjs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzIyNV8yLjAwO0xCWDI7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMyMzZfMi4wMDtETUJYMSxUUFJYMTs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzIzNl8yLjAwO0RNQlgxLFRQUlgxOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzMjM2XzIuMDA7RE1CWDEsVFBSWDE7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMyMzZfMi4wMDtETUJYMSxUUFJYMTs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzU5MF8yLjAwO0FSSUQzQixBUklEM0M7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDM1OTBfMi4wMDtBUklEM0IsQVJJRDNDOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzNTkwXzIuMDA7QVJJRDNCLEFSSUQzQzs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wNDg4N18yLjAwO0dSSEwxOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA0ODg3XzIuMDA7R1JITDE7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDQ4ODdfMi4wMDtHUkhMMTs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wNDg4N18yLjAwO0dSSEwxOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA0ODg4XzIuMDA7R1JITDE7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDQ4ODhfMi4wMDtHUkhMMTs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wNDg4OF8yLjAwO0dSSEwxOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA0ODg4XzIuMDA7R1JITDE7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNQTA2MzQuMTtBTFgzOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TUEwNjM0LjE7QUxYMzs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO01BMDY2Ny4xO01ZRjY7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNQTA2NjcuMTtNWUY2OzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TUEwNjY3LjE7TVlGNjs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO01BMDY2Ny4xO01ZRjY7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNQTA2OTkuMTtMQlgyOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TUExOTY4LjE7VEZDUDI7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNQTE5NjguMTtURkNQMjs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO01BMTk2OC4xO1RGQ1AyOzQsMjY3NjZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TUExOTY4LjE7VEZDUDI7NCwyNjc2NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNQTE5NjguMTtURkNQMjs0LDI2NzY2ZS0wMgpGT1hBMjtjb2JpbmRlcl83O01BMTEyNi4xO0ZPUzo6SlVOOzQsMjkwNjZlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUEwNjIxLjE7TUlYLUE7NCwzMTQyNGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDAzNjNfMi4wMDtQT1U2RjI7NCwzMjE5OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDAzNjNfMi4wMDtQT1U2RjI7NCwzMjE5OWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDAzNjNfMi4wMDtQT1U2RjI7NCwzMjE5OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDAxMTVfMi4wMDtBUklEM0IsQVJJRDNDOzQsMzIyOTRlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAwMTE1XzIuMDA7QVJJRDNCLEFSSUQzQzs0LDMyMjk0ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMDExNV8yLjAwO0FSSUQzQixBUklEM0M7NCwzMjI5NGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDE2NjJfMi4wMDtBUklEM0IsQVJJRDNDOzQsMzIyOTRlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAxNjYyXzIuMDA7QVJJRDNCLEFSSUQzQzs0LDMyMjk0ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMTY2Ml8yLjAwO0FSSUQzQixBUklEM0M7NCwzMjI5NGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDIwOThfMi4wMDtOQU5PR1A4OzQsMzIyOTRlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAyMDk4XzIuMDA7TkFOT0dQODs0LDMyMjk0ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMjEyM18yLjAwO1RQUlgxOzQsMzIyOTRlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAyNDMyXzIuMDA7TENPUjs0LDM0NDkxZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMjQzMl8yLjAwO0xDT1I7NCwzNDQ5MWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDk0MzNfMi4wMDtUQlBMMjs0LDM0NDkxZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wOTQzM18yLjAwO1RCUEwyOzQsMzQ0OTFlLTAyCkZPWEEyO2NvYmluZGVyXzU7VU4wMTg3LjE7Wk5GNDI5OzQsMzU1MjllLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0Mjk4XzIuMDA7Q1JFQjNMNCxDUkVCM0wyOzQsMzU4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0Mjk4XzIuMDA7Q1JFQjNMNCxDUkVCM0wyOzQsMzU4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0Mjk4XzIuMDA7Q1JFQjNMNCxDUkVCM0wyOzQsMzU4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0Mjk4XzIuMDA7Q1JFQjNMNCxDUkVCM0wyOzQsMzU4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0Mjk4XzIuMDA7Q1JFQjNMNCxDUkVCM0wyOzQsMzU4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0Mjk4XzIuMDA7Q1JFQjNMNCxDUkVCM0wyOzQsMzU4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0Mjk4XzIuMDA7Q1JFQjNMNCxDUkVCM0wyOzQsMzU4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MzE0XzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzQsMzU4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MzE0XzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzQsMzU4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MzE0XzIuMDA7Q1JFQjNMMSxDUkVCM0wyOzQsMzU4NjBlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3NTgxXzIuMDA7Wk5GNDg0OzQsMzYwNzFlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA4MzMwXzIuMDA7Wk5GMzA7NCwzNjA3MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDgzOTZfMi4wMDtaTkYzNTA7NCwzNjA3MWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDgzOTZfMi4wMDtaTkYzNTA7NCwzNjA3MWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU1NDJfMi4wMDtJUkY4OzQsMzg0NjhlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA1NTQyXzIuMDA7SVJGODs0LDM4NDY4ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNTU0Ml8yLjAwO0lSRjg7NCwzODQ2OGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDU1NDJfMi4wMDtJUkY4OzQsMzg0NjhlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA1NTQyXzIuMDA7SVJGODs0LDM4NDY4ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNTU0Ml8yLjAwO0lSRjg7NCwzODQ2OGUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDc2NjRfMi4wMDtaTkY3MTY7NCwzOTQ3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDgyNTJfMi4wMDtaTkY0MTU7NCwzOTQ3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDgyNTJfMi4wMDtaTkY0MTU7NCwzOTQ3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDkzNDlfMi4wMDtORkFUQzE7NCwzOTQ3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDkzNDlfMi4wMDtORkFUQzE7NCwzOTQ3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDkzNDlfMi4wMDtORkFUQzE7NCwzOTQ3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDkzNDlfMi4wMDtORkFUQzE7NCwzOTQ3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE3MjcuMTtaTkY0MTc7NCwzOTQ3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE5OTIuMTtJS1pGMzs0LDM5NDc5ZS0wMgpGT1hBMjtjb2JpbmRlcl82O01BMTk5Mi4xO0lLWkYzOzQsMzk0NzllLTAyCkZPWEEyO2NvYmluZGVyXzY7TUExOTkyLjE7SUtaRjM7NCwzOTQ3OWUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNQTE5OTIuMTtJS1pGMzs0LDM5NDc5ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wNzczN18yLjAwO1pORjY2Nzs0LDQxMDEyZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMDQwNV8yLjAwO1NFQk9YOzQsNDIxMTFlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAwNDA1XzIuMDA7U0VCT1g7NCw0MjExMWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDA0MDVfMi4wMDtTRUJPWDs0LDQyMTExZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wMjQzOF8yLjAwO0xDT1I7NCw0MjExMWUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDI0MzhfMi4wMDtMQ09SOzQsNDIxMTFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA3NjU3XzIuMDA7Wk5GODE2OzQsNDc0NjFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA3NzEwXzIuMDA7Wk5GMzNCOzQsNDc0NjFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA3NzEwXzIuMDA7Wk5GMzNCOzQsNDc0NjFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA3NzEwXzIuMDA7Wk5GMzNCOzQsNDc0NjFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA3NzM2XzIuMDA7Wk5GODQ7NCw0NzQ2MWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDgzODBfMi4wMDtaTkY5ODs0LDQ3NDYxZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wODM4MF8yLjAwO1pORjk4OzQsNDc0NjFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUExOTc4LjE7Wk5GMzU0QTs0LDQ3NDYxZS0wMgpGT1hBMjtjb2JpbmRlcl80O01BMTk3OC4xO1pORjM1NEE7NCw0NzQ2MWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNQTE5NzguMTtaTkYzNTRBOzQsNDc0NjFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TUExOTc4LjE7Wk5GMzU0QTs0LDQ3NDYxZS0wMgpGT1hBMjtjb2JpbmRlcl80O01BMTk3OC4xO1pORjM1NEE7NCw0NzQ2MWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNQTE5NzguMTtaTkYzNTRBOzQsNDc0NjFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7VU4wNjQ3LjE7Wk5GNjY0OzQsNDc0NjFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7VU4wNjQ3LjE7Wk5GNjY0OzQsNDc0NjFlLTAyCkZPWEEyO2NvYmluZGVyXzQ7VU4wNjY3LjE7Wk5GOTg7NCw0NzQ2MWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtVTjA2NjcuMTtaTkY5ODs0LDQ3NDYxZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNzYxMV8yLjAwO1pORjEyOzQsNDc5MzJlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3NjExXzIuMDA7Wk5GMTI7NCw0NzkzMmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDc2MTFfMi4wMDtaTkYxMjs0LDQ3OTMyZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wNzYxMV8yLjAwO1pORjEyOzQsNDc5MzJlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA5MjM1XzIuMDA7SVJGNDs0LDQ3OTMyZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wOTIzNV8yLjAwO0lSRjQ7NCw0NzkzMmUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDkyMzVfMi4wMDtJUkY0OzQsNDc5MzJlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA5MjM1XzIuMDA7SVJGNDs0LDQ3OTMyZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wMDI1MV8yLjAwO1pORjY1NTs0LDQ4NTg0ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wMDI1MV8yLjAwO1pORjY1NTs0LDQ4NTg0ZS0wMgpGT1hBMjtjb2JpbmRlcl83O1VOMDMzMi4xO1pORjUzNDs0LDQ5MTA5ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO1VOMDYyOS4xO1pORjU0NDs0LDUwOTU3ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wODk0OF8yLjAwO1pORjQxODs0LDU2ODY0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O01BMDg5Ny4xO0hNWDI7NCw1Njg2NGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNQTA4OTcuMTtITVgyOzQsNTY4NjRlLTAyCkZPWEEyO2NvYmluZGVyXzU7TUEwODk4LjE7SE1YMzs0LDU2ODY0ZS0wMgpGT1hBMjtjb2JpbmRlcl81O01BMDg5OC4xO0hNWDM7NCw1Njg2NGUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNQTA4OTguMTtITVgzOzQsNTY4NjRlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4ODk5XzIuMDA7Wk5GNTQ3OzQsNTcxNDJlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4ODk5XzIuMDA7Wk5GNTQ3OzQsNTcxNDJlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4ODk5XzIuMDA7Wk5GNTQ3OzQsNTcxNDJlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4ODk5XzIuMDA7Wk5GNTQ3OzQsNTcxNDJlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA4ODk5XzIuMDA7Wk5GNTQ3OzQsNTcxNDJlLTAyCkZPWEEyO2NvYmluZGVyXzM7TTA4MjU0XzIuMDA7Wk5GNjIxOzQsNjA3MzllLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA3NzMzXzIuMDA7Wk5GODIzOzQsNjEyNTJlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA1NTEyXzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7NCw2MjYwMGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDU1MTJfMi4wMDtIU0ZZMixIU0ZYMSxIU0ZYMjs0LDYyNjAwZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wNTUxMl8yLjAwO0hTRlkyLEhTRlgxLEhTRlgyOzQsNjI2MDBlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA1NTEyXzIuMDA7SFNGWTIsSFNGWDEsSFNGWDI7NCw2MjYwMGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtVTjAxMjkuMTtIU0ZZMjs0LDYyNjAwZS0wMgpGT1hBMjtjb2JpbmRlcl80O1VOMDEyOS4xO0hTRlkyOzQsNjI2MDBlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAzODUzXzIuMDA7U0VCT1g7NCw2MzIzMWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDM4NTNfMi4wMDtTRUJPWDs0LDYzMjMxZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wMzg1M18yLjAwO1NFQk9YOzQsNjMyMzFlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA0NjYwXzIuMDA7TUJOTDI7NCw2ODQxNGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDQ2NjBfMi4wMDtNQk5MMjs0LDY4NDE0ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wNDY2MF8yLjAwO01CTkwyOzQsNjg0MTRlLTAyCkZPWEEyO2NvYmluZGVyXzc7TUExNjU3LjE7Wk5GNjUyOzQsNjg0MTRlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4ODY0XzIuMDA7UEFUWjE7NCw2OTA5MGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg4NjRfMi4wMDtQQVRaMTs0LDY5MDkwZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODg2NF8yLjAwO1BBVFoxOzQsNjkwOTBlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4ODY0XzIuMDA7UEFUWjE7NCw2OTA5MGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDg4NjRfMi4wMDtQQVRaMTs0LDY5MDkwZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODg2NF8yLjAwO1BBVFoxOzQsNjkwOTBlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA4ODY0XzIuMDA7UEFUWjE7NCw2OTA5MGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDUzNTBfMi4wMDtQT1U2RjE7NCw2OTI2NGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDUzNTBfMi4wMDtQT1U2RjE7NCw2OTI2NGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDUzNTBfMi4wMDtQT1U2RjE7NCw2OTI2NGUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDgzOTBfMi4wMDtaU0NBTjVDOzQsNzAwNjZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4MzkwXzIuMDA7WlNDQU41Qzs0LDcwMDY2ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wOTI5MF8yLjAwO0VTUlJBOzQsNzAwNjZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA5MjkwXzIuMDA7RVNSUkE7NCw3MDA2NmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDkyOTBfMi4wMDtFU1JSQTs0LDcwMDY2ZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wOTI5MF8yLjAwO0VTUlJBOzQsNzAwNjZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA5MjkwXzIuMDA7RVNSUkE7NCw3MDA2NmUtMDIKRk9YQTI7Y29iaW5kZXJfNztNQTE3MjcuMTtaTkY0MTc7NCw3MDA2NmUtMDIKRk9YQTI7Y29iaW5kZXJfNztVTjA2NjQuMTtaTkY4NjA7NCw3MDA2NmUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNQTE5NTQuMTtGT1hPMTo6RUxLMTs0LDcwOTQ0ZS0wMgpGT1hBMjtjb2JpbmRlcl8wO00wMDIxNl8yLjAwO1RCUEwyOzQsNzExNjVlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAwMjE2XzIuMDA7VEJQTDI7NCw3MTE2NWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDgzNDZfMi4wMDtaTkY0NTQ7NCw3MjMwMWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDI0MzNfMi4wMDtMQ09SOzQsNzI2NTdlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAyNDMzXzIuMDA7TENPUjs0LDcyNjU3ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wOTQzM18yLjAwO1RCUEwyOzQsNzI2NTdlLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA5NDMzXzIuMDA7VEJQTDI7NCw3MjY1N2UtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDI3NDdfMi4wMDtORkFUQzE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDI3NDdfMi4wMDtORkFUQzE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDI3NDdfMi4wMDtORkFUQzE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDI3NDdfMi4wMDtORkFUQzE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMwODhfMi4wMDtWU1gxOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzMDg4XzIuMDA7VlNYMTs0LDczMDQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzA4OF8yLjAwO1ZTWDE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMwODhfMi4wMDtWU1gxOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzMDg4XzIuMDA7VlNYMTs0LDczMDQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzA4OF8yLjAwO1ZTWDE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMwODhfMi4wMDtWU1gxOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzMzUxXzIuMDA7TVlCTDE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDMzNTFfMi4wMDtNWUJMMTs0LDczMDQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzQwMF8yLjAwO0VTUlJBOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzNDAwXzIuMDA7RVNSUkE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDM0MDBfMi4wMDtFU1JSQTs0LDczMDQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wMzQwMF8yLjAwO0VTUlJBOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTAzNDAwXzIuMDA7RVNSUkE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDQ2NTZfMi4wMDtTQ1JUMTs0LDczMDQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wNDY1Nl8yLjAwO1NDUlQxOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA1NDY4XzIuMDA7UE9VMkYzOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA1NDY4XzIuMDA7UE9VMkYzOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA1NDY4XzIuMDA7UE9VMkYzOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA1NDY4XzIuMDA7UE9VMkYzOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA1NDY4XzIuMDA7UE9VMkYzOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA1NDY4XzIuMDA7UE9VMkYzOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA1NDY4XzIuMDA7UE9VMkYzOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA5MzcxXzIuMDA7UlVOWDE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDkzNzFfMi4wMDtSVU5YMTs0LDczMDQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wOTM3MV8yLjAwO1JVTlgxOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA5MzcxXzIuMDA7UlVOWDE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDkzNzFfMi4wMDtSVU5YMTs0LDczMDQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8yO00wOTM3MV8yLjAwO1JVTlgxOzQsNzMwNDZlLTAyCkZPWEEyO2NvYmluZGVyXzI7TTA5MzcxXzIuMDA7UlVOWDE7NCw3MzA0NmUtMDIKRk9YQTI7Y29iaW5kZXJfMjtNMDkzNzFfMi4wMDtSVU5YMTs0LDczMDQ2ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wODg5OF8yLjAwO1pORjIxNDs0LDc1NDA1ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO00wODg5OF8yLjAwO1pORjIxNDs0LDc1NDA1ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wMTI1OV8yLjAwO01TQU5URDM7NCw3NzQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDEyNTlfMi4wMDtNU0FOVEQzOzQsNzc0MjdlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAxNjY4XzIuMDA7QVJJRDVBOzQsNzc0MjdlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAxNjY4XzIuMDA7QVJJRDVBOzQsNzc0MjdlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAxNjY4XzIuMDA7QVJJRDVBOzQsNzc0MjdlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0MTI5XzIuMDA7Q0xPQ0s7NCw3NzQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQxMjlfMi4wMDtDTE9DSzs0LDc3NDI3ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDIxN18yLjAwO0hFUzU7NCw3NzQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNQTA4MjEuMjtIRVM1OzQsNzc0MjdlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTA3Njg4XzIuMDA7Wk5GNzkzOzQsNzc0NzdlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTAzMTMyXzIuMDA7SE9YQzExOzQsNzc3MThlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3Njg0XzIuMDA7Wk5GMTk3OzQsNzk0OTFlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3Njg0XzIuMDA7Wk5GMTk3OzQsNzk0OTFlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3Njg0XzIuMDA7Wk5GMTk3OzQsNzk0OTFlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3Njg0XzIuMDA7Wk5GMTk3OzQsNzk0OTFlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3Njg0XzIuMDA7Wk5GMTk3OzQsNzk0OTFlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3Njg0XzIuMDA7Wk5GMTk3OzQsNzk0OTFlLTAyCkZPWEEyO2NvYmluZGVyXzE7TTA3Njg0XzIuMDA7Wk5GMTk3OzQsNzk0OTFlLTAyCkZPWEEyO2NvYmluZGVyXzY7VU4wMzE5LjE7Wk5GMzE2OzQsODA1MzZlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0NTM4XzIuMDA7S0xGMTM7NCw4MzEwMWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQ1MzhfMi4wMDtLTEYxMzs0LDgzMTAxZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDUzOF8yLjAwO0tMRjEzOzQsODMxMDFlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0NTM4XzIuMDA7S0xGMTM7NCw4MzEwMWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQ1MzhfMi4wMDtLTEYxMzs0LDgzMTAxZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDU0MF8yLjAwO0tMRjEzOzQsODMxMDFlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0NTQwXzIuMDA7S0xGMTM7NCw4MzEwMWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQ1NDBfMi4wMDtLTEYxMzs0LDgzMTAxZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wNDU0MF8yLjAwO0tMRjEzOzQsODMxMDFlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTA0NTQwXzIuMDA7S0xGMTM7NCw4MzEwMWUtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQ2NThfMi4wMDtLTEYxNDs0LDgzMTAxZS0wMgpGT1hBMjtjb2JpbmRlcl83O00wMDUyN18yLjAwO1RQUlgxOzQsODMxNTZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzQsODMxNTZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzQsODMxNTZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzQsODMxNTZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzQsODMxNTZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzQsODMxNTZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzQsODMxNTZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzQsODMxNTZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTAxMjA3XzIuMDA7WUJYMixZQlgzOzQsODMxNTZlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4OTE2XzIuMDA7Wk5GMjc0OzQsODQ3MzNlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4OTE2XzIuMDA7Wk5GMjc0OzQsODQ3MzNlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4OTE2XzIuMDA7Wk5GMjc0OzQsODQ3MzNlLTAyCkZPWEEyO2NvYmluZGVyXzc7TTA4OTE2XzIuMDA7Wk5GMjc0OzQsODQ3MzNlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA3Njg5XzIuMDA7Wk5GMzgzOzQsODQ3NTNlLTAyCkZPWEEyO2NvYmluZGVyXzA7TTA3Njg5XzIuMDA7Wk5GMzgzOzQsODQ3NTNlLTAyCkZPWEEyO2NvYmluZGVyXzE7VU4wMjUzLjE7TFlMMTs0LDg1MTc1ZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODg3OF8yLjAwO1pCVEIxNzs0LDg1NjAwZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODg3OF8yLjAwO1pCVEIxNzs0LDg1NjAwZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODg3OF8yLjAwO1pCVEIxNzs0LDg1NjAwZS0wMgpGT1hBMjtjb2JpbmRlcl8xO00wODg3OF8yLjAwO1pCVEIxNzs0LDg1NjAwZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wMjkwM18yLjAwO0tMRjEzOzQsODg2ODdlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAyOTAzXzIuMDA7S0xGMTM7NCw4ODY4N2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDI5MDNfMi4wMDtLTEYxMzs0LDg4Njg3ZS0wMgpGT1hBMjtjb2JpbmRlcl81O00wMjkwM18yLjAwO0tMRjEzOzQsODg2ODdlLTAyCkZPWEEyO2NvYmluZGVyXzU7TTAyOTAzXzIuMDA7S0xGMTM7NCw4ODY4N2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtNMDQ0NzlfMi4wMDtaTkY2NjA7NCw4ODY4N2UtMDIKRk9YQTI7Y29iaW5kZXJfNTtVTjA2MzIuMTtaTkY1NjY7NCw4ODY4N2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDg4ODhfMi4wMDtaTkYzODQ7NCw4OTQ0N2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDg4ODhfMi4wMDtaTkYzODQ7NCw4OTQ0N2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDg4ODhfMi4wMDtaTkYzODQ7NCw4OTQ0N2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDg4ODhfMi4wMDtaTkYzODQ7NCw4OTQ0N2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDg4ODhfMi4wMDtaTkYzODQ7NCw4OTQ0N2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDg4ODhfMi4wMDtaTkYzODQ7NCw4OTQ0N2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDg4ODhfMi4wMDtaTkYzODQ7NCw4OTQ0N2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDg5NTBfMi4wMDtaTkYyNTc7NCw4OTQ0N2UtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDg5NTBfMi4wMDtaTkYyNTc7NCw4OTQ0N2UtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDAzNjBfMi4wMDtQT1U0RjM7NCw5MTI2NWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDAzNjBfMi4wMDtQT1U0RjM7NCw5MTI2NWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDAzNjBfMi4wMDtQT1U0RjM7NCw5MTI2NWUtMDIKRk9YQTI7Y29iaW5kZXJfNztNMDAzNjBfMi4wMDtQT1U0RjM7NCw5MTI2NWUtMDIKRk9YQTI7Y29iaW5kZXJfMDtNMDc3NDZfMi4wMDtaTkY1ODc7NCw5NTg3MGUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDQ0NTlfMi4wMDtaU0NBTjU7NCw5NzAxOWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDQ0NjBfMi4wMDtaU0NBTjU7NCw5NzAxOWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtVTjAyNDguMTtaU0NBTjVBOzQsOTcwMTllLTAyCkZPWEEyO2NvYmluZGVyXzQ7VU4wMjQ4LjE7WlNDQU41QTs0LDk3MDE5ZS0wMgpGT1hBMjtjb2JpbmRlcl80O1VOMDY4MS4xO1pGUDY4Mzs0LDk3MDE5ZS0wMgpGT1hBMjtjb2JpbmRlcl8zO1VOMDI1My4xO0xZTDE7NCw5ODE2MmUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDI0MzhfMi4wMDtMQ09SOzQsOTg0MDllLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTAyNDM4XzIuMDA7TENPUjs0LDk4NDA5ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wMjc0OV8yLjAwO05GQVRDMTs0LDk4NDA5ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wMjc0OV8yLjAwO05GQVRDMTs0LDk4NDA5ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wMjc0OV8yLjAwO05GQVRDMTs0LDk4NDA5ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wMjc0OV8yLjAwO05GQVRDMTs0LDk4NDA5ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wOTMxN18yLjAwO05SNEEzOzQsOTg0MDllLTAyCkZPWEEyO2NvYmluZGVyXzQ7TTA5MzE3XzIuMDA7TlI0QTM7NCw5ODQwOWUtMDIKRk9YQTI7Y29iaW5kZXJfNDtNMDkzMTdfMi4wMDtOUjRBMzs0LDk4NDA5ZS0wMgpGT1hBMjtjb2JpbmRlcl80O00wOTMxN18yLjAwO05SNEEzOzQsOTg0MDllLTAyCkZPWEEyO2NvYmluZGVyXzE7TTAyMjgxXzIuMDA7TkFJRjE7NCw5OTIwOGUtMDIKRk9YQTI7Y29iaW5kZXJfMTtNMDIyODFfMi4wMDtOQUlGMTs0LDk5MjA4ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMTIxMF8yLjAwO0NYWEM1LENYWEM0LFRFVDM7NCw5OTI5NmUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDEyMTBfMi4wMDtDWFhDNSxDWFhDNCxURVQzOzQsOTkyOTZlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAxMjEwXzIuMDA7Q1hYQzUsQ1hYQzQsVEVUMzs0LDk5Mjk2ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMTIxMF8yLjAwO0NYWEM1LENYWEM0LFRFVDM7NCw5OTI5NmUtMDIKRk9YQTI7Y29iaW5kZXJfNjtNMDEyMTBfMi4wMDtDWFhDNSxDWFhDNCxURVQzOzQsOTkyOTZlLTAyCkZPWEEyO2NvYmluZGVyXzY7TTAxMjEwXzIuMDA7Q1hYQzUsQ1hYQzQsVEVUMzs0LDk5Mjk2ZS0wMgpGT1hBMjtjb2JpbmRlcl82O00wMTIxMF8yLjAwO0NYWEM1LENYWEM0LFRFVDM7NCw5OTI5NmUtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDc3NTBfMi4wMDtaTkY3ODk7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDc3NzFfMi4wMDtaTkY2NzQ7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNMDc3NzFfMi4wMDtaTkY2NzQ7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTA2MjQuMjtORkFUQzE7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTA2MjQuMjtORkFUQzE7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTA2MjQuMjtORkFUQzE7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTA2MjQuMjtORkFUQzE7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTE2MDEuMjtaTkY3NUQ7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTE2MDEuMjtaTkY3NUQ7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTE2MDEuMjtaTkY3NUQ7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTE2MDEuMjtaTkY3NUQ7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztNQTE2MDEuMjtaTkY3NUQ7NCw5OTQyN2UtMDIKRk9YQTI7Y29iaW5kZXJfMztVTjA2NjUuMTtaTkY4ODA7NCw5OTQyN2UtMDIK" download="FOXA2_predicted_cobinders.csv">
<button class="btn btn-primary" has_icon="TRUE"><i class="fa fa-save"></i> Download table as csv</button>
</a><!--/html_preserve-->

<p>&nbsp;</p>

<!-- ```{r predicted-pairs-full, cache = TRUE, echo = FALSE, eval = TRUE, fig.cap = "**Table 3B. Significant co-binder TFs, inferred using motif comparison with pooled motif library from all species and when such pairs are not found in PPI data** (displaying top100 significant p-values)", fig.align = "center"} -->

<!-- if (file.exists(novel.predictions.full.file)) { -->

<!--   ## Table: -->
<!--   predicted.pairs.tab <- fread(novel.predictions.full.file, header = TRUE, sep = "\t") -->

<!--   predicted.pairs.tab <- predicted.pairs.tab %>% -->
<!--                          mutate(anchor_tf = folder_name) %>% -->
<!--                          select(anchor_tf, cobinder_id, cobinder_motif_id, -->
<!--                                 cobinder_name, p_value) -->
<!--   predicted.pairs.tab.top100 <- predicted.pairs.tab %>% -->
<!--                          top_n(p_value, n = 100) -->

<!-- } else { -->

<!--   predicted.pairs.tab.top100 <- data.frame(anchor_tf = character(), -->
<!--                                     cobinder_id = character(), -->
<!--                                     cobinder_motif_id = character(), -->
<!--                                     cobinder_name = character(),  -->
<!--                                     tf_pair = character(), -->
<!--                                     p_value = double()) -->
<!-- } -->

<!--   DT::datatable(predicted.pairs.tab.top100, -->
<!--                 style = "default", -->
<!--                 rownames = FALSE, -->
<!--                 options = list(scrollX = TRUE)) -->

<!-- if (file.exists(novel.predictions.full.file)) { -->

<!--   ## Download button: -->
<!--   predicted.pairs.tab %>% -->
<!--     downloadthis::download_this(output_name      = paste0(family_name, "_predicted_cobinders_full"), -->
<!--                                 output_extension = ".csv", -->
<!--                                 button_label     = "Download table as csv", -->
<!--                                 button_type      = "primary", -->
<!--                                 has_icon         = TRUE, -->
<!--                                 icon             = "fa fa-save") -->
<!-- } -->

<!-- ``` -->

<!-- <p>&nbsp;</p> -->

<!-- ## Co-binder matches in the PPI data from Goos et al. (human-only)  -->

<!-- ```{r, goos-PPI-similarity, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.cap = "**Figure 2-H. Co-binder motif similarity with matches in protein-protein interaction (PPI) data from Goos et al.**", fig.align = "center", fig.height = 10, fig.width = 15} -->

<!-- ## determining, if a list is not empty: -->
<!-- if (as.character(goos.PPI.motif.similarity.files) != "NA" | goos.PPI.motif.similarity.files != "NA") { -->

<!--   ## Splitting a string into a vector: -->
<!--   goos.PPI.motif.similarity.files    <- unlist(strsplit(goos.PPI.motif.similarity.files, ",")) -->
<!--   goos.PPI.motif.similarity.pdf      <- unlist(lapply(goos.PPI.motif.similarity.files, -->
<!--                                                       function(p) { -->
<!--                                                         gsub(pattern = ".RData", replacement = ".pdf", x = p)})) -->
<!--   goos.full.PPI.motif.similarity.pdf <- unlist(lapply(goos.PPI.motif.similarity.pdf, -->
<!--                                                       function(pd) { -->
<!--                                                         gsub(pattern = "\\/goos\\/", replacement = "\\/goos_full\\/", x = pd)})) -->
<!--   ## Iterating through a list of plots: -->
<!--   for (i in 1:length(goos.PPI.motif.similarity.files)) { -->

<!--     ## Variables: -->
<!--     goos.ppi.plot.rdata <- goos.PPI.motif.similarity.files[[i]] -->
<!--     cobinder_id <- gsub(basename(goos.ppi.plot.rdata), -->
<!--                         pattern = "_motif_similarity_PPI_plot_with_alignment.RData", -->
<!--                         replacement = "") -->
<!--     goos.full.ppi.plot.rdata <- gsub(goos.ppi.plot.rdata, pattern = "\\/goos\\/", replacement = "\\/goos_full\\/") -->

<!--     ## Header: -->
<!--     cat("###", cobinder_id, " {.tabset .tabset-pills}    \n") -->

<!--     ## Species specific plot: -->
<!--     cat("#### Species-specific motif library {.active}   \n") -->
<!--     load(goos.ppi.plot.rdata) -->
<!--     goos.ppi.plot <- get(load(goos.ppi.plot.rdata)) -->
<!--     print(goos.ppi.plot) -->
<!--     cat('\n') -->

<!--     if (file.exists(goos.full.ppi.plot.rdata)) { -->
<!--       ## Full plot: -->
<!--       cat("#### Pooled motif library \n") -->
<!--       load(goos.full.ppi.plot.rdata) -->
<!--       goos.full.ppi.plot <- get(load(goos.full.ppi.plot.rdata)) -->
<!--       print(goos.full.ppi.plot) -->
<!--       cat('\n') -->
<!--     } -->

<!--     } -->

<!-- } else { -->

<!--   cat(paste0("\n\n", -->
<!--              "## {.unlisted .unnumbered}", -->
<!--              "\n\n", -->
<!--              "<div align = 'center'>", -->
<!--              "\n\n", -->
<!--              "\n\n", -->
<!--              "<p>&nbsp;</p>", -->
<!--              "\n\n", -->
<!--              "<p>&nbsp;</p>", -->
<!--              "\n\n", -->
<!--              "**==>> No significant Goos et al. PPI score for ANCHOR-CO-BINDER pairs. <<==**", -->
<!--              "\n\n", -->
<!--              "</div>", -->
<!--              "## {.unlisted .unnumbered}", -->
<!--              "\n\n")) -->

<!-- } -->

<!-- ``` -->

<!-- ## {.unlisted .unnumbered .toc-ignore} -->

<!-- ```{r, goos-PPI-similarity-button, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->
<!-- if (as.character(goos.PPI.motif.similarity.files) != "NA" | goos.PPI.motif.similarity.files != "NA") { -->

<!--   if (file.exists(goos.PPI.motif.similarity.files[1])) { -->

<!--   downloadthis::download_file(path = as.vector(goos.PPI.motif.similarity.pdf), -->
<!--                               output_name = "goos_ppi_motif_similarity_plots_species_specific_collection", -->
<!--                               button_label = "Download species-specific collection result plots as pdf", -->
<!--                               button_type = "primary", -->
<!--                               has_icon = TRUE, -->
<!--                               icon = "fa fa-save", -->
<!--                               self_contained = FALSE) -->
<!--   } -->
<!-- } -->
<!-- ``` -->

<!-- ```{r, goos-PPI-similarity-button-full, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->
<!-- if (as.character(goos.PPI.motif.similarity.files)[1] != "NA" | goos.PPI.motif.similarity.files != "NA") { -->

<!--   goos.full.PPI.motif.similarity.pdf.paths <- c() -->

<!--   for (file in as.vector(goos.full.PPI.motif.similarity.pdf)) { -->

<!--     if (file.exists(file)) { -->
<!--        goos.full.PPI.motif.similarity.pdf.paths <- c(goos.full.PPI.motif.similarity.pdf.paths, file) -->
<!--     } -->
<!--   } -->

<!--   if (!identical(goos.full.PPI.motif.similarity.pdf.paths, "NULL")) { -->

<!--       downloadthis::download_file(path = as.vector(goos.full.PPI.motif.similarity.pdf.paths), -->
<!--                               output_name = "goos_ppi_motif_similarity_plots_full_collection", -->
<!--                               button_label = "Download full collection result plots as pdf", -->
<!--                               button_type = "primary", -->
<!--                               has_icon = TRUE, -->
<!--                               icon = "fa fa-save", -->
<!--                               self_contained = FALSE) -->
<!--   } -->
<!-- } -->
<!-- ``` -->

<!-- <p>&nbsp;</p> -->

<!-- ### Co-binder-anchor confirmed pairs, based on PPI Goos et al. analysis and comparison with species-specific motif library -->

<!-- <p>&nbsp;</p> -->

<!-- ```{r goos-confirmed-pairs, cache = TRUE, echo = FALSE, eval = TRUE, fig.cap = "**Table 2A-H. Significant co-binding pairs, based on motif similarity (using species-specfic library) and PPI Goos et al. data**", fig.align = "center"} -->

<!-- if (file.exists(goos.confirmed.pairs.tab.file)) { -->

<!--   ## Table: -->
<!--   goos.confirmed.pairs.tab <- fread(goos.confirmed.pairs.tab.file, header = TRUE, sep = "\t") -->

<!--   goos.confirmed.pairs.tab <- goos.confirmed.pairs.tab %>% -->
<!--     select(anchor_tf, cobinder_id, cobinder_motif_id, -->
<!--            cobinder_name, tf_pair, -->
<!--            p_value, combined_score) -->


<!-- } else { -->

<!--   goos.confirmed.pairs.tab <- data.frame(anchor_tf = character(), -->
<!--                                     cobinder_id = character(), -->
<!--                                     cobinder_motif_id = character(), -->
<!--                                     cobinder_name = character(),  -->
<!--                                     tf_pair = character(), -->
<!--                                     p_value = double(),  -->
<!--                                     combined_score = integer()) -->
<!-- } -->

<!--   DT::datatable(goos.confirmed.pairs.tab, -->
<!--                 style = "default", -->
<!--                 rownames = FALSE, -->
<!--                 options = list(scrollX = TRUE)) -->

<!-- if (file.exists(goos.confirmed.pairs.tab.file)) { -->

<!--   ## Download button: -->
<!--   goos.confirmed.pairs.tab %>% -->
<!--     downloadthis::download_this(output_name      = paste0(family_name, "_goos_confirmed_pairs"), -->
<!--                                 output_extension = ".csv", -->
<!--                                 button_label     = "Download table as csv", -->
<!--                                 button_type      = "primary", -->
<!--                                 has_icon         = TRUE, -->
<!--                                 icon             = "fa fa-save") -->
<!-- } -->

<!-- ``` -->

<!-- <p>&nbsp;</p> -->

<!-- ### Co-binder-anchor confirmed pairs, based on PPI analysis and comparison with pooled motif library -->

<!-- <p>&nbsp;</p> -->

<!-- ```{r goos-confirmed-pairs-full, cache = TRUE, echo = FALSE, eval = TRUE, fig.cap = "**Table 2B-H. Significant co-binding pairs, based on motif similarity (using pooled motif library from multiple species) and PPI Goos et al. data**", fig.align = "center"} -->

<!-- if (file.exists(goos.confirmed.pairs.full.tab.file)) { -->

<!--   ## Table: -->
<!--   goos.confirmed.pairs.tab <- fread(goos.confirmed.pairs.full.tab.file, header = TRUE, sep = "\t") -->

<!--   goos.confirmed.pairs.tab <- goos.confirmed.pairs.tab %>% -->
<!--     select(anchor_tf, cobinder_id, cobinder_motif_id, -->
<!--            cobinder_name, tf_pair, -->
<!--            p_value, combined_score) -->


<!-- } else { -->

<!--   goos.confirmed.pairs.tab <- data.frame(anchor_tf = character(), -->
<!--                                     cobinder_id = character(), -->
<!--                                     cobinder_motif_id = character(), -->
<!--                                     cobinder_name = character(),  -->
<!--                                     tf_pair = character(), -->
<!--                                     p_value = double(),  -->
<!--                                     combined_score = integer()) -->
<!-- } -->

<!--   DT::datatable(goos.confirmed.pairs.tab, -->
<!--                 style = "default", -->
<!--                 rownames = FALSE, -->
<!--                 options = list(scrollX = TRUE)) -->

<!-- if (file.exists(goos.confirmed.pairs.full.tab.file)) { -->

<!--   ## Download button: -->
<!--   goos.confirmed.pairs.tab %>% -->
<!--     downloadthis::download_this(output_name      = paste0(family_name, "_goos_confirmed_pairs_full"), -->
<!--                                 output_extension = ".csv", -->
<!--                                 button_label     = "Download table as csv", -->
<!--                                 button_type      = "primary", -->
<!--                                 has_icon         = TRUE, -->
<!--                                 icon             = "fa fa-save") -->
<!-- } -->

<!-- ``` -->

<!-- <p>&nbsp;</p> -->

<!-- ## Co-binder motif similarity when no matches in the PPI data found {.tabset} -->

<!-- ```{r, goos-no-match-similarity, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.cap = "**Figure 3-H. Co-binder motif similarity when no matches in protein-protein interaction (PPI) data from Goos et al. were found for those motif pairs**", fig.align = "center", fig.height = 10, fig.width = 15} -->

<!-- if (as.character(goos.no.mach.motif.similarity.files) != "NA") { -->

<!--   ## Splitting a string into a vector: -->
<!--   goos.no.mach.motif.similarity.files <- unlist(strsplit(goos.no.mach.motif.similarity.files, ",")) -->

<!--   goos.no.match.motif.similarity.pdf      <- unlist(lapply(goos.no.mach.motif.similarity.files, -->
<!--                                           function(p) { -->
<!--                                             gsub(pattern = ".RData", replacement = ".pdf", x = p)})) -->
<!--   goos.full.no.match.motif.similarity.pdf <- unlist(lapply(goos.no.match.motif.similarity.pdf, -->
<!--                                           function(pd) { -->
<!--                                             gsub(pattern = "\\/physical\\/", replacement = "\\/physical_full\\/", x = pd)})) -->

<!--   ## Iterating through a list of plots: -->
<!--   for (i in 1:length(goos.no.mach.motif.similarity.files)) { -->

<!--     ## Variables: -->
<!--     goos.ppi.plot.rdata <- goos.no.mach.motif.similarity.files[[i]] -->
<!--     cobinder_id <- gsub(basename(goos.ppi.plot.rdata), -->
<!--                         pattern = "_no_match_motif_similarity_plot_with_alignment.RData", -->
<!--                         replacement = "") -->
<!--     goos.full.ppi.plot.rdata <- gsub(ppi.plot.rdata, pattern = "\\/goos\\/", replacement = "\\/goos_full\\/") -->

<!--     ## Header: -->
<!--     cat("###", cobinder_id, " {.tabset .tabset-pills}    \n") -->

<!--     ## Species specific plot: -->
<!--     cat("#### Species-specific motif library {.active}   \n") -->
<!--     load(goos.ppi.plot.rdata) -->
<!--     goos.ppi.plot <- get(load(goos.ppi.plot.rdata)) -->
<!--     print(goos.ppi.plot) -->
<!--     cat('\n') -->

<!--     ## Full plot: -->
<!--     cat("#### Pooled motif library \n") -->
<!--     load(goos.full.ppi.plot.rdata) -->
<!--     goos.full.ppi.plot <- get(load(goos.full.ppi.plot.rdata)) -->
<!--     print(goos.full.ppi.plot) -->
<!--     cat('\n') -->
<!--     } -->

<!-- } else { -->

<!--   cat(paste0("\n\n", -->
<!--              "### {.unlisted .unnumbered .toc-ignore}", -->
<!--              "\n\n", -->
<!--              "<div align = 'center'>", -->
<!--              "\n\n", -->
<!--              "\n\n", -->
<!--              "<p>&nbsp;</p>", -->
<!--              "\n\n", -->
<!--              "**==>> No significant match with a collection of known motifs. <<==**", -->
<!--              "\n\n", -->
<!--              "</div>", -->
<!--              "\n\n")) -->

<!-- } -->

<!-- ``` -->

<!-- ## {.unlisted .unnumbered .toc-ignore} -->

<!-- ```{r, goos-no-match-similarity-button, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->

<!-- if (as.character(goos.no.mach.motif.similarity.files) != "NA") { -->

<!--   if (file.exists(goos.no.match.motif.similarity.pdf[1])) { -->

<!--   downloadthis::download_file(path = as.vector(goos.no.match.motif.similarity.pdf), -->
<!--                               output_name = "goos_no_match_motif_similarity_plots_species_specific_collection", -->
<!--                               button_label = "Download species-specific collection result plots as pdf", -->
<!--                               button_type = "primary", -->
<!--                               has_icon = TRUE, -->
<!--                               icon = "fa fa-save", -->
<!--                               self_contained = FALSE) -->
<!--   } -->
<!-- } -->
<!-- ``` -->

<!-- ```{r, goos-no-match-similarity-button-full, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->

<!-- if (as.character(goos.no.mach.motif.similarity.files) != "NA") { -->

<!--   if (file.exists(goos.full.no.match.motif.similarity.pdf[1])) { -->

<!--   downloadthis::download_file(path = as.vector(goos.full.no.match.motif.similarity.pdf), -->
<!--                               output_name = "goos_no_match_motif_similarity_plots_full_collection", -->
<!--                               button_label = "Download full collection result plots as pdf", -->
<!--                               button_type = "primary", -->
<!--                               has_icon = TRUE, -->
<!--                               icon = "fa fa-save", -->
<!--                               self_contained = FALSE) -->
<!--   } -->
<!-- } -->
<!-- ``` -->

<!-- <p>&nbsp;</p> -->

<!-- ### Co-binder-anchor pair predictions, based on motif similarity -->

<!-- <p>&nbsp;</p> -->

<!-- ```{r goos-predicted-pairs, cache = TRUE, echo = FALSE, eval = TRUE, fig.cap = "**Table 3A-H. Significant co-binder TFs, inferred using motif comparison with species-specific motif library and when such pairs are not found in PPI Goos et al. data** (displaying top100 significant p-values)", fig.align = "center"} -->

<!-- if (file.exists(goos.novel.predictions.file)) { -->

<!--   ## Table: -->
<!--   goos.predicted.pairs.tab <- fread(goos.novel.predictions.file, header = TRUE, sep = "\t") -->

<!--   goos.predicted.pairs.tab <- goos.predicted.pairs.tab %>% -->
<!--                          mutate(anchor_tf = folder_name) %>% -->
<!--                          select(anchor_tf, cobinder_id, cobinder_motif_id, -->
<!--                                 cobinder_name, p_value) -->

<!--   goos.predicted.pairs.tab.top100 <- goos.predicted.pairs.tab %>% -->
<!--     top_n(p_value, n = 100) -->

<!-- } else { -->

<!--   goos.predicted.pairs.tab.top100 <- data.frame(anchor_tf = character(), -->
<!--                                     cobinder_id = character(), -->
<!--                                     cobinder_motif_id = character(), -->
<!--                                     cobinder_name = character(),  -->
<!--                                     tf_pair = character(), -->
<!--                                     p_value = double()) -->
<!-- } -->

<!--   DT::datatable(goos.predicted.pairs.tab.top100, -->
<!--                 style = "default", -->
<!--                 rownames = FALSE, -->
<!--                 options = list(scrollX = TRUE)) -->

<!-- if (file.exists(goos.novel.predictions.file)) { -->

<!--   ## Download button: -->
<!--   goos.predicted.pairs.tab %>% -->
<!--     downloadthis::download_this(output_name      = paste0(family_name, "_goos_predicted_cobinders"), -->
<!--                                 output_extension = ".csv", -->
<!--                                 button_label     = "Download table as csv", -->
<!--                                 button_type      = "primary", -->
<!--                                 has_icon         = TRUE, -->
<!--                                 icon             = "fa fa-save") -->
<!-- } -->

<!-- ``` -->

<!-- <p>&nbsp;</p> -->

<!-- ```{r goos-predicted-pairs-full, cache = TRUE, echo = FALSE, eval = TRUE, fig.cap = "**Table 3B-H. Significant co-binder TFs, inferred using motif comparison with pooled motif library from all species and when such pairs are not found in PPI Goos er al. data** (displaying top100 significant p-values)", fig.align = "center"} -->

<!-- if (file.exists(goos.novel.predictions.full.file)) { -->

<!--   ## Table: -->
<!--   goos.predicted.pairs.tab <- fread(goos.novel.predictions.full.file, header = TRUE, sep = "\t") -->

<!--   goos.predicted.pairs.tab <- goos.predicted.pairs.tab %>% -->
<!--                          mutate(anchor_tf = folder_name) %>% -->
<!--                          select(anchor_tf, cobinder_id, cobinder_motif_id, -->
<!--                                 cobinder_name, p_value) -->

<!--   goos.predicted.pairs.tab.top100 <- goos.predicted.pairs.tab %>% -->
<!--     top_n(p_value, n = 100) -->

<!-- } else { -->

<!--   goos.predicted.pairs.tab.top100 <- data.frame(anchor_tf = character(), -->
<!--                                     cobinder_id = character(), -->
<!--                                     cobinder_motif_id = character(), -->
<!--                                     cobinder_name = character(),  -->
<!--                                     tf_pair = character(), -->
<!--                                     p_value = double()) -->
<!-- } -->

<!--   DT::datatable(goos.predicted.pairs.tab.top100, -->
<!--                 style = "default", -->
<!--                 rownames = FALSE, -->
<!--                 options = list(scrollX = TRUE)) -->

<!-- if (file.exists(goos.novel.predictions.full.file)) { -->

<!--   ## Download button: -->
<!--   goos.predicted.pairs.tab %>% -->
<!--     downloadthis::download_this(output_name      = paste0(family_name, "_goos_predicted_cobinders_full"), -->
<!--                                 output_extension = ".csv", -->
<!--                                 button_label     = "Download table as csv", -->
<!--                                 button_type      = "primary", -->
<!--                                 has_icon         = TRUE, -->
<!--                                 icon             = "fa fa-save") -->
<!-- } -->

<!-- ``` -->

<p>&nbsp;</p>

# Annotation of co-binder regions {.tabset}

<div align = "justify">
Regions with and without co-binder are annotated using ChIPseeker package. *Co-binder only* are only co-binder regions extracted and annotated, while *Full* regions consists of anchors + flanks.
</div>

<p>&nbsp;</p>

## Full 

<div class="figure">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/annotations-1.png" alt="**Figure 4. Co-binder regions annotations. Co-binder-specific cobinder-only and full (anchor and co-binder) regions together with regions with and without co-binders.**" width="672" />
<p class="caption">**Figure 4. Co-binder regions annotations. Co-binder-specific cobinder-only and full (anchor and co-binder) regions together with regions with and without co-binders.**</p>
</div>

# {.unlisted .unnumbered .toc-ignore}

<!-- ```{r, annotations-button-centered, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->

<!-- if (file.exists(centered.region.anno)) { -->

<!--   download_file(path = as.vector(centered.region.anno.pdf), -->
<!--                 output_name = "cobinders_only_region_annotations", -->
<!--                 button_label = "Download co-binder regions annotation results as pdf", -->
<!--                 button_type = "primary", -->
<!--                 has_icon = TRUE, -->
<!--                 icon = "fa fa-save", -->
<!--                 self_contained = FALSE) -->
<!-- } -->
<!-- ``` -->

<!-- ```{r, annotations-button-full, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->

<!-- if (file.exists(full.region.anno)) { -->

<!--   download_file(path = as.vector(full.region.anno.pdf), -->
<!--                 output_name = "full_cobinders_region_annotations", -->
<!--                 button_label = "Download full co-binder regions annotation results as pdf", -->
<!--                 button_type = "primary", -->
<!--                 has_icon = TRUE, -->
<!--                 icon = "fa fa-save", -->
<!--                 self_contained = FALSE) -->
<!-- } -->
<!-- ``` -->

<p>&nbsp;</p>

# Conservation of regions with and without co-binders {.tabset}

<div align = "justify">
Conservation is analyzed for regions where co-binder was discovered relative to the anchor and also for the regions where none of the co-binders were not found. Chosen window to compute the conservation is 100 bp centering around the anchor motif.
</div>

<p>&nbsp;</p>

## cobinder_0_left_12     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-1.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_0_left_18     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-2.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_0_left_3     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-3.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_0_left_6     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-4.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_0_right_10     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-5.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_0_right_14     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-6.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_0_right_15     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-7.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_0_right_16     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-8.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_0_right_18     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-9.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_0_right_19     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-10.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_0_right_2     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-11.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_0_right_4     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-12.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_1_left_15     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-13.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_1_left_2     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-14.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_1_right_15     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-15.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_1_right_2     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-16.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_1_right_9     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-17.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_2_left_2     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-18.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_3_left_2     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-19.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_4_left_2     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-20.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_5_left_2     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-21.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_6_left_2     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-22.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_7_left_2     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_FOXA2_files/figure-html/conservation-analysis-23.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>

# {.unlisted .unnumbered .toc-ignore}

<!-- ```{r, conservation-buttons, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->

<!-- if (as.character(conservation.plot.files) != "NA") { -->

<!-- downloadthis::download_file(path = as.vector(conservation.plot.files.pdf), -->
<!--                             output_name = "conservation_plots", -->
<!--                             button_label = "Download conservation plots as pdf", -->
<!--                             button_type = "primary", -->
<!--                             has_icon = TRUE, -->
<!--                             icon = "fa fa-save", -->
<!--                             self_contained = FALSE) -->
<!-- } -->
<!-- ``` -->

<p>&nbsp;</p>

<!-- ```{r conservation-statistics, cache = TRUE, echo = FALSE, eval = TRUE, fig.cap = "**Table 4. Conservation comparison of anchor and co-binder regions with and without co-binders.**", fig.align = "center"} -->

<!-- if (file.exists(conservation.statistics.tab.file)) { -->

<!--   ## Table: -->
<!--   conservation.statistics.tab <- fread(conservation.statistics.tab.file, header = TRUE, sep = "\t") -->
<!-- } else { -->

<!--   conservation.statistics.tab <- data.frame(cobinder_id = character(), -->
<!--                                             conservation_score = character(), -->
<!--                                             type_of_region = character(),  -->
<!--                                             p_value = character(), -->
<!--                                             p_value_formatted = double()) -->
<!-- } -->

<!--   DT::datatable(conservation.statistics.tab, -->
<!--                 style = "default", -->
<!--                 rownames = FALSE, -->
<!--                 options = list(scrollX = TRUE)) -->

<!-- # if (file.exists(conservation.statistics.tab.file)) { -->
<!-- #      -->
<!-- #   ## Download button: -->
<!-- #   conservation.statistics.tab %>% -->
<!-- #     downloadthis::download_this(output_name      = paste0(family_name, "_conservation_statistics"), -->
<!-- #                                 output_extension = ".csv", -->
<!-- #                                 button_label     = "Download table as csv", -->
<!-- #                                 button_type      = "primary", -->
<!-- #                                 has_icon         = TRUE, -->
<!-- #                                 icon             = "fa fa-save") -->
<!-- # } -->

<!-- ``` -->

<!-- <p>&nbsp;</p> -->

<!-- # Co-binder region enrichment analysis with GREAT {.tabset .tabset-pills} -->

<!-- <div align = "justify"> -->
<!-- Optional GREAT analysis is performed on regions with and without co-binders for each co-binder. Bellow you can see top20 ontology terms for different ontologies available. All resulting plots and tables can be downloaded bellow. -->
<!-- </div> -->

<!-- <p>&nbsp;</p> -->

<!-- ```{r great-analysis, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.cap = "**Figure 6. GREAT analysis results for different co-binders.**", fig.align = "center", fig.height = 8, fig.width = 9} -->

<!-- if (as.character(great.plot.dirs) != "NA") { -->

<!--   ## Splitting a string into a vector: -->
<!--   great.plot.directories <- unlist(strsplit(great.plot.dirs, ",")) -->

<!--   ## Iterating through a list of directories: -->
<!--   for (i in 1:length(great.plot.directories)) { -->

<!--     ## Variables: -->
<!--     cobinder_dir <- great.plot.directories[[i]] -->
<!--     cobinder_id  <- basename(cobinder_dir) -->

<!--     ## Header: -->
<!--     cat("##", cobinder_id, " {.tabset .tabset-pills}    \n") -->

<!--     ## Listing ontology directories: -->
<!--     ontologies.dirs <- list.dirs(file.path(cobinder_dir, "with_cobinder"), -->
<!--                                 full.names = TRUE, recursive = FALSE) -->
<!--     # with.cobinder.dir  <- file.path(cobinder_dir, "with_cobinder") -->
<!--     # list_of_ontologies <- c("Ensembl_Genes", -->
<!--     #                         "GO_Biological_Process", -->
<!--     #                         "GO_Cellular_Component",  -->
<!--     #                         "GO_Molecular_Function",  -->
<!--     #                         "Human_Phenotype", -->
<!--     #                         "Mouse_Phenotype_Single_KO",  -->
<!--     #                         "Mouse_Phenotype") -->
<!--     # ontologies.dirs   <- unlist(lapply(list_of_ontologies, -->
<!--     #                                function(o) { -->
<!--     #                                  file.path(with.cobinder.dir, o)})) -->

<!--     ## Iterating through ontologies to plot them: -->
<!--     for (j in 1:length(ontologies.dirs)) { -->

<!--       ontology_dir  <- ontologies.dirs[[j]] -->
<!--       ontology_name <- basename(ontology_dir) -->

<!--       ## Ontology header: -->
<!--       cat("###", ontology_name, " {.tabset .tabset-pills}    \n") -->

<!--       ## With co-binder: -->
<!--       cat("#### With co-binder {.active}   \n") -->
<!--       with.ontology.plot.path <- file.path(ontology_dir, paste0(ontology_name, ".RData")) -->
<!--       if (file.exists(with.ontology.plot.path)) { -->
<!--           load(with.ontology.plot.path) -->
<!--           # with_ontology_plot      <- get(load(with.ontology.plot.path)) -->
<!--           with_ontology_plot <- ontology_plot -->
<!--           print(with_ontology_plot) -->
<!--           cat('\n') -->
<!--       } else { -->

<!--       cat(paste0( -->
<!--         "<div align = 'center'>", -->
<!--         "*>> No plot for ontology available. <<*" -->
<!--         )) -->

<!--       } -->

<!--       ## No co-binder: -->
<!--       cat("##### No co-binder {.active}   \n") -->
<!--       no.ontology.plot.path <- gsub(with.ontology.plot.path, pattern = "\\/with_cobinder\\/", replacement = "\\/no_cobinder\\/") -->

<!--       if (file.exists(no.ontology.plot.path)) { -->

<!--       load(no.ontology.plot.path) -->
<!--       # no_ontology_plot      <- get(load(no.ontology.plot.path)) -->
<!--       no_ontology_plot <- ontology_plot -->
<!--       print(no_ontology_plot) -->
<!--       cat('\n') -->

<!--       } else { -->

<!--       cat(paste0( -->
<!--         "<div align = 'center'>", -->
<!--         "*>> No plot for ontology available. <<*" -->
<!--         )) -->
<!--       } -->
<!--     } -->
<!--   } -->

<!-- } else { -->

<!--   cat(paste0("\n\n", -->
<!--              "### {.unlisted .unnumbered .toc-ignore}", -->
<!--              "\n\n", -->
<!--              "<div align = 'center'>", -->
<!--              "\n\n", -->
<!--              "\n\n", -->
<!--              "<p>&nbsp;</p>", -->
<!--              "\n\n", -->
<!--              "**==>> No GREAT analysis results available. <<==**", -->
<!--              "\n\n", -->
<!--              "</div>", -->
<!--              "\n\n")) -->

<!-- } -->

<!-- ``` -->

<!-- ## {.unlisted .unnumbered .toc-ignore} -->

<!-- ```{r, GREAT-analysis-button, results = 'asis', cache = TRUE, echo = FALSE, eval = TRUE, fig.align = "center"} -->

<!-- if (as.character(great.plot.dirs) != "NA") { -->

<!--   great.plot.directories <- unlist(strsplit(great.plot.dirs, ",")) -->
<!--   great.plot.directories <- dirname(great.plot.directories[[1]]) -->
<!--   downloadthis::download_dir(path = great.plot.directories, -->
<!--                              output_name = "cobinder_specific_great_analysis_results", -->
<!--                              button_label = "Download all co-binder-specific GREAT analysis results", -->
<!--                              button_type = "primary", -->
<!--                              has_icon = TRUE, -->
<!--                              icon = "fa fa-save", -->
<!--                              self_contained = FALSE) -->
<!-- } -->
<!-- ``` -->


<p>&nbsp;</p>
<p>&nbsp;</p>


<!-- End of Report -->
