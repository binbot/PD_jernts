# AGENTS.md - Pure Data FM Generator Project

## Build/Lint/Test Commands
This is a Pure Data (Pd) visual programming project. No traditional build/lint/test commands apply.

- **Run patch**: Open `fm_generator.pd` in Pure Data application
- **Test audio**: Connect audio output and adjust sliders to verify FM synthesis
- **Debug**: Use Pd's built-in debugging tools and print objects

## Code Style Guidelines

### Pure Data Conventions
- Use descriptive object names and comments for complex patches
- Organize objects logically with clear signal flow left-to-right
- Group related functionality with subpatches when patches grow complex
- Use consistent slider ranges (0-1000) for modulation parameters

### Naming Conventions
- Object names: lowercase, descriptive (e.g., `osc~`, `*~`, `dac~`)
- Slider labels: Use tooltips for parameter descriptions
- Canvas naming: descriptive filenames with underscores

### Error Handling
- Use `[catch~]` and `[throw~]` for signal routing errors
- Add `[print]` objects for debugging audio signals
- Validate frequency ranges to prevent aliasing

### Best Practices
- Keep patch complexity manageable - break into subpatches for large projects
- Document signal flow with comments and clear layout
- Test patches across different sample rates and system loads