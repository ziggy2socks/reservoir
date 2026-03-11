# Dark Mode Reference

To switch back to dark mode, change these values in index.html:

## CSS
- body background: #000
- .project-item color: rgba(255,255,255,0.35)
- .project-item hover/active: var(--accent, #fff)
- Mobile gradient: rgba(0,0,0,0.85)
- Mobile pill border: rgba(255,255,255,0.12)
- Mobile pill bg: rgba(255,255,255,0.04)
- Mobile pill active bg: rgba(255,255,255,0.08)

## JS
- renderer.setClearColor: 0x000000
- scene.fog: new THREE.FogExp2(0x000000, 0.008)
- COLORS.studio:  0xa8c8ff  (cool blue-white)
- COLORS.bid:     0xC9A84C  (gold)
- COLORS.pulse:   0x00d4ff  (cyan)
- COLORS.radar:   0x00ff88  (green)
- COLORS.datamap: 0xff6b35  (orange)
- Particle size: isMobile ? 0.7 : 0.4
- Re-enable UnrealBloomPass: strength 1.4, radius 0.35, threshold 0
  (wrap in `if (!isMobile)` block)

## Notes
- Bloom looks great in dark mode, wrong in light mode
- Dark = cinematic/tech, Light = editorial/Swiss modernism
- Both particle counts (20k desktop / 6k mobile) stay the same
