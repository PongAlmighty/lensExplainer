# lensExplainer

An interactive, single-file explainer for how a camera lens and sensor turn light into a picture. Move a slider and watch the lens internals, the sensor, and the final image respond.

Open `index.html` in any modern browser. No build step, no dependencies.

## What it shows

- **Final picture** with live depth of field, bokeh shaped by the iris, motion blur, noise, exposure and clipping, vignetting, and diffraction softening, plus an exposure meter in stops.
- **Lens cross-section** with rays from the subject and the background, light blocked by the iris, and the blur disc each point makes on the sensor.
- **Iris and rotary shutter** views, with the shutter wedge spinning at the frame rate.
- **What's happening** panel that explains the current settings in plain language.

## Controls

| Control | Range |
| --- | --- |
| Aperture | f/1.4 – f/22 in 1/3 stops |
| Shutter | **angle** 11.2° – 360°, or **speed** 1/24 – 1/8000 (toggle between them) |
| Shutter type | mechanical rotary disc, electronic rolling, or electronic global (rolling adds a lean to fast sideways motion) |
| Frame rate | 23.976 – 120 fps |
| ISO | 100 – 25600, with an optional dual-native ISO mode (400 / 3200) |
| ND filter | none, 2, 4, 6 stops |
| Focal length | 18 – 135 mm |
| Focus distance | 0.5 m – ∞ |
| Sensor | Super 35 or Micro Four Thirds |
| Scene | night, indoors, outdoors at golden hour, outdoors in daylight (independent of brightness) |
| Scene brightness | EV 1 – 16 |

There are also presets (cinematic 24p, dreamy portrait, deep-focus landscape, freeze the action, motion blur, night street) and a camera row (Blackmagic Micro Studio Camera 4K G2) that only changes camera settings, plus 25, 55 and 120 mm lens buttons that change only the focal length.

## About the model

This is a teaching tool, not a measurement tool. It uses thin-lens optics, circle-of-confusion blur, and a stylised exposure and noise curve. The trends are right; the exact numbers are not those of any particular camera or lens.
