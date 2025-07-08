📦 Gun Data README
markdown
복사
편집
# 🔫 Gun Data Project

이 프로젝트는 다양한 총기(Gun)의 데이터를 구조화하여 저장하고 활용하기 위한 목적의 모듈입니다.  
게임 개발, 시뮬레이션, 군사 교육 자료 등에 응용 가능합니다.

---

## 📂 디렉토리 구조

gun-data/
├── data/
│ ├── pistols.json
│ ├── rifles.json
│ ├── shotguns.json
│ └── snipers.json
├── images/
│ ├── desert_eagle.png
│ └── ak47.png
├── README.md
└── gun_model.py

swift
복사
편집

---

## 📋 데이터 설명

모든 총기 데이터는 `.json` 형식으로 저장되며, 공통 속성은 다음과 같습니다:

| 필드명           | 설명                       | 예시                      |
|------------------|----------------------------|---------------------------|
| `id`             | 총기의 고유 ID              | `"gun_ak47"`              |
| `name`           | 총기 이름                   | `"AK-47"`                |
| `type`           | 총기 종류 (`pistol`, `rifle` 등) | `"rifle"`                |
| `damage`         | 기본 피해량                 | `42`                      |
| `fireRate`       | 초당 발사 속도 (round/s)     | `9.5`                     |
| `reloadTime`     | 재장전 시간 (초)             | `2.7`                     |
| `range`          | 유효 사거리 (미터)          | `350`                     |
| `attachments`    | 장착 가능 부속품 목록         | `["scope", "suppressor"]` |
| `isAutomatic`    | 자동 사격 가능 여부          | `true`                    |

---

## 🧪 예시 데이터 (rifles.json 중 일부)

```json
[
  {
    "id": "gun_ak47",
    "name": "AK-47",
    "type": "rifle",
    "damage": 42,
    "fireRate": 9.5,
    "reloadTime": 2.7,
    "range": 350,
    "attachments": ["scope", "grip", "suppressor"],
    "isAutomatic": true
  },
  {
    "id": "gun_m4a1",
    "name": "M4A1",
    "type": "rifle",
    "damage": 38,
    "fireRate": 11.0,
    "reloadTime": 2.5,
    "range": 400,
    "attachments": ["scope", "laser", "grip"],
    "isAutomatic": true
  }
]
