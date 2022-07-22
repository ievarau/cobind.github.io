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
title: RELA
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
<img src="COBIND_analysis_report_RELA_files/figure-html/spacing-summary-plot-1.png" alt="**Figure 1. Spacings summary plot **" width="1920" />
<p class="caption">**Figure 1. Spacings summary plot **</p>
</div>

<p>&nbsp;</p>

## Summary in a table

<div align = "justify">
The spacing summary table consists of all details from co-binder motif discovery. This includes the datasets where the co-binders were found, the NMF details, number of regions in the input file and the fraction of those regions where the co-binder was found. Last columns summarizes the fraction of regions with the co-binder with specific spacer and location.
</div>

<p>&nbsp;</p>
<p>&nbsp;</p>

<!--html_preserve--><a href="data:text/csv;base64,U3ViY2x1c3RlcjtEYXRhc2V0O0ZsYW5rO05iX2NvbXBvbmVudHM7Q29tcG9uZW50O1NwYWNlcl9sZW5ndGg7TG9jYXRpb247TmJfcmVnaW9uc19pbl9pbnB1dF9iZWQ7TmJfcmVnaW9uc193aXRoX2NvYmluZGVyO0ZyYWN0aW9uX29mX3JlZ2lvbnNfd2l0aF9jb2JpbmRlcjtOYl9kYXRhc2V0cztDb2JpbmRlcl9wcm9wb3J0aW9uClN1YmNsdXN0ZXJfMDtIU19EMTAyNl9DMTYwX0o1NV9UMTc3X1JFTEE7cmlnaHQ7Nl9jb21wb25lbnRzOzM7MDtyaWdodDsxMDIzNzsgMjQ5OzAsMDI0OzE1OzAsMDMzClN1YmNsdXN0ZXJfMDtIU19EMTAzMF9DMTUxX0o1NV9UMTc3X1JFTEE7cmlnaHQ7NV9jb21wb25lbnRzOzE7MDtyaWdodDsxMTQyNDsgMzU0OzAsMDMxOzE1OzAsMDMzClN1YmNsdXN0ZXJfMDtIU19EMTAzMF9DMTUxX0o1NV9UMTc3X1JFTEE7cmlnaHQ7Nl9jb21wb25lbnRzOzM7MDtyaWdodDsxMTQyNDsgMzYwOzAsMDMyOzE1OzAsMDMzClN1YmNsdXN0ZXJfMDtIU19EMTAzMV9DMTM1X0o1NV9UMTc3X1JFTEE7cmlnaHQ7NV9jb21wb25lbnRzOzM7MDtyaWdodDsgNzI4NTsgMzA0OzAsMDQyOzE1OzAsMDMzClN1YmNsdXN0ZXJfMDtIU19EMTAzMV9DMTM1X0o1NV9UMTc3X1JFTEE7cmlnaHQ7Nl9jb21wb25lbnRzOzM7MDtyaWdodDsgNzI4NTsgMTkyOzAsMDI2OzE1OzAsMDMzClN1YmNsdXN0ZXJfMDtIU19EMTAzMl9DMTU4X0o1NV9UMTc3X1JFTEE7cmlnaHQ7Nl9jb21wb25lbnRzOzM7MDtyaWdodDsgNzcyNzsgMTkwOzAsMDI1OzE1OzAsMDMzClN1YmNsdXN0ZXJfMDtIU19EMjgyOV9DMjI2X0o1NV9UMTc3X1JFTEE7cmlnaHQ7Nl9jb21wb25lbnRzOzE7MDtyaWdodDs2MDQ0NzsxMDgyOzAsMDE4OzE1OzAsMDMzClN1YmNsdXN0ZXJfMDtIU19EMzEwNV9DMTBfSjU1X1QxNzdfUkVMQTtyaWdodDs2X2NvbXBvbmVudHM7MzswO3JpZ2h0OzM4NjYyOyA5NDQ7MCwwMjQ7MTU7MCwwMzMKU3ViY2x1c3Rlcl8wO0hTX0QzMzFfQzEzNV9KNTVfVDE3N19SRUxBO3JpZ2h0OzZfY29tcG9uZW50czszOzA7cmlnaHQ7IDUwNTY7ICA2MDswLDAxMjsxNTswLDAzMwpTdWJjbHVzdGVyXzA7SFNfRDMzMjBfQzFfSjU1X1QxNzdfUkVMQTtyaWdodDs1X2NvbXBvbmVudHM7NDswO3JpZ2h0OyAzOTc5OyAgNzI7MCwwMTg7MTU7MCwwMzMKU3ViY2x1c3Rlcl8wO0hTX0QzMzg3X0MyMjZfSjU1X1QxNzdfUkVMQTtyaWdodDs1X2NvbXBvbmVudHM7MTswO3JpZ2h0OzE2Nzg4OyA4NTc7MCwwNTE7MTU7MCwwMzMKU3ViY2x1c3Rlcl8wO0hTX0QzMzg3X0MyMjZfSjU1X1QxNzdfUkVMQTtyaWdodDs2X2NvbXBvbmVudHM7MzswO3JpZ2h0OzE2Nzg4OyA1MTc7MCwwMzE7MTU7MCwwMzMKU3ViY2x1c3Rlcl8wO0hTX0QzMzlfQzE1MF9KNTVfVDE3N19SRUxBO3JpZ2h0OzVfY29tcG9uZW50czswOzA7cmlnaHQ7MTQ4ODU7IDU0NTswLDAzNzsxNTswLDAzMwpTdWJjbHVzdGVyXzA7SFNfRDM0MF9DMTUxX0o1NV9UMTc3X1JFTEE7cmlnaHQ7NV9jb21wb25lbnRzOzM7MDtyaWdodDsgMjc2NjsgIDU0OzAsMDIwOzE1OzAsMDMzClN1YmNsdXN0ZXJfMDtIU19EMzQ0X0MxNThfSjU1X1QxNzdfUkVMQTtyaWdodDs2X2NvbXBvbmVudHM7MzswO3JpZ2h0OyA0Nzk4OyAgNjM7MCwwMTM7MTU7MCwwMzMKU3ViY2x1c3Rlcl8wO0hTX0QzNDZfQzE2MF9KNTVfVDE3N19SRUxBO3JpZ2h0OzVfY29tcG9uZW50czszOzA7cmlnaHQ7IDM1MDc7ICA2MjswLDAxODsxNTswLDAzMwpTdWJjbHVzdGVyXzA7SFNfRDM0NzBfQzIyNl9KNTVfVDE3N19SRUxBO3JpZ2h0OzZfY29tcG9uZW50czszOzA7cmlnaHQ7IDY1Njg7IDEzNzswLDAyMTsxNTswLDAzMwpTdWJjbHVzdGVyXzA7SFNfRDM5OTZfQzI2Ml9KNTVfVDE3N19SRUxBO3JpZ2h0OzVfY29tcG9uZW50czswOzA7cmlnaHQ7MTYyMjA7IDM0NjswLDAyMTsxNTswLDAzMwpTdWJjbHVzdGVyXzA7SFNfRDM5OTZfQzI2Ml9KNTVfVDE3N19SRUxBO3JpZ2h0OzZfY29tcG9uZW50czszOzA7cmlnaHQ7MTYyMjA7IDIxMDswLDAxMzsxNTswLDAzMwpTdWJjbHVzdGVyXzE7SFNfRDI4MjdfQzIyNl9KNTVfVDE3N19SRUxBO3JpZ2h0OzVfY29tcG9uZW50czswOzA7cmlnaHQ7MTM1NTQ7IDE5NzswLDAxNTsgMzswLDAxNQpTdWJjbHVzdGVyXzE7SFNfRDI4MjdfQzIyNl9KNTVfVDE3N19SRUxBO3JpZ2h0OzZfY29tcG9uZW50czs1OzA7cmlnaHQ7MTM1NTQ7IDE0MDswLDAxMDsgMzswLDAxNQpTdWJjbHVzdGVyXzE7SFNfRDI4MjhfQzIyNl9KNTVfVDE3N19SRUxBO3JpZ2h0OzVfY29tcG9uZW50czswOzA7cmlnaHQ7NDQ3MDM7IDMyOTswLDAwNzsgMzswLDAxNQpTdWJjbHVzdGVyXzE7SFNfRDI4MjlfQzIyNl9KNTVfVDE3N19SRUxBO3JpZ2h0OzVfY29tcG9uZW50czswOzA7cmlnaHQ7NjA0NDc7IDMxNjswLDAwNTsgMzswLDAxNQpTdWJjbHVzdGVyXzE7SFNfRDI4MjlfQzIyNl9KNTVfVDE3N19SRUxBO3JpZ2h0OzZfY29tcG9uZW50czs1OzA7cmlnaHQ7NjA0NDc7IDQ3MjswLDAwODsgMzswLDAxNQpTdWJjbHVzdGVyXzEwO0hTX0QxMDMyX0MxNThfSjU1X1QxNzdfUkVMQTtyaWdodDs1X2NvbXBvbmVudHM7MDswO3JpZ2h0OyA3NzI3OyAyMzk7MCwwMzE7IDE7MCwwMzEKU3ViY2x1c3Rlcl8yO0hTX0QzMzlfQzE1MF9KNTVfVDE3N19SRUxBO3JpZ2h0OzZfY29tcG9uZW50czsxOzA7cmlnaHQ7MTQ4ODU7IDEzNzswLDAwOTsgODswLDAyMQpTdWJjbHVzdGVyXzI7SFNfRDM0MF9DMTUxX0o1NV9UMTc3X1JFTEE7cmlnaHQ7NV9jb21wb25lbnRzOzI7MDtyaWdodDsgMjc2NjsgIDU5OzAsMDIxOyA4OzAsMDIxClN1YmNsdXN0ZXJfMjtIU19EMzQyX0MxNTZfSjU1X1QxNzdfUkVMQTtyaWdodDs2X2NvbXBvbmVudHM7MTswO3JpZ2h0OyA0NDIyOyAgNTQ7MCwwMTI7IDg7MCwwMjEKU3ViY2x1c3Rlcl8yO0hTX0QzNDRfQzE1OF9KNTVfVDE3N19SRUxBO3JpZ2h0OzZfY29tcG9uZW50czsyOzA7cmlnaHQ7IDQ3OTg7ICA2NTswLDAxNDsgODswLDAyMQpTdWJjbHVzdGVyXzI7SFNfRDM0Nl9DMTYwX0o1NV9UMTc3X1JFTEE7cmlnaHQ7NV9jb21wb25lbnRzOzQ7MDtyaWdodDsgMzUwNzsgIDY0OzAsMDE4OyA4OzAsMDIxClN1YmNsdXN0ZXJfMjtIU19EMzQ2X0MxNjBfSjU1X1QxNzdfUkVMQTtyaWdodDs2X2NvbXBvbmVudHM7MDswO3JpZ2h0OyAzNTA3OyAgNDY7MCwwMTM7IDg7MCwwMjEKU3ViY2x1c3Rlcl8yO0hTX0QzOTkyX0MyNjJfSjU1X1QxNzdfUkVMQTtyaWdodDs2X2NvbXBvbmVudHM7MTswO3JpZ2h0OzEwNjU2OyAgODk7MCwwMDg7IDg7MCwwMjEKU3ViY2x1c3Rlcl8yO0hTX0QzOTk2X0MyNjJfSjU1X1QxNzdfUkVMQTtyaWdodDs1X2NvbXBvbmVudHM7MzswO3JpZ2h0OzE2MjIwOyAyNTk7MCwwMTY7IDg7MCwwMjEKU3ViY2x1c3Rlcl8yO0hTX0QzOTk2X0MyNjJfSjU1X1QxNzdfUkVMQTtyaWdodDs2X2NvbXBvbmVudHM7MjswO3JpZ2h0OzE2MjIwOyAyMDA7MCwwMTI7IDg7MCwwMjEKU3ViY2x1c3Rlcl8yO0hTX0QzOTk4X0MyNjJfSjU1X1QxNzdfUkVMQTtyaWdodDs1X2NvbXBvbmVudHM7MjswO3JpZ2h0OyAyMTI0OyAgNDY7MCwwMjI7IDg7MCwwMjEKU3ViY2x1c3Rlcl8yO0hTX0QzOTk4X0MyNjJfSjU1X1QxNzdfUkVMQTtyaWdodDs2X2NvbXBvbmVudHM7MTswO3JpZ2h0OyAyMTI0OyAgNTg7MCwwMjc7IDg7MCwwMjEKU3ViY2x1c3Rlcl8zO0hTX0QzMzIwX0MxX0o1NV9UMTc3X1JFTEE7bGVmdDs2X2NvbXBvbmVudHM7MDsxO2xlZnQ7IDM5Nzk7ICA5MzswLDAyMzsgMTswLDAyMwpTdWJjbHVzdGVyXzQ7SFNfRDEzOTVfQzI5X0o1NV9UMTc3X1JFTEE7cmlnaHQ7NV9jb21wb25lbnRzOzM7NDtyaWdodDsgNTA5NzsgMTAzOzAsMDIwOyA1OzAsMDY1ClN1YmNsdXN0ZXJfNDtIU19EMTM5NV9DMjlfSjU1X1QxNzdfUkVMQTtyaWdodDs2X2NvbXBvbmVudHM7MDs0O3JpZ2h0OyA1MDk3OyAxNzk7MCwwMzU7IDU7MCwwNjUKU3ViY2x1c3Rlcl80O0hTX0QzMzIzX0MxX0o1NV9UMTc3X1JFTEE7cmlnaHQ7Nl9jb21wb25lbnRzOzQ7NDtyaWdodDsgODMxMTsgMjQyOzAsMDI5OyA1OzAsMDY1ClN1YmNsdXN0ZXJfNDtIU19EMzQ3MV9DMjMwX0o1NV9UMTc3X1JFTEE7cmlnaHQ7Nl9jb21wb25lbnRzOzA7NDtyaWdodDsgOTAwODsgNDI4OzAsMDQ4OyA1OzAsMDY1ClN1YmNsdXN0ZXJfNDtIU19EMzU2N19DMTJfSjU1X1QxNzdfUkVMQTtyaWdodDs0X2NvbXBvbmVudHM7Mjs0O3JpZ2h0OyAzMDAwOyAgOTA7MCwwMzA7IDU7MCwwNjUKU3ViY2x1c3Rlcl80O0hTX0QzNTY3X0MxMl9KNTVfVDE3N19SRUxBO3JpZ2h0OzVfY29tcG9uZW50czsxOzQ7cmlnaHQ7IDMwMDA7ICA5NzswLDAzMjsgNTswLDA2NQpTdWJjbHVzdGVyXzQ7SFNfRDM1NjdfQzEyX0o1NV9UMTc3X1JFTEE7cmlnaHQ7Nl9jb21wb25lbnRzOzI7NDtyaWdodDsgMzAwMDsgIDk4OzAsMDMzOyA1OzAsMDY1ClN1YmNsdXN0ZXJfNDtIU19EMzc3M19DNDEyX0o1NV9UMTc3X1JFTEE7cmlnaHQ7NF9jb21wb25lbnRzOzE7NDtyaWdodDs0MTAyMDsxMDc5OzAsMDI2OyA1OzAsMDY1ClN1YmNsdXN0ZXJfNDtIU19EMzc3M19DNDEyX0o1NV9UMTc3X1JFTEE7cmlnaHQ7NV9jb21wb25lbnRzOzM7NDtyaWdodDs0MTAyMDsyNTIxOzAsMDYxOyA1OzAsMDY1ClN1YmNsdXN0ZXJfNDtIU19EMzc3M19DNDEyX0o1NV9UMTc3X1JFTEE7cmlnaHQ7Nl9jb21wb25lbnRzOzM7NDtyaWdodDs0MTAyMDsxMTAxOzAsMDI3OyA1OzAsMDY1ClN1YmNsdXN0ZXJfNTtIU19EMTM5Ml9DMjlfSjU1X1QxNzdfUkVMQTtsZWZ0OzZfY29tcG9uZW50czswOzM7bGVmdDsgNDg0NTsgMTI0OzAsMDI2OyAzOzAsMDUzClN1YmNsdXN0ZXJfNTtIU19EMzQ3MV9DMjMwX0o1NV9UMTc3X1JFTEE7bGVmdDs1X2NvbXBvbmVudHM7MTszO2xlZnQ7IDkwMDg7IDM0MDswLDAzODsgMzswLDA1MwpTdWJjbHVzdGVyXzU7SFNfRDM0NzFfQzIzMF9KNTVfVDE3N19SRUxBO2xlZnQ7Nl9jb21wb25lbnRzOzA7MztsZWZ0OyA5MDA4OyAyNTI7MCwwMjg7IDM7MCwwNTMKU3ViY2x1c3Rlcl81O0hTX0QzNzczX0M0MTJfSjU1X1QxNzdfUkVMQTtsZWZ0OzRfY29tcG9uZW50czsyOzM7bGVmdDs0MTAyMDsgOTQ5OzAsMDIzOyAzOzAsMDUzClN1YmNsdXN0ZXJfNTtIU19EMzc3M19DNDEyX0o1NV9UMTc3X1JFTEE7bGVmdDs1X2NvbXBvbmVudHM7MjszO2xlZnQ7NDEwMjA7MjE2MzswLDA1MzsgMzswLDA1MwpTdWJjbHVzdGVyXzY7SFNfRDM5OThfQzI2Ml9KNTVfVDE3N19SRUxBO2xlZnQ7NV9jb21wb25lbnRzOzE7MTtsZWZ0OyAyMTI0OyAgNTI7MCwwMjQ7IDE7MCwwMjQKU3ViY2x1c3Rlcl83O0hTX0QzMzIwX0MxX0o1NV9UMTc3X1JFTEE7cmlnaHQ7Nl9jb21wb25lbnRzOzA7MDtyaWdodDsgMzk3OTsgIDc1OzAsMDE5OyAxOzAsMDE5ClN1YmNsdXN0ZXJfODtIU19EMzU2N19DMTJfSjU1X1QxNzdfUkVMQTtsZWZ0OzVfY29tcG9uZW50czswOzM7bGVmdDsgMzAwMDsgIDQ5OzAsMDE2OyAxOzAsMDE2ClN1YmNsdXN0ZXJfOTtIU19EMTQ4OV9DMzE1X0o1NV9UMTc3X1JFTEE7cmlnaHQ7NV9jb21wb25lbnRzOzE7MDtyaWdodDs1MjMyNzsyODE4OzAsMDU0OyAxOzAsMDU0Cg==" download="RELA_spacings_summary.csv">
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
<img src="COBIND_analysis_report_RELA_files/figure-html/PPI-similarity-1.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_1  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/PPI-similarity-2.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_10  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/PPI-similarity-3.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_3  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/PPI-similarity-4.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_4  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/PPI-similarity-5.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_5  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/PPI-similarity-6.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_6  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/PPI-similarity-7.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_7  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/PPI-similarity-8.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_8  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/PPI-similarity-9.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
<p class="caption">**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**</p>
</div>
### cobinder_9  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/PPI-similarity-10.png" alt="**Figure 2. Co-binder motif similarity with matches in protein-protein interactions (PPIs)**" width="1440" />
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

<!--html_preserve--><a href="data:text/csv;base64,YW5jaG9yX3RmO2NvYmluZGVyX2lkO2NvYmluZGVyX21vdGlmX2lkO2NvYmluZGVyX25hbWU7dGZfcGFpcjtwX3ZhbHVlO2NvbWJpbmVkX3Njb3JlClJFTEE7Y29iaW5kZXJfNTtNMDU4NDBfMi4wMDtDRUJQQjtSRUxBOjpDRUJQQjswLDAwMTg0MDc5OzkzNQpSRUxBO2NvYmluZGVyXzc7TTA5OTk0XzIuMDA7Q0VCUEI7UkVMQTo6Q0VCUEI7MCwwMDE5MTIxOTs5MzUKUkVMQTtjb2JpbmRlcl82O00wNTg4N18yLjAwO05GS0IxO1JFTEE6Ok5GS0IxOzAsMDAxOTU4MTk7NzgyClJFTEE7Y29iaW5kZXJfNTtNMDk5OTRfMi4wMDtDRUJQQjtSRUxBOjpDRUJQQjswLDAwMjM2NzU5OzkzNQpSRUxBO2NvYmluZGVyXzU7TTA5OTkzXzIuMDA7Q0VCUEI7UkVMQTo6Q0VCUEI7MCwwMDM0NDI4Njs5MzUKUkVMQTtjb2JpbmRlcl80O00wNTg0MF8yLjAwO0NFQlBCO1JFTEE6OkNFQlBCOzAsMDA1ODQyOTE7OTM1ClJFTEE7Y29iaW5kZXJfNztNMDU4NDBfMi4wMDtDRUJQQjtSRUxBOjpDRUJQQjswLDAwNzE4NzExOzkzNQpSRUxBO2NvYmluZGVyXzc7TTA5OTkzXzIuMDA7Q0VCUEI7UkVMQTo6Q0VCUEI7MCwwMDgwMjkyMjs5MzUKUkVMQTtjb2JpbmRlcl80O00wOTk5NF8yLjAwO0NFQlBCO1JFTEE6OkNFQlBCOzAsMDA5Njc2ODA7OTM1ClJFTEE7Y29iaW5kZXJfNTtNMDI4NTFfMi4wMDtDRUJQQjtSRUxBOjpDRUJQQjswLDAwOTczNDIyOzkzNQpSRUxBO2NvYmluZGVyXzc7TTA3ODMwXzIuMDA7Q0VCUEI7UkVMQTo6Q0VCUEI7MCwwMTUwMTM0MDs5MzUKUkVMQTtjb2JpbmRlcl8xMDtNMDkzNTBfMi4wMDtSRUw7UkVMQTo6UkVMOzAsMDE1NTgzMDA7OTM4ClJFTEE7Y29iaW5kZXJfMTA7TTA0NDU1XzIuMDA7S0xGMjtSRUxBOjpLTEYyOzAsMDE3OTQ4MjA7ODA0ClJFTEE7Y29iaW5kZXJfODtNMDgxNjFfMi4wMDtSRUxCO1JFTEE6OlJFTEI7MCwwMTg0NzUwMDs4NTQKUkVMQTtjb2JpbmRlcl84O01BMTExNy4xO1JFTEI7UkVMQTo6UkVMQjswLDAxODQ3NTAwOzg1NApSRUxBO2NvYmluZGVyXzQ7TTAyODUxXzIuMDA7Q0VCUEI7UkVMQTo6Q0VCUEI7MCwwMTg5Nzk5MDs5MzUKUkVMQTtjb2JpbmRlcl8xMDtNQTE1MTUuMTtLTEYyO1JFTEE6OktMRjI7MCwwMjQ2MzA2MDs4MDQKUkVMQTtjb2JpbmRlcl83O00wMjg1MV8yLjAwO0NFQlBCO1JFTEE6OkNFQlBCOzAsMDI0OTEyNjA7OTM1ClJFTEE7Y29iaW5kZXJfNjtNMDkzNTBfMi4wMDtSRUw7UkVMQTo6UkVMOzAsMDI1NDg1MjA7OTM4ClJFTEE7Y29iaW5kZXJfNTtNMDgxNjFfMi4wMDtSRUxCO1JFTEE6OlJFTEI7MCwwMjg0MTA2MDs4NTQKUkVMQTtjb2JpbmRlcl81O01BMTExNy4xO1JFTEI7UkVMQTo6UkVMQjswLDAyODQxMDYwOzg1NApSRUxBO2NvYmluZGVyXzU7TTAyODUyXzIuMDA7Q0VCUEI7UkVMQTo6Q0VCUEI7MCwwMzQ5MDI5MDs5MzUKUkVMQTtjb2JpbmRlcl83O00wMjg1Ml8yLjAwO0NFQlBCO1JFTEE6OkNFQlBCOzAsMDM2NjQ5NTA7OTM1ClJFTEE7Y29iaW5kZXJfODtNMDk5OTNfMi4wMDtDRUJQQjtSRUxBOjpDRUJQQjswLDAzODI1NjkwOzkzNQpSRUxBO2NvYmluZGVyXzg7TTA5MzUwXzIuMDA7UkVMO1JFTEE6OlJFTDswLDA0MjMzNjQwOzkzOApSRUxBO2NvYmluZGVyXzEwO00wNTg4N18yLjAwO05GS0IxO1JFTEE6Ok5GS0IxOzAsMDQzNTI3MzA7NzgyClJFTEE7Y29iaW5kZXJfNDtNMDk5OTNfMi4wMDtDRUJQQjtSRUxBOjpDRUJQQjswLDA0MzcwNTYwOzkzNQo=" download="RELA_confirmed_pairs.csv">
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
<img src="COBIND_analysis_report_RELA_files/figure-html/no-match-similarity-1.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_1  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/no-match-similarity-2.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_10  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/no-match-similarity-3.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_2  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/no-match-similarity-4.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_3  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/no-match-similarity-5.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_4  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/no-match-similarity-6.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_5  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/no-match-similarity-7.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_6  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/no-match-similarity-8.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_7  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/no-match-similarity-9.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_8  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/no-match-similarity-10.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
<p class="caption">**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**</p>
</div>
### cobinder_9  {.tabset .tabset-pills}    
#### Species-specific motif library {.active}   
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/no-match-similarity-11.png" alt="**Figure 3. Co-binder motif similarity when no matches in interactions (PPIs) were found for those motif pairs**" width="1440" />
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
<img src="COBIND_analysis_report_RELA_files/figure-html/annotations-1.png" alt="**Figure 4. Co-binder regions annotations. Co-binder-specific cobinder-only and full (anchor and co-binder) regions together with regions with and without co-binders.**" width="672" />
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

## cobinder_0_right_0     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/conservation-analysis-1.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_1_right_0     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/conservation-analysis-2.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_10_right_0     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/conservation-analysis-3.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_2_right_0     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/conservation-analysis-4.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_3_left_1     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/conservation-analysis-5.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_4_right_4     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/conservation-analysis-6.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_5_left_3     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/conservation-analysis-7.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_6_left_1     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/conservation-analysis-8.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_7_right_0     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/conservation-analysis-9.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_8_left_3     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/conservation-analysis-10.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
<p class="caption">**Figure 5. Conservation of regions with and without co-binders.**</p>
</div>
## cobinder_9_right_0     
<div class="figure" style="text-align: center">
<img src="COBIND_analysis_report_RELA_files/figure-html/conservation-analysis-11.png" alt="**Figure 5. Conservation of regions with and without co-binders.**" width="960" />
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