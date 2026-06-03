# VIP Project Documentation

Professional documentation for the **Voltage Vandals** Smart Warehouse Robot System (VIP course).

## Contents

| Document | Description |
|----------|-------------|
| [01_project_overview.ipynb (Google Colab)](https://colab.research.google.com/github/melody2004reborn/vip_project/blob/main/docs/01_project_overview.ipynb) | Main course documentation: architecture, modules, workflows, and operational guide |

## How to read

**Google Colab (recommended):** [Open the notebook in Colab](https://colab.research.google.com/github/melody2004reborn/vip_project/blob/main/docs/01_project_overview.ipynb)

Or open [`01_project_overview.ipynb`](./01_project_overview.ipynb) locally in VS Code / Cursor with the Jupyter extension.

## Repository layout (quick reference)

```
vip_project/
├── docs/                    ← You are here
├── src/
│   ├── irobot/              ← Primary ROS 2 package (use this)
│   └── inventory/           ← Legacy initial development
└── other_files/             ← UI, MongoDB seeds, AprilTags, robot bringup
```

## Primary entry points for development

- **Full inventory patrol:** `src/irobot/irobot/Inventory_scan.py`
- **Navigation stack:** `src/irobot/launch/slam_navigation.launch.py`
- **Mapping:** `src/irobot/launch/cartographer_mapping.launch.py`
- **Operator dashboard:** `other_files/Web_interface/receiver.py`

See the notebook for full detail.
