# LifeSailing

This project contains the questionnaire pages and downloadable role maps.

## Role PDF Mapping

The files in `downloads/` were renamed from `Role-<number>.pdf` to Chinese filenames. Use the table below to map role numbers to the new files:

| Role No. | Filename |
|-------|---------|
| 1 | 索隆型｜角色航行地圖.pdf |
| 2 | 喬巴型｜角色航行地圖.pdf |
| 3 | 魯夫型｜角色航行地圖.pdf |
| 4 | 艾莎型｜角色航行地圖.pdf |
| 5 | 安娜型｜角色航行地圖.pdf |
| 6 | 克斯托夫型｜角色航行地圖.pdf |
| 7 | 奧拉夫型｜角色航行地圖.pdf |
| 8 | 哈利型｜角色航行地圖.pdf |
| 9 | 榮恩型｜角色航行地圖.pdf |
| 10 | 露娜型｜角色航行地圖.pdf |
| 11 | 妙麗型｜角色航行地圖.pdf |
| 12 | 巴斯型｜角色航行地圖.pdf |
| 13 | 小叉型｜角色航行地圖.pdf |
| 14 | 翠絲型｜角色航行地圖.pdf |
| 15 | 歐比王型｜角色航行地圖.pdf |
| 16 | 黛西型｜角色航行地圖.pdf |
| 17 | 韓索羅型｜角色航行地圖.pdf |

## Download Logic

Inside `Result.html`, the recommended character image name (e.g. `Role-05.png`) is used to extract a numeric id. The script looks up the Chinese filename from the `ROLE_FILENAMES` table and builds the path `downloads/<filename>` accordingly. A temporary anchor is created with this path so the browser downloads the PDF using the same filename.
