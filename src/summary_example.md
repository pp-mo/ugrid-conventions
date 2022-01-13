# UGRID checker file summary
File : `/project/avd/ng-vat/data/lfric_C96_aquaplanet_diag.nc` 

## File mesh structure
### Meshes
-   `Mesh2d_edge_half_levels`
    -   node(`nMesh2d_edge_half_levels_node`)
        -   coordinates : `Mesh2d_edge_half_levels_node_x`, `Mesh2d_edge_half_levels_node_y`
    -   edge(`nMesh2d_edge_half_levels_edge`)
        -   edge_node_connectivity : `Mesh2d_edge_half_levels_edge_nodes`
        -   coordinates : `Mesh2d_edge_half_levels_edge_x`, `Mesh2d_edge_half_levels_edge_y`
-   `Mesh2d_full_levels`
    -   node(`nMesh2d_full_levels_node`)
        -   coordinates : `Mesh2d_full_levels_node_x`, `Mesh2d_full_levels_node_y`
    -   edge(`nMesh2d_full_levels_edge`)
        -   edge_node_connectivity : `Mesh2d_full_levels_edge_nodes`
        -   coordinates : `Mesh2d_full_levels_edge_x`, `Mesh2d_full_levels_edge_y`
    -   face(`nMesh2d_full_levels_face`)
        -   face_node_connectivity : `Mesh2d_full_levels_face_nodes`
        -   coordinates : `Mesh2d_full_levels_face_x`, `Mesh2d_full_levels_face_y`
-   `Mesh2d_half_levels`
    -   node(`nMesh2d_half_levels_node`)
        -   coordinates : `Mesh2d_half_levels_node_x`, `Mesh2d_half_levels_node_y`
    -   edge(`nMesh2d_half_levels_edge`)
        -   edge_node_connectivity : `Mesh2d_half_levels_edge_nodes`
        -   coordinates : `Mesh2d_half_levels_edge_x`, `Mesh2d_half_levels_edge_y`
    -   face(`nMesh2d_half_levels_face`)
        -   face_node_connectivity : `Mesh2d_half_levels_face_nodes`
        -   coordinates : `Mesh2d_half_levels_face_x`, `Mesh2d_half_levels_face_y`

### ?? Connectivities with no mesh ??

-   `Mesh2d_full_levels_face_edges`  ( `nMesh2d_full_levels_face`, `nMesh2d_full_levels_vertex` )
    -   cf_role = `face_edge_connectivity`
-   `Mesh2d_half_levels_face_edges`  ( `nMesh2d_half_levels_face`, `nMesh2d_half_levels_vertex` )
    -   cf_role = `face_edge_connectivity`

### Mesh Data Variables

- `area_fraction`
    - mesh : `Mesh2d_full_levels`
    - location : `face`


## Checker Errors and Warnings

### Summary 

Total of 10 problems logged :

| n | type |  |
| --- | --- | --- |
| 1 | Rxxx | requirement failures |
| 9 | Axxx | advisory recommendation warnings |

### Details

| type | code | comment |
| ---  | ---  | --- |
| <span style="color:red"> **FAIL** </span> | [R113](../conformance/#R113)  | Mesh variable `Mesh2d_edge_half_levels` has topology_dimension=`2`,<br> but it has no 'face_node_connectivity' attribute. |
| WARN | [A307](../conformance/#A307) | Mesh connectivity variable `Mesh2d_full_levels_face_edges` has<br> _FillValue=`999999`, which is not negative. |
| WARN | [A301](../conformance/#A301) | connectivity variable `Mesh2d_full_levels_face_edges` has no parent mesh. |
| WARN | [A307](../conformance/#A307) | Mesh connectivity variable `Mesh2d_half_levels_face_edges` has<br> _FillValue=`999999`, which is not negative. |
| WARN | [A301](../conformance/#A301) | connectivity variable `Mesh2d_half_levels_face_edges` has no parent mesh. |
| WARN | [A903](../conformance/#A903) | dataset has Conventions=`UGRID`, which does not contain a UGRID convention<br> statement of the form `UGRID-<major>.<minor>`. |
| WARN | [A905](../conformance/#A905) | netcdf variable `Mesh2d_full_levels_edge_face_links` has<br> cf_role=`edge_face connectivity`, which is not a recognised cf-role value<br> defined by either CF or UGRID.|
| WARN | [A905](../conformance/#A905) | netcdf variable `Mesh2d_full_levels_face_links` has<br> cf_role=`face_face connectivity`, which is not a recognised cf-role value<br> defined by either CF or UGRID.|
| WARN | [A905](../conformance/#A905) | netcdf variable `Mesh2d_half_levels_edge_face_links` has<br> cf_role=`edge_face connectivity`, which is not a recognised cf-role value<br> defined by either CF or UGRID.|
| WARN | [A905](../conformance/#A905) | netcdf variable `Mesh2d_half_levels_face_links` has<br> cf_role=`face_face connectivity`, which is not a recognised cf-role value<br> defined by either CF or UGRID.|

