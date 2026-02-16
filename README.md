## Target-Program-Data

<table>
  <tr>
    <th>OSS</th> <th>bug ID</th> <th>fix commit</th> <th>fix file</th> <th>bug rows</th>
  </tr>
  <tr>
    <td rowspan="4">find</td>  <td>find-1</td> <td>c8491c1</td> <td>parser.c</td> <td>1505, 1523</td>
  </tr>
  <tr>
    <td>find-2</td> <td>dbcb10e</td> <td>parser.c</td> <td>3195</td>
  </tr>
  <tr>
    <td>find-5</td> <td>07b941b</td> <td>parser.c</td> <td>1645</td>
  </tr>
  <tr>
    <td>find-14</td> <td>9362375</td> <td>parser.c</td> <td>889, 890, 940, 941, 942, 1998, 2013, 3428</td>
  </tr>
  <tr>
    <td rowspan="3">gpac</td>  <td>gpac-1</td> <td>c22c0bb</td> <td>configfile.c</td> <td>113, 116</td>
  </tr>
  <tr>
    <td>gpac-3</td> <td>c22c0bb</td> <td>os_file.c</td> <td>686, 771, 772, 780, 782</td>
  </tr>
  <tr>
    <td>gpac-4</td> <td>c22c0bb</td> <td>data_map.c</td> <td>360</td>
  </tr>
  <tr>
    <td>gdbm</td> <td>gdbm-1</td> <td>988d360</td> <td>gdbmload.c</td> <td>76, 77, 87, 114, 126, 128, 144, 154, 161, 226</td>
  </tr>
  <tr>
    <td rowspan="3">lua</td> <td>lua-1</td> <td>2bfa13e</td> <td>ldo.c</td> <td>415</td>
  </tr>
  <tr>
    <td>lua-2</td> <td>cf613cd</td> <td>ldo.c</td> <td>536</td>
  </tr>
  <tr>
    <td>lua-3</td> <td>ad3942a</td> <td>ltable.c</td> <td>153, 154, 156, 157, 160, 164</td>
  </tr>
  <tr>
    <td rowspan="2">bluez</td>  <td>bluez-1</td> <td>00eea35</td> <td>sdp-xml.c</td> <td>548</td>
  </tr>
  <tr>
    <td>bluez-2</td> <td>5573661</td> <td>textfile.c</td> <td>130, 131, 132, 133</td>
  </tr>
  <tr>
    <td rowspan="2">hdf-5</td> <td>hdf5-1</td> <td>9e765b9</td> <td>H5Ofsinfo.c</td> <td>97, 98, 99, 100, 101, 117, 118, 132, 133, 146, 205, 206</td>
  </tr>
  <tr>
    <td>gdf5-2</td> <td>1126b83</td> <td>H5FSsection.c</td> <td>934</td>
  </tr>
</table>

## Average rank of bug-fixing locations
### AFL
| Target program |  Barinel  |   Dstar   |  Ochiai   |    Op2    | Tarantula |
|:---------------|:---------:|:---------:|:---------:|:---------:|:---------:|
| find-1 | 23.54 | 71.16 | 9.14 | 14.58 | 23.54 |
| find-2 | 11.37 | 20.95 | 6.2 | 20.95 | 6.2 |
| find-5 | 18.25 |6.4 | 3.2 | 3.2 | 4.8 | 
| find-14 | 18.42 | 18.42 | 18.42 | 5.93 | 18.42 |
| gpac-1 | 85.94 | 85.94 | 85.94 | 20.68 | 85.94 | 
| gpac-3 | 95.12 | 90.24 | 95.12 | 69.81 | 95.12 | 
| gpac4 | 87.5 | 87.5 | 87.5 | 33.3 | 87.5 | 
| gdbm-1 | 38.33 | 42.7 | 42.7 | 31.58 | 38.33 |
| lua-1 | 2.16 | 2.16 | 2.16 | 2.0 | 2.16 |
| lua-2 | 45.78 | 45.78 | 45.78 | 33.33 | 45.78 |
| lua-3 | 21.43 | 20.37 | 20.37 | 16.67 | 21.43 |
| bluez-1 | 54.29 | 47.62 | 47.62 | 40.68 | 54.29 |
| bluez-2 | 48.67 | 12.00 | 4.67 | 4.31 | 48.67 |
| hdf5-1 | 38.72 | 38.72 | 38.72 | 23.16 | 38.72 |
| hdf5-2 | 33.33 | 33.33 | 33.33 | 33.33 | 33.33 |

### AFL++
| Target program |  Barinel  |   Dstar   |  Ochiai   |    Op2    | Tarantula |
|:---------------|:---------:|:---------:|:---------:|:---------:|:---------:|
| find-1 | 39.13 | 80.53 | 39.13 | 23.89 | 39.13 |
| find-2 |  |  |  |  |  |
| find-5 | 18.29 | 100 | 18.29 | 50.48 | 18.29 | 
| find-14 | 36.92 | 14.89 | 14.89 | 20.28 | 36.92 |
| gpac-1 | 87.50 | 85.94 | 85.94 | 12.7 | 85.94 |
| gpac-3 | 72.72 | 72.72 | 72.72 | 72.72 | 72.72 |
| gpac4 | 36.58 | 36.58 | 36.58 | 21.95 | 36.58 |
| gdbm-1 | 34.37 | 45.53 | 31.10 | 26.9 | 34.37 |
| lua-1 | 2.11 | 2.11 | 1.97 | 1.97 | 2.11 |
| lua-2 | 34.31 | 34.31 | 34.31 | 31.96 | 34.31 |
| lua-3 | 21.43 |21.43 | 21.43 | 15.10 | 21.43 |
| bluez-1 | 82.76 | 77.01 | 77.01 | 73.56 | 82.76 |
| bluez-2 | 33.12 | 34.74 | 36.69 | 29.93 | 33.12 |
| hdf5-1 | 24.40 | 27.11 | 29.38 | 21.49 | 24.40 |
| hdf5-2 | 46.98 | 46.98 | 46.98 | 37.66 | 46.98 |
