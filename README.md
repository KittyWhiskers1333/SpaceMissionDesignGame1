# ORBIT FOUNDRY — Version 2

A browser-based 3D spacecraft design and mission adventure prototype. Built with HTML, CSS, JavaScript and Three.js.

## Included
- Cinematic-style home screen, story briefing and mission cards.
- Ten randomly assigned mission storylines with distinct destinations, hazards, objectives and science instruments.
- Interactive spacecraft configurator: structure, propulsion, power, communications, thermal control, science instruments, surface systems and protection.
- 3D ship model, drag-to-rotate, zoom, and subsystem swaps.
- Mission readiness, build credits, mass and power trade-offs.
- Launch countdown and launch telemetry.
- 3D flight scene with planet, stars, beacon radar, chase/cockpit camera, keyboard controls, resources and mission tools.
- Science capture, data transmission, return attempt, repair/diagnostics panel, failures and debrief.
- Completion tracking for all ten unique missions and finale/replay screen.

## Run locally
This uses Three.js from a CDN, so internet access is required.
1. Extract the ZIP.
2. Open a terminal in the project folder.
3. Run `python3 -m http.server 8000`
4. Visit `http://localhost:8000`

You can also open `index.html` directly in a modern browser, but a local server is more reliable.

## Publish on GitHub Pages
1. Create a GitHub repository named `orbit-foundry`.
2. Upload `index.html`, `style.css`, `game.js`, and `README.md` to the repository root.
3. Open Settings → Pages.
4. Select Deploy from a branch → `main` → `/(root)` → Save.
5. Wait for the Pages URL to appear.

## Controls
- Shipyard: drag the model to rotate, scroll to zoom, or use the rotation buttons.
- Flight: W/S thrust and reverse; A/D yaw; arrow keys pitch; Space stabilizes; Shift boosts (uses extra fuel).
- E: use mission instrument; T: transmit data; R: diagnostics/repair; H: return/dock; Esc: pause.
- On screen: buttons work with mouse/touch.

## Scientific grounding and limitations
The component categories are informed by NASA educational resources on spacecraft systems and science instruments:
- NASA Basics of Space Flight, Onboard Systems: https://science.nasa.gov/learn/basics-of-space-flight/chapter11-1/
- NASA Basics of Space Flight, Science Instruments: https://science.nasa.gov/learn/basics-of-space-flight/chapter12-1/
- NASA Small Spacecraft Systems Virtual Institute, State of the Art: https://www.nasa.gov/smallsat-institute/sst-soa/platforms/

This is an educational game prototype, not an engineering design tool. The spacecraft model and physics are stylized; numeric mass, credits, power, fuel, hazard rates and flight dynamics are game-balancing values rather than flight-certified or specific NASA hardware specifications. Real spacecraft designs require mission-specific orbital mechanics, thermal/radiation analysis, structures, propulsion performance, communication link budgets, fault tolerance, and validated instrument requirements.

## Further development ideas
- Use glTF models and animations for a detailed cockpit, robotic arm, lander and instrument mechanisms.
- Replace simplified motion with orbital mechanics and collision volumes.
- Add mission-specific interaction minigames, science data visualizations and more nuanced repair procedures.
- Save progress in browser storage or a backend; this prototype intentionally keeps progress in the current page session.
- Add accessibility options, subtitles, touch-specific flight controls, audio and reduced-motion settings.
