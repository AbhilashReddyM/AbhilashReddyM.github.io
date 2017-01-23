class: center, middle
# Computation of membrane bending forces
Abhilash Reddy M

---

# Bending Force

## Helfrich's Formulation

$$\bar{f}_b = E_b \left[(2H+H_o)(2 H^2 -2G -H_oH) + 2\Delta_s H\right]\bar{n} $$

--

If we assume that `\(H_o\)` is that of a plane(=0), we get:

$$\bar{f}_b = 2E_b \left[2H(H^2 -G) + \Delta_s H\right]\bar{n} $$

--

### Things that are needed:

- Normal Vector :  `\(\bar{n} \)`
- Mean Curvature: H
- Gaussian Curvature: G
- Surface Laplacian of H: `\(\Delta_s H\)`



These are all geometrical quantities
---

# Discretized surface

The surface is discretized using flat triangles. `\(\subset^0\)`

<img src="nomesh.png" width="350" height="350" />
<img src="mesh.png" width="350" height="350" />

---

# Normal vector
- Face Normals are well defined for a flat triangle mesh. 
- Not the case for Vertex Normals ...

--

Take weighted average of the face normals that surround a vertex
