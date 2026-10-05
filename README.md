# Vertical Farm Controller Weather-Aware Scheduling

Build a smart agriculture prototype that uses flow sensor, SHT31 to adapt actions using local weather readings. Include setup instructions, a circuit diagram, tested firmware, and sample output.

## Project details

| Field | Value |
| --- | --- |
| Roadmap ID | 179 |
| Category | Smart Agriculture |
| Platform | Raspberry Pi |
| Difficulty | Beginner |
| Estimated build time | 20 hours |
| Connectivity | RS-485 |
| Core components | flow sensor, SHT31 |
| Control mode | closed loop control |

## Repository layout

- `src/main.py`: runnable firmware or application
- `docs/wiring.md`: suggested low-voltage wiring plan
- `docs/architecture.md`: system data flow
- `docs/test-plan.md`: repeatable verification steps
- `sample-data/example.json`: example telemetry record
- `tools/validate.py`: dependency-free repository validation

## Quick start

1. Run `python -m src.main --iterations 10 --interval 0.5`.
2. Run `python -m unittest discover -s tests -v`.
3. Replace `simulated_values()` with a hardware adapter after bench testing.

## Expected behavior

Weather-Aware Scheduling demonstration with repeatable test steps. The default implementation supports simulated or generic analog inputs so the control path can be exercised before hardware-specific drivers are added.

## Hardware adaptation

The included code is a safe reference implementation. Update pin assignments and sensor conversions from the exact component datasheets, then repeat the test plan before connecting actuators.

## License

MIT
