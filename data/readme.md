## SETP 数据说明

### 目录结构

以下为当前本地数据目录，TanDEM-X 产品目录及批量栅格文件作合并展示。

```text
data/
├── dem/                                # 数字高程模型
│   ├── srtm-c/                         # SRTM DEM 与分析结果
│   │   ├── individual_glaciers_analysis/ # 单冰川分析栅格
│   │   ├── tiles_1deg_SRTMGL1/          # SRTMGL1 分幅数据
│   │   ├── setp_SRTMGL3.tif
│   │   ├── setp_SRTMGL3_005deg.tif
│   │   └── setp_SRTMGL3_utm46.tif
│   └── tandem-x/                       # TanDEM-X DEM 与拼接结果
│       ├── TDM1_DEM__30_*/              # 各分幅产品目录（合并展示）
│       ├── TDM90-url-list.txt
│       ├── dems_mosaic.tif
│       ├── dems_mosaic_subs.tif
│       └── dems_mosaic_subs_utm.tif
├── glacier/                            # 冰川数据
│   ├── glacier-height/                 # 冰川高程与测高数据（空目录）
│   └── rgi70/                          # RGI 7.0 冰川编目（空目录）
├── glacier-lake/                       # 冰川湖数据（空目录）
├── isat-2/                             # 测高数据预留目录（空目录）
├── rsimg/                              # 遥感影像及配套 DEM
│   ├── glakes-specific/                # 特定冰川湖影像（空目录）
│   ├── setp-region/                    # SETP 区域影像（空目录）
│   ├── l5_scene_01_dem.tif
│   └── l5_scene_01_nor.tif
├── setp-boundary/                      # 研究区边界
│   ├── TPBoundary_new2021.gpkg
│   ├── hma_bolch2019.gpkg
│   ├── setp.kml
│   └── setp_zhao2022.gpkg
└── readme.md                           # 数据目录说明
```

### 数据与用途

| 目录 | 当前数据与用途 |
| --- | --- |
| `setp-boundary/` | SETP、青藏高原及高亚洲边界，包含 KML、GeoPackage 文件，用于研究区裁剪与制图。 |
| `dem/srtm-c/` | SRTMGL1 分幅、SETP SRTMGL3 栅格及其派生版本；`individual_glaciers_analysis/` 存放单冰川分析栅格，用于地形与高程分析。 |
| `dem/tandem-x/` | TanDEM-X 分幅产品目录、下载 URL 列表及 DEM 拼接、子集和投影处理结果，用于地形与冰川高程变化分析。 |
| `glacier/rgi70/` | 预留 RGI 7.0 冰川编目目录，用于边界参考与面积统计，目前为空。 |
| `glacier/glacier-height/` | 预留冰川高程与测高数据目录，用于高程变化监测，目前为空。 |
| `glacier-lake/` | 预留冰川湖边界与水位数据目录，用于面积、水位监测，目前为空。 |
| `isat-2/` | 测高数据预留目录，目前为空；目录名按现有拼写保留。 |
| `rsimg/` | 已有 `l5_scene_01_nor.tif` 影像及配套 `l5_scene_01_dem.tif`；`setp-region/`、`glakes-specific/` 分别预留区域与特定冰川湖影像，目前为空。 |
