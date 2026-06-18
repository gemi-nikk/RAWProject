# RAWProject

Based on the final working tree, divide it like this:

# 1. DevOps & Core I/O Systems Engineer

Owns Core I/O setup, Docker, deployment, and environment.

```text
docker/
├── Dockerfile
├── docker-compose.yml
└── start.sh

config/
├── robot_config.py
└── settings.py

spot_core/
├── connect_spot.py
└── robot_health.py

docs/
├── core_io_setup.md
└── architecture.md

README.md
requirements.txt
.gitignore
```

# 2. Edge Perception & Vision Specialist

Owns image capture, camera handling, image processing, and lock detection.

```text
spot_core/
└── capture_image.py

inspection/
├── lock_detector.py
└── image_processor.py

images/
├── door_1/
├── door_2/
└── door_3/
```

# 3. Autonomy & Mission Logic Programmer

Owns Autowalk, AprilTags, waypoints, and mission flow.

```text
spot_core/
└── mission_status.py

inspection/
├── inspection_runner.py
└── door_inspection.py

autowalk/
├── mission_notes.md
├── waypoint_list.md
└── apriltag_locations.md

docs/
└── apriltag_mapping.md
```

# 4. Integration, Extension & Safety Specialist

Owns database, safety logging, network/localization monitoring, recovery, reports, testing, and final integration.

```text
database/
├── database.py
├── schema.sql
└── db_utils.py

safety/
├── safety_logger.py
├── network_monitor.py
├── localization_monitor.py
└── recovery_manager.py

reporting/
├── generate_report.py
└── export_csv.py

docs/
├── risk_assessment.md
├── database_design.md
└── weekly_contributions.md

reports/
└── inspection_report.csv

tests/
├── test_database.py
├── test_logging.py
└── test_inspection.py

main.py
```

