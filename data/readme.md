## SETP 数据说明

### 目录结构

```text
data/
├── dem/                    # 数字高程模型
│   ├── srtm-c/             # SRTM DEM
│   └── tandem-x/           # TanDEM-X DEM
├── glacier/                # 冰川数据
│   ├── glacier-height/     # 冰川高程与测高数据
│   └── rgi70/              # RGI 7.0 冰川编目
├── glacier-lake/           # 冰川湖边界与水位数据
├── rsimg/                  # 遥感影像
│   ├── glakes-specific/    # 特定冰川湖影像
│   └── setp-region/        # SETP 区域影像
├── setp-boundary/          # 研究区边界
└── readme.md               # 数据目录说明
```

### 数据与用途    

| 目录                        | 数据与用途                                                                                                            |
| --------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| `setp-boundary/`          | SETP、青藏高原及高亚洲边界，用于研究区裁剪与制图。                                                                    |
| `dem/srtm-c/`             | SRTM DEM、分幅及单冰川分析栅格，用于地形与高程分析。                                                                  |
| `dem/tandem-x/`           | TanDEM-X DEM 及拼接结果，用于冰川高程变化分析。                                                                       |
| `glacier/rgi70/`          | RGI 7.0 冰川编目，用于边界参考与面积统计（待补充）。                                                                  |
| `glacier/glacier-height/` | 冰川高程与测高数据，用于高程变化监测（待补充）。                                                                      |
| `glacier-lake/`           | 冰川湖边界与水位数据，用于面积、水位监测（待补充）。                                                                  |
| `rsimg/`                  | 光学影像及配套 DEM，用于深度学习分割；`setp-region/`、`glakes-specific/` 分别存放区域与特定冰川湖影像（待补充）。 |
