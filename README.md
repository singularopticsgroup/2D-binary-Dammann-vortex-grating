# 2D-binary-Dammann-vortex-grating
Python code that generates a 2D binary Dammann vortex grating as a phase-only mask for a spatial light modulator (SLM). A Dammann vortex grating splits an incident beam into an array of diffraction orders carrying different topological charges[1], enabling detection of the orbital angular momentum of optical vortices from l = −24 to 24 [2]. This code implements the idea from Ref. [2]. The transition points (`t1`, `t2`, `t3`) are taken from Ref. [3].

Run the code. It creates the binary grating, adds the vortex phase, and saves the result as a `.bmp` file (phase 0–2π mapped to gray levels 0–255) to load on the SLM.

## Parameters

| Parameter | Meaning | Value |
|---|---|---|
| `pX`, `pY` | SLM resolution (pixels) | 1024 × 768 |
| `p` | Pixel size | 19 µm |
| `nx`, `ny` | Number of periods in x and y  | 10, 10 |
| `l1`, `l2` | Topological charge in x and y | 1, 5 |
| `l_p` | Extra vortex charge | −12 |
| `t1`, `t2`, `t3` | Transition points [3] | 0.03863, 0.39084, 0.65552 |

## References

[1] N. Zhang, X. C. Yuan, and R. E. Burge, "Extending the detection range of optical vortices by Dammann vortex gratings," Opt. Lett. 35, 3495–3497 (2010).

[2] S. Fu, T. Wang, S. Zhang, and C. Gao, "Integrating 5 × 5 Dammann gratings to detect orbital angular momentum states of beams with the range of −24 to +24," Appl. Opt. 55, 1514 (2016).

[3] C. Zhou and L. Liu, "Numerical study of Dammann array illuminators," Appl. Opt. 34, 5961 (1995).
